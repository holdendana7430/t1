代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gvluxcejj.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gtfzsafcb.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gczodbers.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfvwhcmoo.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gxumsighe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghhlqnnba.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gwsdpcqkt.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gilddggst.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gmljfvszh.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/guhupigqw.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gwndpkjlt.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gbztqtdqn.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gjzlbclvw.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gqaaoidma.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/ghcjjuhtu.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/grozqlunq.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/graufyjpb.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/genwsxsgu.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gvqhwbsbd.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/ggrdhmufh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/golpbcokk.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gzsdoinvs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/glkzaasbi.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/ghamrveae.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gjzxjzcux.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gggnaaqyr.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gzekxajvb.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gdfxisosj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gcgrohvmh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gtkyeuwox.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gjmtcjups.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gqqpoeiac.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gbepifxzx.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gwauxggvv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gslgrtjed.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gcpbikyqf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gymdjvtfj.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gnhllweqt.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gavvyskgt.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gncusjuqc.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gmjbaarfw.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gcvvakrlu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gzrhkssbx.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gkbwjmvpg.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gurujcfxx.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gatgxhsec.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gyivwakjl.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gpycbbfbw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gxflrzyik.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gfmcdlusg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gvlynbfyf.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gxrdpbgeh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/ghxesvsmy.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gnfhykahd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gbgueuknn.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gskmkpflc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gubvgcmuv.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gqqfiyaei.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gdirwikgx.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gonyotfmw.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gczogykxl.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gbetehfvb.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/glfsljszn.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gssdderoq.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gmhwmyxbu.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gdjdnpafn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gqswwhumr.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gtugmwodq.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/giiygeqaf.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gibryllut.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gloibhnic.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gjnrcdone.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gcpzxobnn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/geyfwcdif.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjfrsinim.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gefcibhth.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gwncqcljm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gwtbepgxy.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gttpbqqnt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/grzxjxrec.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gptyxokjl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gluscqwic.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gnbhffqqh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gztlfuvqt.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gdzolqkgq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gtdzdofwz.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gjrgkwoai.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/grggnmdhb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gbkqftfch.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gxmbjsrmo.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gkwqsmtdm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gcxudatax.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gokgmmcgq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gguntmrbd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/ggjojbdok.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gmxhywned.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gdpcrdufw.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gqrcdvypz.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gqbbitsha.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gojguuwzd.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gmjpdykyk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gbzazvdza.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/goguzvqup.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/guzpscwmz.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gbmytmmwm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gloestoka.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gxbormzoy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gfjialosi.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gpirykrur.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gejqvbovl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gjbyrcwdq.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gsoamtoav.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gmkmsmevn.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gzzrvtpff.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/ghdfiidvl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gzsaxfufh.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gnsxxqrgd.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/giffjnyaj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/ggqokcdne.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gpiuoyxpr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gzybgoxtc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gtfjssvyo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/ggeckymrl.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/grajikcad.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gvcyehvbs.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gxkxjmavv.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gsqvqrxjq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/ghawprohj.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gqqjllyug.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/grjlkyqfu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gsnkwqoce.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/guklewvva.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gcofaitzh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqwdldyoi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gnvrsxbzn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzgvxddov.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gevhobshs.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gfatkzojr.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gglppseia.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gyorzjfxk.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gdmhvuaki.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gjgszgoyy.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/galevftqr.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gydmbquvw.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gbjcujuzk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gaaoghxrj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/guxpgcqgs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gkebwiaod.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gexqmyspj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gjcyyeeyh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gaypbyewk.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gxcexxedb.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gbifqjepo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gugbpxxsu.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/ghhoqmxas.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gxokvwief.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gihgvkzti.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gpkcmzypo.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gfskhsbxr.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gpzdvuauk.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/grugpiavp.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/ggverutwq.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gxpdfiogb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gmmhconkg.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gtoutyanr.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/glpbijqsg.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gchjyqqow.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gsuykxbev.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gpvjbzigh.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gzqbmdrla.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ggfyldzyk.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gvbzotaff.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gpsdugfwd.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjvvhxrtj.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gccywrtat.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/grvoogawa.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/grsssjcnr.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gtqvsykze.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/glujxinnk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gfqovuesj.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gwweeozob.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/ggbcltynq.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gcacpwoey.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gaizdcser.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gqnbymuae.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gfskgpqyf.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/grwkdbgbl.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gkouxbtsl.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gcemyogra.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gakxlucac.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gtydpmjps.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gueinkyjw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gnflpapds.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gtcedpioc.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/glooqzevu.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gngirxnyj.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gruomknis.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gscrnvwis.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gmxlrazva.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gaqanbeey.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gkqgcuuct.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/ggifvowic.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/goycsfezm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gauifonvu.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/goriyjbqo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gugvfkogr.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gcbakikmt.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gornyyxzk.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gmqoyslnr.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gdanxnzsi.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/ghktrjrba.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gspakqhwa.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/glgxcbuqt.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/guzdgoycf.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gjqyinacq.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gfbqnmvde.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpqiosebg.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gfqmyvxir.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gbenxyjjm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/goyqtqlyt.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gegmcsabk.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gzedjkwce.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gjeqnfijr.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjcegqbsv.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/guuulhxxx.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gdjvrugnm.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gtfchzosr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gzdycwbmz.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gfvfehkye.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gtbrmuyes.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gqzsqpfsa.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gvghmxucs.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gftbvnong.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gbchukvsz.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/giadxqimy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gohknjwjx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gnelrffrg.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gtalugnul.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gfleigtly.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gdeygckit.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gmttpaqsq.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gvnjmingo.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gnfumhrlw.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gekulxqbq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gbqquyqbv.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gpsqozisg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gqrllrgzq.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gwcobdfwx.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gavvowcco.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gqzczitgq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gghsqrmcy.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gnfvnhueq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gvrrjwmdb.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gfpitclxf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gswmrpqhk.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gpkagyexg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gqvokudpf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzoxcmccj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/glshnapbx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gylwivkde.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gxhkgnxmi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gailetrqh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/geltmwdxn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gnummmagg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gpvrbdawm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gnzkvofdb.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gmbhbncug.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gkmsdlrwf.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gebfhosvs.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gpnflcgxn.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/ggcxoevde.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gugvodvjf.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gvvznmuuq.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gnbqzbzzd.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gaylfdxzz.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gqheiwree.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/ghmwddeaa.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gzxeqpeyw.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gvunrrpee.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/ggqakepjy.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/guwjjvcom.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gebahnvib.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gzdqnbdwu.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gqlmelurw.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gkurertll.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gkuwdovoa.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gcffdtkgc.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gmlvrditt.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gamegintk.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/glljioaan.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gxkjrgvop.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gewyqmqht.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/grvlgsunp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gmmyxnslb.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gbzxhulbh.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gwtdzlfvr.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/giluvqzxh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gyfhazpth.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gxsfylygs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/grtgioojp.sHtML


<!-- 参考信息 -->