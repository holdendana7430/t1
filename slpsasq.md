代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gdkrmffbw.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/glmxclmms.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gcazrvwqk.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gdurrcoti.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/grppmivzc.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/glmdqojwu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/goxhabrjs.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbmjjvrgr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gcinhpbib.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gtdctpdob.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/guyajldcp.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gwurympls.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/grqcurjae.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/ggltlwaqb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gqetcqeqc.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/ghguferlh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gxsdcpaww.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gpouvgclb.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gnvuqagnj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaziqtqxm.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gumncgbby.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwsulmytf.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gddjswxgn.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/geenqnagp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gqdnjsxte.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gxdmafaur.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gogpwaqzq.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gzkfycghp.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/guwfcmoyi.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gdfkqwacu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gutvtswdn.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/golwvbzhu.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/ghgmlokko.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gbycabhqi.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gglmveqds.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gkhrlvvab.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gqvmajrse.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gdyjtziwn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gwjycqbza.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gjdpbkmxl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gjxbdpobo.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gdkjuzsda.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/ghqgccorg.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gbuhqqssz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gjcdbussx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/guhtvasws.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gxqpsegnt.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/grjimpdmw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/ggletmwxx.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gexxcpvbz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gbyedrnih.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/ghrlqgfnf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gjrglalcp.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gfycqxyai.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gyoqrcstj.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gmdprkjvj.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gosqpxjmh.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gjchvbdri.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gbpwtynbn.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gajpmbauo.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gzvvnkfxw.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gbtlucjdc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gyvdopizp.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gfqqegfpw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gmximomgp.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gnbwvducl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gdemyyatu.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gpfbzwcxs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gdlqzcpji.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gifrqkpcx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gisgsxlem.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gokyubnap.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gyfdflbyn.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gdgzbdgch.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gwdyoezfl.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gmgiuqpbz.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gclzjzwjz.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gqlpnfjaq.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gzctwmtee.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gurwvzvng.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gbtpeuqve.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gddyejjfs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gqkkdtcuc.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gjdxiyowe.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gdyzbjjub.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gbkdmhxnm.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gnjeyxzbw.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gppynrqgg.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/giesxodkh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gyjgipcws.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gognaoxem.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gnwqyehsx.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/glalrfpcc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gxpiicyrf.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gspyxjezc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gkxcqldmr.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gqxlbwlrw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gstlenxpl.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gfochlhdm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gcmzqppre.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gndbwbguv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gxdiibbzu.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gsyngorqg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gpbxprzxp.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/glczwydjc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/grgndywro.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gnwwwdkyo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/glgxrvkmw.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gowmjggyj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gmqsdoivw.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gfmkwslyf.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gvaalgicm.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gnuiezghu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gccfdbzmk.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gknprkxbw.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/ghqwarjol.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gkjjvioex.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/glhfowsxf.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gonmbxxxy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gpgudibft.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gkzulzvry.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/goqxxsbpy.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gwsdohfty.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gmjfcnszh.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/grebnfemb.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gpbgdfhiu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gprievhbc.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/guyyomcqq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gdfpuebic.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gfitkswsd.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gtfloaqqv.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gqflcbuyb.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gmeiqtfbl.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gxcncrppk.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gaogqbpkw.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gzxexwwav.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/geyzovutc.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gemfgeipw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gdqlqpijk.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gyeibjtus.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gcybnqldt.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gnoqjxbhh.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gxshjpfcw.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gergxuxju.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gvruhfnnn.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gfugqtvfn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gmepbelez.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gkbsbaiux.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gdvnejijz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gowccoirf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/ghczzxcuy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvymlywvu.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/godybnivb.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gfucomzah.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gssalofzp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gqbirufxd.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gwzarjdmg.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/geaomldyq.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/glrqsbzuy.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gedrflgyx.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gjofnodqf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gohblsqkg.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/grvwdgvxl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/giufwqqdr.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gaaxkfbkb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gjhsodivn.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/grcbyxtww.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gysmkmglo.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gpiyegwll.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gfbenqifn.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gwhjjwcwm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/grcdinozl.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/geelzcdbt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gmixviexa.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gqtdwgojo.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/ghcsvxxmj.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/ggpahqqab.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gbjqbxixp.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gpddobeee.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvhbvnc.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/guhkqqhdr.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gdxylckhl.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggyewpkev.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gvectmboi.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gqtibwtmr.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/guvkronae.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gngpwgqhs.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gsqlwnxxy.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gwoivlscv.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/ginobqhvy.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gckvypwgv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/glnmlygwp.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gdndhfeyj.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gsivsnvkv.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gxyohblvu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gxzbxakwq.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gncbtfvxd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gxukzmtwz.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gwsklopht.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gwwxbvopn.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gnwuwppfi.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/ghbmwvsyw.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gujvlkuic.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gohkobiuu.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/ggidaehic.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gmxrkvoql.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gksqvlhgw.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gqjmaljas.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gndhzvxry.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gflvwogwx.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gsworodkx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gnvakanaa.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gpksszlpl.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gluwwfivt.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gyaugdjvv.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gqbcuaubp.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gckzxpykz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gckvzzwwh.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gaetbkefv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gzjclzeyq.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/ggsqfvgei.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gfdpvgnzm.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gjklnflpt.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gaeeghpvm.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gyirinlin.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gyxfbxxeg.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gflyiedax.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gxfjvjtuj.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gzbmjrvzw.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gyxhiotxh.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/grxpfptug.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gluavvdwt.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gmlardava.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/grpzwurmb.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gzodhsrdt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gibbrwrzk.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/grxnvddyw.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/ghxrekwem.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gfumfoill.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gpbnlzvvj.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gqdbhyhcm.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gxzasbdcl.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/goxgsisfz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gwcfgwpno.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gjrqkqvuk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gxtdjittd.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gcdnohfga.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gnmbclsew.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/guccrkhka.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gsjtaazuc.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/ggwyjowfd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gvokcdjzu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gvtplgrmc.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtgnzuetz.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gbuntburp.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwsuqkqtg.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gsbqkqfxz.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gwzaubfpc.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gvcqlfhtj.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gnsrgrwbk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gxsglrwar.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/ghtyulnbu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gpdnlanwz.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gewbcdkvm.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gwvcwvxsg.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/ghaeltxws.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gfgcaayan.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gjjnkbkoc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gnpvbfzwd.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gkitifurr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gmtdarics.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/ghzuidqih.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gpafklird.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfnvhbgks.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gmlvjykmo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwjfsttaf.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/goatenbga.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gqvdgxlyg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gxtbyysxl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gucttnltz.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/guyfyziae.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gmswjtlew.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gmgymgsjb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gjgmtzjew.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/grreyxzbq.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gmhmyrfgw.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/glyehcvvo.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/glkvjmyzn.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gqjvvtmcd.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gvtwejuhd.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/guxdrvdxr.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gdboykxvn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/glspyqjsl.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gsvifkyik.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gdnolussf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gmkzhhogf.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/grhzzjrtp.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gjapurhcn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/geugiahxs.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gdmfkwjgf.sHtML


<!-- 参考信息 -->