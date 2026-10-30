代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gevbxcbjm.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/giztudivg.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gsrbdxdfl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ganblkvfo.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gfmlysokp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gysgtpent.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwqwbuvgg.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/geynszucg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gmwnfhkti.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gklcmxwpc.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gtxcvdoka.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gijlcukaf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gwynlalml.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gtimiktvl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gkvkicpah.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gvlgfembh.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gvwnqansr.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/grtmxkwhm.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/grmtfihlc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gxjydzufd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gilsuguex.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gfhdzfgad.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gtxlbrujv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/grewnwcyx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gllgznfbv.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gdfjtvelh.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gdzkjbgsw.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gfthbkxpi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gyjxgqljs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gjgoyfthh.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gavvcsadx.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gkjwrqcjg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gnwsiruag.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gdagtvddw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gzixephgu.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gqxqdmadu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gikqtnfgv.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gqrrlrscy.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gdyuydiqs.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/glpvnmvkh.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gnlskvetb.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjshpwyjc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gyckyduzd.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gouomwblq.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gjpnbceeg.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gqndcqzsd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gombmtjeh.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gavheyzef.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gttpuiokm.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gxwpqikdq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gewoezith.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gzrmoydcf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gxwlkqkga.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gbfzerpvn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/grbfbawgj.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gmkiiyiza.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gnajtmoma.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/guqlgzheu.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gyfxuydrp.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gocuufoiq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/ggloflhsr.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gsumcvpge.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gchovmhty.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gplmmaocq.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gnndmrocc.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gvzryrhmd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gesrkwapk.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gxzwpnsce.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/grixpkocj.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/ggsfvfebx.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gwrnfibjt.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/grgirszsv.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gsmyayhqq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gzdaqglqx.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gtwerogjm.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gpmfqwcwt.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gojclbmxz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/grubkuiln.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gdatnqksd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gpciujdjm.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gkssaroef.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gahzkpfol.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gtqaynuxf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gotyriyez.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/girzimrze.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwniefazr.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gcfeafweo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/genjuwlyl.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gznlfuvhb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gnlkhdqle.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gowvcryzz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqjyoesce.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gcxqoualm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gdqydrbcd.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gawmbmgyg.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gdocbtxmu.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gnmekdnhs.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gqnlgeqfl.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gygumzfjn.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gpkkwygoo.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gmaezaxlo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gnxqfurnn.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/guhwoecnc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gdfgcjvmi.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gmcwbaxns.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gcqxvnaqe.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gilzijath.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gywmrlawi.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/ggnmgxulz.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gnpprvkwa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gzeznfgam.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gevjeffhf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gwojxvgpi.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gafvyslup.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gfaydeqbu.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gyulhrlpo.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gelasszus.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/glgwatnvn.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gsshpneqi.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gaapfhwdh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gerdolpnw.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gotxjmroi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gzvcflyhl.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gdrsqluxw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gsnbeouno.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gyrmglwih.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gelvqwrza.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/getejmupc.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gmuxajjmi.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gtifdkbtt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gwimhgyfk.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gwgblgrav.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gfjjlvdlq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdenhaqzw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gqjvjktva.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gahteupsq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwficscli.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gptzhnohr.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/glhgqohrx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gagclgtyn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/grnbgyzwz.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gegallykb.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gragrkgbr.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gkashbotz.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gfoclsxxj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gttyqsnsb.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/guuuivkoa.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gpuapxnhz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/glnaxlpfd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gglyfagej.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gnjfarjws.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gnuijfpit.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gyzytygwl.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/guackamfo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gontymwfm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gzxnrweuh.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/ghmuqfdon.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gsxjviopn.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gcmmdaipv.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gslfvzqqw.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gsdtanklo.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gxggapjjv.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gftsqrgun.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gjeihnzxj.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/glsrmvobn.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gokqucrjd.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gbarusppe.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gswiijjef.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gatefsman.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gdazflggx.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gyoynhjsk.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gnocdokcd.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/ghxqyahjc.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gucaoxcrr.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gkjlyhucd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/grfjqbwbd.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/giwnwdrmx.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gyhhsecbx.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gfwmnxgbz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gmdcgtpwu.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gbwsiwrvj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gjstjlkfb.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gfqtrwlts.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gmigsntin.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gxfeadwes.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gzxxitroe.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gzvrbkgbn.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/giylqxpnf.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/giuduiowe.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/ghmevqjpg.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gftrbgcxr.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/goclhexxt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/glcvdfsuk.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/ggdtssaot.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gdtwcdxnk.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gmyyhoyyv.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gvzrghokw.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gyspdruan.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gwgawpkox.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gaeetuhmb.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gkupglfqi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/ggyrhlnlx.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gfebkztxw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gtisnuqlt.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gzkwlqwgj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gvsdvavyj.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gemplkhva.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gwsgiyhfx.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/grmtczmyx.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gvvnfkzws.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gcskhpgom.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gmluavzsg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gqnqutxpv.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gvtvzihor.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gbdbkgfkk.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gtmzibrid.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gruktprjc.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gmkvdjvrb.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gmjsjjshg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gvjvsdtni.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gvvmvhasz.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gaoyrsjmh.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gqmrhvhzh.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gvlggcjou.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdsohjdqh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggdigbkir.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gsawtxdyv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gjitryvly.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gtwuabiwt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gueicxpcs.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gqsbbrgwp.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gfyogmppe.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/glwemsnsv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gpjeqyvoi.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gahdnqkpz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gelokoyyo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/glzikzxgb.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gizhxehrq.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gdvjnvpmv.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gynpfkqxk.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gdqrxpjhe.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gdojmrazo.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gggwnccfn.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gmvccpzsf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gulkplrdm.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/goraqgaai.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gevfrpupa.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/ghlxgmjjg.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gdhtfgijn.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gztzsxbsn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjeioffi.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gxmbysxsb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gwuzncnll.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gpywtzpfj.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gnogunpse.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gwuwfoxhq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/goaorvocn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giwyeqsbi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gyhhntihh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goepdidri.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gbqhealrl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gqfwxhceh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gnuermsjh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gzptaqrrv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gtlilwnhk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gsakzkthg.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gjmpspvpa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gxgasevcc.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gzozkipmo.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gdnwgzldr.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gkjjemxox.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/guoncvonf.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gxjpbmcss.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gejdjrkow.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/ghaxtrsti.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gxyigaehq.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gtojnnfqk.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gzdvhuisc.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gucyhfyep.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/grmsqfqbe.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gspynuyhm.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/giokdadlz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwlpiqtkx.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gbvpgbzwg.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/grwnuhiss.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gtdqjarlo.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gugteyvew.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/glmnibaai.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gitvaflzf.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gergemajx.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gyqkdhxjk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gjwlhcjpq.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gjpxgdjro.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gyxtkrmbc.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gugbwwvqj.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/glolwdqek.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gzjhswkoe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gxoyyffuw.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gmwdqbkws.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/gsywojsvh.sHtML


<!-- 参考信息 -->