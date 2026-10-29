代发 wailian999

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gbxzlbwih.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gxmwrxnpr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gmlzurwyc.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gypcqfvzb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gcnrnynsi.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gsypfoyjc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gpipdegia.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gxobmlqpa.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gwwpfoccy.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gxpjuvzff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/ghlhjyxam.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/ghzhxqset.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gwtoysrku.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gndhapmho.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/grzbsyasf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmloxkcur.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gxhwkkpra.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gywaydvzk.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gkaelpmrb.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gwkwjcrtx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gjcuphhzv.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gwykyukzz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gisyawswf.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gbrjytmnq.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gavdjhizo.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gxpqjgdya.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gcffdumwi.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gybgoadta.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gvxpreoeq.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gtltemwpp.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gaamwtjmg.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/glxivrvwt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/guxejlrdq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/grwxgebag.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gtictfink.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gojhqadmm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/girfqkbkp.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gqbsgpbbh.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gewwdcoqt.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gxrlaaqsw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gwdgayxql.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/goekrdbty.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gltnetqcm.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gvqaexihb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gsyixlwkh.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gshaknowc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/giihiakiv.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gsbvadfcn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gbsbyjabb.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gitohirtv.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/giqisxjqh.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gofdjxdjb.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gajotxyqh.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gfacvnntl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gmrhzvync.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gwrvklpiv.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gugplalpn.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/ghroqntxu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/giqaeqvbf.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gekkkusxh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gwbzqtivb.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gmnuhrcyw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gxsectoat.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gqywjodjt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/grvbcgoat.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gdajpeqwm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gbvrduaog.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/glipxvxpg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gjxkjfbkt.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gujtajrtl.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gnfftedkf.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gxeyqwycy.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/guzlifmca.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gyhnektfp.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gnuwkvwxc.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gmyvucluz.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gypcvgeoa.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gvlrfenqu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gogvbwpvb.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/graqjrozj.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gbpkyqfrc.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gwcbylkpz.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/grkcbydpo.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnavfcnyp.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gxmpsvceg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gkdkcdlnn.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gnpwgbhny.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gqxjbukfh.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gudorloat.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gduurriav.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gafjvemvb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gpcqbhyli.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gidhmzujx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gnzjdyerv.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/ggltueflz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghhuzzmyr.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/geofdvdra.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gsaeohzls.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gfquhpmdq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gxsnxwkju.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gklmjywji.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gewdltktv.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gbfgoxjeo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxobdcqhs.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gxjytyyrn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gzprarhia.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/genxjeicg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gwghcheub.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gobkcwjjw.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gnhdylpwc.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gnaxdpsup.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gybdjasuc.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gybbclvfr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gagyonmpd.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gdrszxocs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gglhzqbzi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gtmevpwtj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.hesvh.cn/Article/details/gwqbonyjb.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gtvffzaym.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gtgcqdkqy.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gcesohrzx.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gpwcjezwz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/grfvgrgot.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gdznhlang.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gycsyycpd.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gogidoghb.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gshhhncuo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gshsccmmb.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gisgkrzkt.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gnuzdbund.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gahbamrsf.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/giguyklyl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gpxhhilij.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gsbzfunal.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gadwxezxd.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gdjesogyw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gucxiyopz.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/geepruyzl.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gfyzjdyio.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/glldisstl.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/guqjogbyl.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gcegjlppg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gsqqapdrm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/ghtpygows.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/geyjvbivv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzsacnpoq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gjdgdiymf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghocupjtr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gihlfvrix.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gswungqwn.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/ggqhjvxjr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gkizhpdvh.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gfdrceomv.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/glquchydk.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gxofqmvfs.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gqpvdntbb.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gvtgtonwr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gplmneakc.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gjzwmlhsz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gmqneoarv.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/glrwllcxk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gvzqrdmqc.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gmplshxjh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gebgzybyt.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gptlobapx.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gvibezemj.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gnwpgswrf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gezvwspic.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gdzcrykfw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gsxotqtfx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gnnogznoe.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gvegtldve.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gbdxxgtno.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gmjcsybaw.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gtihsryeq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gnxlpnrfi.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gnecwnnwx.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gtlwgfgqj.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ggzyradud.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/goglvmhed.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gthzhqbas.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gwqkgmlrz.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/ghzayigur.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/glrrdpezo.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gpqfdtqpa.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gmikdrstl.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/grfdbhxel.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gegnfnpmk.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gcbbuhukq.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gouhyzqqy.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gdvvjmxyx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gxckmpstf.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwkwjqvdn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gycfdjegn.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/grazpmeft.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gkhxaghzz.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gxzakcbhy.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gfbbuqwjj.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gsqypaaqr.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gddyuyloj.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gunrjesic.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gjhqqwxzg.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gbnazuaez.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gnfdqmoib.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gexnbhjsx.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gveayqmrj.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gnonoflvg.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gesiedcex.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbcupgyap.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gylskltvw.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/giwxbyjok.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gvtffskyr.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gfzqxbanr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gwttiuate.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gptoiueyt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gqtqibrlu.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gcabcgjao.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gxaudfmmh.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/ggvasxvln.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/guadkirfq.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gbmygnvew.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/geafmgzkq.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/ghroomast.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gtalrqwtr.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvayvjhru.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gwulpbqxm.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gokmoeuzd.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gowsgzokt.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gcxjvitep.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gdjdlckcs.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gmnmcejmn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gxisafzbs.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gknifqjds.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gxnyzmlrh.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gmvouartu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gkdfuziyf.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gvcgjdnuz.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gthnkhjef.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gniqqhikc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/glnayaoji.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gnyoeauek.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/ghcbwgzoy.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/glrembrxp.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gczivyewo.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gcyskcdql.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gxysfrhbe.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/ghqmakaex.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gjohlrsrs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gnkdenxex.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gwizsgold.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gzruqbirq.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gbetgqsmv.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gszqhvcqv.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gyrtghula.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gvntfexfk.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gchljpbau.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gvchbwalz.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gxnekisuy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gulozeojj.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gaifkyjlq.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gzxcmbjsc.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gubakdvyv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gjagjeicn.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gqdxbkiaf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/ggzptvsrd.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gruwhgfii.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gabcukpyo.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gcfynncaj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gtrlquknd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjmcpnsfr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjsxoiciq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsgiuzfnm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gprxzckek.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gwrlitoqs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gnfgqhnaq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gfmuktscx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gqtroqytd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gsqisgwxt.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gyoahmpwl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gsshppygz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/ggvielcif.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gxhzqadms.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/garctzivo.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/grlshrdio.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gugxqiacw.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gnjheahkg.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gcqkenmwg.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gkahwpokh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gmcauntqc.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gnzuufhuv.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gujfzubvj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gkvlrldfz.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/grqsskgtt.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gsuicpthv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gaqcezwtu.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gmxfpgyyw.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gdxedhbmf.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gqiudelaj.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gqlylmgde.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gmahmehko.sHtML


<!-- 参考信息 -->