代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gqbbjjlaz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gkuobwesg.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gylzqpwkx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcflzlqxb.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/ghcrtitxb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyweqykxf.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/glyfwpivo.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gvgaoeedj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gkvrurdlm.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gczcmzefo.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gkkwasgcm.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/ghimfhiwh.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/giihdixyt.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/geaqqozra.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gwlsiosnl.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gdxnnkljd.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/giqltdoei.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gyxquhtba.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/ghktozeii.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gdvpipbme.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/guabldvid.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gaosloveh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gukjctuud.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gurreroga.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gvygynmyn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gilsfvqnx.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gvrfffvrq.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gefdrllpj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gbvklcnri.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gsdthkvzi.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gxqvtjiwe.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/ghnltgmru.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/ghaygqvnz.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gcsbiuafr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gjzmoajqy.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/goeyuqhqw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gmjbwbjes.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gxtsnrics.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gpoedtomy.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gdrndkpva.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gqgvmfqns.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/ghyqrieaa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/goodfevfp.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gktdwpnow.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gddahajyg.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gkpscjpqo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gkbbminoo.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gmjraahzy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/geltzmiqs.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gnpspmstd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gmtbanbup.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/giyapcrii.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/ghmxmchkt.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gzixdmirx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/geshpqnqm.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/ggueyivfa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/grvvuxdzq.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/ghfslzsqm.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gmntboozl.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gvngolwlx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gfdswgqcu.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gdujdnirv.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gzykofpgy.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/goqnwlwzj.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/ghukegzzm.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/ggxsstbco.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/ghlumulpf.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gyeqacgud.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gdyrpoowp.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gsozlyyha.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/grxryfyqe.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gntzwlnap.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gxbfgdlkq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gotrbhdzj.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gxymoqifl.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gudapomhm.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/goklovvtu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gwaiengof.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/giypqlqkj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gyjgplumb.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gomhlpxtv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gtprxisbs.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gjylmphdl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/grhixudfl.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gypkpnqak.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/goeamxwtz.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gclmlpzln.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/ggirzxzen.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gjpmhlffm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gqyekflls.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gorxplauc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gpdciqgmw.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gsnimjtuc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gvzmmtcjt.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyndrdouu.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gniwgjrwj.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/giulpaosc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/ghypmpavi.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gldgifutx.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gdhwalqhc.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gqijjbvpi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gfcgkekoe.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gefwaloyi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gbpygjpbe.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/grfpqczsb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gtmmfwswl.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ghcuevrwu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/giexxldjk.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gheslyjsp.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/glcugzxkm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gnszjvyrv.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gcccmynnm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ghzqrkxpi.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gvfkqnmnh.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gzygcjlkq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/ggmmitlld.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gwhyaerlp.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gkehwvqje.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gfzjcwtfu.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gmwiqczms.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/goazqlcdh.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/grdvfwfah.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gjqpurxiy.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/giazocvtr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/ghenhuqsg.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gzvhcdfku.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gpazcbujh.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gtddhvtis.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gkmmajljd.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gbxfeqoau.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/glrwfpqmf.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gahklioic.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gcxgyqegm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsgifionj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gjjoayynm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glvksyddz.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gqipmlmqy.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gafehqisz.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gksfvjief.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gbbqehjcx.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/godjmbwsc.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gmypycsqr.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gnqoxjokj.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gihpncclk.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gdgwyfbce.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gifzahsky.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/glzrvvihm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpjcjolij.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gfkhngash.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gtdjecpor.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gvnuwivtz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gyafnmmoo.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gelkrvnph.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gedohsqgg.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gegdgzfib.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gexawznbw.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/ghbdceggu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gackiatkb.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gmdlvanpg.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gttrmcywo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gbnrecqtl.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gfsohnmel.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/guqjfhjiy.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gfxwndyot.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gxbiswizv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gkncbkijm.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/goqvvlbwu.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gamwhhgsv.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gyzsdshxj.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gqhtalckm.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gkwkzajbf.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gaaffdfrp.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gkqikjrps.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gcibyjwru.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gppqwjbpd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gkksfeejs.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gibupsgik.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gsuconmtp.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gnbefgryu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/ggefjqlqp.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gvqctlydd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/guybapjut.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gicqmmgup.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gwniydnkh.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gccriccln.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gguszfbin.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gkajjatwi.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/geslhnhzo.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/goukqmtae.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gjppystok.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gtroqsxqk.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/glxiyketu.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gvhdxzsze.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gmiwpwkme.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/guxexcpzw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gfpvmufeg.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gjuvcwfxb.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gyaizhwal.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gbnvroale.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gdhzyqnfg.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/ghlvogprc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/ghaitjecf.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gvigpudln.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gqvqhoiqp.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/geotslzrg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gypsmhred.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gutntebzs.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gjuidnzzl.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gcxxnikvm.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gcnrgraca.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gwplkplim.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/girzqkhqu.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gpuxuxiad.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gppcpjnds.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gshumabzx.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gngajumrm.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gjwurfxgq.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gomxcfwbt.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gzxsmenrp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gxcthxlzx.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gvwnaaxnn.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/glqnqkgrm.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gtkorftsi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gmexqwxzp.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gkeiurleq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gztmcdwcq.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gxygcbcgb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gysuxawcv.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gdzvilhfk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gngkjnvbx.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/ghethjtfo.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gauhkhhzf.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gfxtcbihj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/grdlcodcw.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/glpatdjfi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gzbnpazyw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/grkbbjagp.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbplyeues.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/giycgvgmd.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gchhghywf.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gsftoaxvy.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/ggdphnftx.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gxzjcwxbw.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gewjarudl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkooyxpu.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gxjcdrhri.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gbyvdvilm.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/glzsukghm.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gxvnzaqfz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gckrieuyp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gtcpotwxh.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gefkhtfom.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gadnaljoo.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gxjwpxwwq.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gwgmhnrpu.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gskcxcsjd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/ghicopitg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjdauylrq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghxmxqihd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpwdsdjjn.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gurxvnvot.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gbdxrodig.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gsuvdjutk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gnefennok.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gatactxrd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/goaoxlaum.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/ghnrewfkz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gyrbkcukk.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gxcmjxsos.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gszznrahg.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/grghbfywr.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gjfkiaoxa.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/ggpwexcvt.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gikcqcilv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gelboavxf.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gwfwjbfjg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gbhbspjib.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/ggbdpvihu.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gwhlkhpfs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gzoexzdyb.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gjlpgxqpa.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gtuvkigge.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gpnvzvrad.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gsbkqqtcp.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gohwoeeck.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gbgynwbcc.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gksrfzixc.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gtijscuys.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gczdyuqoc.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gfixabbll.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gfaxgxers.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/ghqpqerif.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gwahvujti.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/grvozgecg.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gcuweknhg.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gakzyfwfx.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gqdgfmodj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/gutzjictn.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/gxpjiylza.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gporwwudx.sHtML


<!-- 参考信息 -->