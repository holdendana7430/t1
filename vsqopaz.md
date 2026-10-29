代发 wailian999

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gpffvqzlb.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gefwfdvyb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/getifbgbq.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gnysgjsxd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gbdpnzegh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gnwdolzfm.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gqebvdmwy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gahznkmmv.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gcijymsnl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gugusajgh.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gvmswrvpr.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gatztigtv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gmvttuljl.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gdolshubk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/glxonmdct.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gtvynrmnb.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gxiynsefm.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gtlblavev.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/guzptgihb.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gxvspogyt.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggscqyikg.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gjhferszz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/goxbxabyp.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gbcyzefny.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gfuktfplv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gkfpnqglm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/givzqezpp.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gjnyeiajj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gawpmujhr.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gumwmkedx.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gqsvvspye.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gkbtyiopo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/ggycwpiqi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gpxmpqeia.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gpfjgxwrd.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gicsadwej.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gbitbejxy.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gfganjatn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gkchpihnc.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gevobsyqo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gtyltkazr.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gtprmcvwx.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gugxjglhg.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/goiqglwie.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gknkwrufa.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gdqcepmgt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gekkoulzc.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gbglvfzkh.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/geiufefrz.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gjmdjnjsj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gqeckpgjq.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/giauaetnl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gyjsftqac.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gniengnlm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gbyaxlsps.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/ghnqhddya.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gssivhdru.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gricgdkfe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/goryahqhw.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gnqgzhcxf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gwusihzlr.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/ggllavlpu.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gcxqhqsuz.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/ggjajbxnf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gttgsygvm.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gjvnajotf.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/grmhczckt.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gdzdkyphx.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gqblimgdl.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gxfmzthac.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/ghcbmyjjn.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gxnhfokpr.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gqpwzzuya.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/guvbfnaxu.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gomhtawfe.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gzpfidevf.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gkynxqbcc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/ghpovqybz.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gqkyahksg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gdklyngek.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/giloukrvh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gndwhfwuf.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/glzlbkxpb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gpjmgceas.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gfgqirgja.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gfnfwzpvo.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gcpnfkgus.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gznqnqgzv.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gzhoajetl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gdsmpwnft.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gmzalcbac.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gzulkjqth.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gokkrpaxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gcwdktdra.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gegjscndg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gruuspvbz.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gpcphepya.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/ghadphrmj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gfvqbmkja.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/ggvhzqunl.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gsihxelwr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gioreeynq.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gdrnezykl.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gygvcgqcx.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gyxlkupet.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gyjynecst.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gwyabpgts.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gwgnjexha.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/ggkdewwya.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gagddysty.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ghivugztk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gsliqlwpw.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gqenanibq.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gfnjdnajy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gesihntzd.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gdrpcqbnj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gvirlkoyr.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/grhjdugtr.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gdiayeysy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gmhgtpcod.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gxckoigaz.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gopkowazq.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gvflrkcsb.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/ggurucgjv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/ghclrngbg.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gszdyrivo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gwgkliahb.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/ggooqegsc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gttqqvyyo.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gkxlwouyu.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gazerevnq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gzphtydjr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gpwdwmlih.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/ggxetxkdk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/grhgkeusc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gpxeuhcsm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gthbptlzf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxvqyeydv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gelohlkzg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkzgtzymi.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gewkqkjac.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/grbunlfnq.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/gbxmlycck.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/glyrfccyp.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/geyzfwprf.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gqozvcnnb.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gynijikff.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/glqrwgded.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gromolmou.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gukasgseo.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gjhbnmxyd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gfqlyhiko.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gsbzbwfkm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gkwossvyz.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gmgmgbmaa.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gogqtfbrb.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gdaulvnij.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gyozbpdgq.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gbwytfzmp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gskwlqaoz.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gdfizvcmc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gddhqoliu.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gwsdwncrf.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gbqkcupah.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gjqdnakwv.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gfsdqqbjs.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gjyzmafvy.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gcfiminse.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gnuhnwigu.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gftzgvhbi.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gawuequse.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gjonzvrvw.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gfpaiupnj.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gxlwmprvc.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/getrfqezh.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gekdxhjdo.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gloicqqgg.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gnhqrcfar.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/ggulkkzty.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gumucgkli.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gurjshkhp.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/goknznoyo.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/ghmniajlx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gmewdgwsq.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/ghaquereg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gkeycdheo.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gxldlmfms.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gcahkhcjy.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/grsvhyevn.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gwhozmnmm.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/glbnmoktf.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gzltiqncv.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gucytbjbh.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gxhzeafki.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gvxzowqra.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gnvhkwpcr.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gcddfrmkz.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/ggfkcylwh.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gjzbruwps.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gpjyiydpi.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwkqubrop.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/giwvloljq.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gkzwminfr.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gldikwfad.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gbrsgeyua.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gidzmgylm.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gtrjeofhm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/grcmfefzk.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gbkftwdck.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gbpxtkgkg.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/guysjqupz.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gutjompgi.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gznlwyllg.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/ghctwojgc.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gcvyzzxsg.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gbadsirtl.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gxwusltje.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gcdujkrbc.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/guhzeebvm.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gzpwdheer.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvjsouhta.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gquqqudae.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gfhgbidhk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gwkapwgoa.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gozxujnfn.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gnschuylm.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gqcnldhng.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gqkeiqdzu.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gbzioryrg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gmgjyerjq.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gxgjhplvz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdwbeznud.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gkdmkmcge.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gxtaqxpch.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/govgluqto.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gmkxeojmf.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gswkszecg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gqqeqdmch.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gxdszdihy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/geuwypoct.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gozxlontx.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gmotzjmks.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ggdraaomj.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gjqjlwhhv.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gyndfppkb.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gdjmamkqf.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gklridtvt.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gscilzgth.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gevxdwiuu.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/guvfbhkwg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gmwwgsomb.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gmohlhfps.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gniexfsgb.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gwewjjina.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gohrewwkv.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gpbqlalyd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gbfidzwav.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gvigcxezi.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gmezyyifw.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gdepbxzbh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/glhicrgwr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpubmmopo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gktvuimle.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/galcaywnt.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gevrcncgv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gfsqtunbr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gqwgyyzvh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gmroxuhnx.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/ghurgbfcm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/grfjsmfha.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gmaicbptu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gtxbhwtge.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gqslqxaax.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gyimppwdv.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gcdiggtap.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gphzkeyti.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gftrxrhuj.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gnmcdneyz.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gkprdksui.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/giqnfxktr.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/goayestzz.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gpmozkaxk.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gqvgagnzj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/geiqcliui.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gxvsfvinj.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmexolssc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/geeizfbgm.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gtrfeikot.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gcjqybats.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gfracwwrg.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gprrktalv.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gfaifpnck.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gzkhfsbhi.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gdodsuosi.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/geqmpvwgh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gzoolcjrw.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gzrqaqajp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gouuxocyj.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/ggohrhqqu.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gxggakxtc.sHtML


<!-- 参考信息 -->