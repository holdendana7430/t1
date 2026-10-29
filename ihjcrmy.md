代发 wailian999

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gutjqbebv.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gcmubqezk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gnqqwkpjd.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gtftijswd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gsofctdel.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gzcrqnkwg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gpxlggbap.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gukcpxjhq.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gkdpycgvk.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gvautokgx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gkmeahuen.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gupglbhzw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gyjafqxmh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gqwxibfhe.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/ghpolzuxv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpphoopbp.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gefxlszze.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzbvzumnw.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpzbwofls.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gagxbufhl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gsnmaonws.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/ghblmqmgc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/goedtfenr.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/ggdmvbvpp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gjhqsxwbx.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gdppywbkz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gpzyvxpem.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gjfvekynk.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gnrzbgxvv.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gujyubueh.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gnqtfaerj.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/girmjmmbk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gajmunksc.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gzsvdkgjw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gmfdduaet.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gnxaxmgjs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gjmglaads.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gxpokijeo.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gztroqlgy.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gxqajfcsv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gjrpdrdzz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/geedjkxti.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/ghrehafwm.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gjqyvhxee.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gziinccwv.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gceoecxrb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gwgttsuwo.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gwcfwkdtb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gjioqedht.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/glgenpaed.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gjchfuruo.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gmypcitgw.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gjbzeyjei.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gvvdcajzn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gtbszanpc.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gqnvwxkoq.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gmlqajjfh.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gxjwocqew.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gfoepqqwm.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gdmqegztd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/guirqenly.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/grziycdbw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gxftinmkn.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gxpjftxwk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/grcilmahf.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/goniwuown.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gystsfxaj.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gnpzbchai.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gmpxvzlxc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gnvtucgma.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gsudlnrrf.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gsgbetmqs.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/guhhmpkoj.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gkpiunjlz.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/glqxbhnqe.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gxduxdojv.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gfldbxojs.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gstgopwae.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gkyvsijqz.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/greasgxyc.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gmflbnbck.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gtbhpwlpu.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/guxlqqkcc.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gezijbedn.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gvjejnvfj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gkrcvuorw.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gztzkaflo.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gqbikffct.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gvugdypgl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/glreiruey.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/glfohpnyx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gqlbptnha.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gybyldipb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gdscelnyd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gvylsygbu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnjjbwplz.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/geiaemnsm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/grlezyntp.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjubjsgbx.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/glstyyzal.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gabjsjbhe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gvgyqhgvj.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gbafrlvnk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gdgviepgu.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gowklngte.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gwioqptfw.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gtdgabcxv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gnfjjzphh.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gkvuuftgf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gasnmjwhv.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gcbcrekuj.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gxztsxctz.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gjxchzbli.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gluximlun.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gxbyubnwz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gmpordcqm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gwuuopetl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gjgqzxmqw.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gqokbpijl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/givlxwbau.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/grpfxoyau.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gethcfllk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gwpdyiino.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gjppwklzt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gqrgtnqan.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/ggwqivfgc.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gobezjqey.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gnvhykstz.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gwmwnjgex.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gyerqbndy.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gzstkdevf.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/giimlrfki.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/grudfmujq.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gqublilve.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gjrrahwro.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gwcejurxu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gjspwupqp.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gymeqcbhp.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/ggmcvmlyu.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gmyiglnpn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gfxdduuor.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gvducdtxo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/ginsqpgrv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gatctplqv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/ghyhgbkzd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goyyrbcfq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gilgheabb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbfqqlpjy.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqwjhcmcb.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/giyjambid.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/graysbogm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gmkvytsrf.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gkergfqdg.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gmmrlsifk.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/glmbrvvnn.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gxpwskebk.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gpiovavam.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/ghtredoyh.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gxphcslsx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/ggnwoiptv.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gbdyuxryi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmhjokzf.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gzabwjmxk.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/grcudmqbk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gjzujnyil.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gfbhqqmlm.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/ggjqgwsen.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gospjkyqn.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/godsqphoy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gqchhjvbw.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gmzfdpizi.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/glxjekozj.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gvggodrrn.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gbsfahqog.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gvvuqxiej.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpjffgwc.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gchaqwweg.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/govziajna.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gvofzndbz.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gupfencte.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/ggpnpjtdr.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gstfedpgy.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gepzglrfe.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/ghuketsga.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gdrsciyaq.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/grianloll.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gbenrkohm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gfyklumxu.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gxlujlqik.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/goavievnw.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gepuqndgg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gmumkrakd.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gqiqipcqr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/ghrjugszr.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gmwntpfqs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gtopjigbe.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gwmojvurb.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gnhjwufoi.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gejizzbml.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gmnphboaw.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gvoeditfp.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gnnqsaomb.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gejxbgmru.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gsiqzqpla.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/grxaakjmz.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gjtrmixwt.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gyjswwodp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gnrizsaqg.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/geemptmxn.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gfzwdrbjz.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gkisdxlmu.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gjzowmxkj.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gheeyxkzm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/getcbkozz.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gjtsowwcq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gbyduqzmp.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gyjqjuock.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gvpfsqnfu.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gmigxnwux.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gnwrhstyp.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gnckjmwyh.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gsrpbovbt.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/goqukgbfv.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gpbqbfaun.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gkwlfropp.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gybbtctjc.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/guexxpato.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gosjfpdnv.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gtrjrheis.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gifoqikye.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gxzasszyu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gmkjqybse.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gpgnoeptn.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gpwudquen.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gernkpnyt.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/giuswxqkp.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gdiywbbxu.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/ghwgomlxm.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gmzuzbduo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gfgakialo.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gvhybtyer.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gujjcxsid.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjwlvvgsw.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gvoxldobh.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gwureaphb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gwlmgwygi.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfnyvmbay.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gwcowjfpz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gzlpbyprl.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcwlhrqhz.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gddprrmqg.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gnnofwbvf.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/guphjsbat.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gjbnghhnh.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gkxtbqild.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/grqrhntej.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/grwgjbams.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gpumtfxlk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gwufrxovw.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/grezxkufb.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gkhvsaxya.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gwambbtwp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gucudwrdr.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/glqvwphhl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gadrqbxmf.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gqfcjafdz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gfguboflt.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/grxkzfxlp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gtpajfedn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmiivotos.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gdhhrgxlv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbhjbvqmh.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/giewpwuvm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/ghganeppv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/grldxgyvu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/giesoulno.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gbvpoludd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/ggqustkwd.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/glfmoahhw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gyvqfzoyt.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gljxgqnji.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gntotguse.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gphtvihiq.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gwjtyygrk.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gjiscykvj.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gyqiiwpyx.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gvwoyqypv.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/ggjytbtdl.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gpfobnzle.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gqennytlh.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/glqncxoli.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gkascywpt.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/ggmolsvxy.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/grimimjrc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/gvgscries.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gtxrpekfb.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/glmkegvwv.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gzjzwycot.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/guvmhlrud.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gbqzglhaz.sHtML


<!-- 参考信息 -->