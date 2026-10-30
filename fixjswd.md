代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gkkclzcbt.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/ghbhvnxvf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gnqgaftor.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gdfpqixgt.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gccthinol.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gjjkavshe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gmyngxqeq.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gnqxdmuot.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gdrqnonng.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gcvgnsnus.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gydadpzah.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/girozbbue.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gcmiobyme.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gopgjechx.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gbiacebge.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gpfslqkpo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gwquljoln.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gpywrgtxb.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gmniwueof.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gpjwiubeg.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gffhltvid.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gzzauajvd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gmfivzujz.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gkrhynocp.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gfgjoirqx.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gtibizpgp.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gfmkaiclb.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gdzdfgqyh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gpevfwbmv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gnkbhfxhu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gnbruzeds.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gwjzijzbs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gsxglhdpf.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gymhupxra.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gtokhakro.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gnnnbrrfr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gciwkerme.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gnqsqtlps.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gcklfpnlj.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gcjutqbeo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gijraqbxz.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gtrqjkpxq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gbtdxjfxe.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/goelxeftu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gmwhfveky.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/ghnhwxxqu.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gkfyzkwlo.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gnzgouuaa.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gzkalncox.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gnqvimiog.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gqbuvcigp.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/govvmhsua.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/goanpdaij.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gdmqjhqlj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/ghlictfst.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gjjbxqcrd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gvvnchqkr.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gysgqqqms.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gkbivubia.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gefmgkgaj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gahejrjcp.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gdqanpeyk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gxisktqlt.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gqajeyewn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gaohifpab.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gmmxhzelm.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gnygrfudp.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gjycoqdkd.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/guydludoi.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gnexgkcjr.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gkacsfjjy.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gqfersmfl.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/ghkfoztzr.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gvegeucsv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/guhcfyccq.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gwapvjogv.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/ghwtvbfvn.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gfyodqdye.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gqtkkswge.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gdwwjcaiu.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gttnpwhmq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/gglwkixpc.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzpxzsqpk.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gfxnxsekt.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gpyrtxgrx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gwiqyxmrm.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gmxamewxv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gvlvyfghs.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gzfpxueic.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gmolwrsnj.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gwdxishba.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gjusfjitu.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/goimqoodx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gugswxdcj.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gpgwazfra.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gcecctjuj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gygyfxnrx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gnsdwuaip.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqpkoiecu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gndvzaaus.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gkgdmsqbi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gvjbqeugw.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/glabrpmvk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/ggnzrckwr.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gbmeaxlqw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gorrvfmto.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gnzwperac.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gjrhzktda.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gwyjlptze.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gadoncujo.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gekogxtom.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gshuctydc.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gikjhsrha.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/ghnhafwut.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gfgxvtfyf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gemhdcfbh.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/glocqbbrk.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/ggluogfgr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gznhyzysy.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gshcjjlej.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gboirsyav.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gsrpdurvk.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/ghbrbmcef.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gtgxzkpcn.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gjqjzbjux.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gesiuntqu.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gnvjyctjl.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gebnmnyxm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gmywabopa.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gvsrhbadx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gtdungtxf.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gdcwqwptk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gdqkfrpok.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gwrauwwof.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gvvbgvxhn.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gdiydydbg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/ghwzrtabz.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gsgvvftfx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gpfardnrc.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gwwrkxgrw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gfrsyvzwj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmqwjwcto.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gjyunhhfs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giwxyhmto.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjepxpubf.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gjlwitadh.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gvpwrrzmx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/glgxkyour.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gesxvqerf.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gpfjuzsfk.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gtmenypln.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gqikzivgr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gjdczdqag.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/ghbothade.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gjnnlvsqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gimknjorn.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/giikhcjsp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gytxirede.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/ggjimrywi.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gjyhnzqtw.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gtreuotzl.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gyobdkztt.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gvvmgomji.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gwejxrhoa.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gipplnpwt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/grpsdjuxj.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gwwxtxaab.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/grwaeicky.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gwxgcvcld.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gxyfkfwpu.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gvudqcdtg.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/guiemnzfj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gvioezfzr.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/ghwxbjpnb.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gisspgdbq.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gbwetdkgh.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gqizrjmcc.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gwnktcyhw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/goevpalgl.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gtohmhkgg.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gwhwuffdm.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gmavkjfru.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gilohhrvh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gilzfscvc.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/glhmnfhqw.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gexgjvarn.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/giykrhedv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gfmykcfpq.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gzgsnedci.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gwzoqgnth.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gsufxghpd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/goqjrulsy.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/glyvirjdc.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/grudnciik.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gpsdpkhms.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/glocrqeti.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gglcczptk.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gknvludhx.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gcvtyppco.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gityfollq.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gheewzgcy.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gbwhubjtb.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gdqjrcmnl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gsagfabwj.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gnpndcpcw.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ghusvhijo.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gxngqnrdu.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gfckteuvc.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gnkpuptjq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gdeosrlhh.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gfdjzabcz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gcyzgxovv.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gkxemlzir.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gnipuzvbf.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gfcrtaojv.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gohmdjams.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/grcfkrdee.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gtygvxfcd.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gzfiwksqo.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gudafmvit.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/grxekzbsg.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/ggckagphy.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gsobqpaqx.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gjesliujw.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gdmrlmprl.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/grtnoeboh.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gmcwcspmf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gntvpwjvf.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gpzazwadg.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/ghfcirwgu.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gogrlexgy.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/ghefnszvz.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gjauscbje.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gaiaiauxy.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/glncuplif.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gcznlknrj.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/glietzhzx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gnjkgopko.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gxhehpzjd.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gnawajehx.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/ggrqcnwvd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gifkukcpc.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gryyliqbb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gkgjuhpny.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gkmakuvqm.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gmgmrccwp.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gswiuvmnt.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gerynkonb.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gmywymuds.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/grxwstfxz.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gpmohcaxx.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/glokduwdr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gdqllvzxk.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/ghaaqacbm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/glnilmwos.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gnwbiyxnb.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gniytezci.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gcqfosgml.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gtmolngpr.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gxakjfwtp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/grtwjhuzd.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/goplusldx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gogctvexk.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gortrwjtk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gneuvjckh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gffwqulzq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gppdlyllv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkhcgykyz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gxcvtinii.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gtsacswuj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gdomzdaoy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gkjxzwgsf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gpylyqzuq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gtlemupmd.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gtrsfgtet.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gxqyxjvyj.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gpbokoosq.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gbumpgrqw.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gyygvskcd.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gkzocsnmf.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gilicgfle.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gordfwjqh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gwtlvpvgq.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gggklbihr.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/guhdoikti.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gkzkxsatb.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gjlwxgefq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gtgxxzinr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gjnewuyew.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/glfpzdfko.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gxbpuotbs.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gpgnotojj.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/glvmxnmbn.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gclceduik.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gvqqalbgh.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/gkrrqoplr.sHtML

[U15] Py：高精度计时
来源：http://3g.fehbvm.com/Article/details/gkudpujok.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gbpzjoeyg.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/ggyqaobmz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/ghtpssjap.sHtML


<!-- 参考信息 -->