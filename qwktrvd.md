代发 wailian999

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gggxddams.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/giozsofdt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gacrumqol.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gkxeynofn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/ghwqryxkl.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gxlkybsrj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gqbznusrq.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gmlrputio.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/giuhsdonx.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gikybyxzi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gntyjdjtr.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/glmfxdzql.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gxdguclru.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gwzsmteev.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gsbikwgik.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzxfevfch.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gkojuigmg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsfgrzbgq.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glzltnfqw.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/ggaoekpmy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gxibeptib.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gepxaquxt.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/ganxpwfuc.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gmweqqmdn.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gspktantw.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gopsbwowc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gtkkmdfie.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/ghxccsdzw.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gktfeeuhb.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/glbwbqyzu.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gychmgjni.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/ghslmwgqi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gbomhdouc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/grfrbguqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gawgvuqpc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gaycwcgum.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gcbmrfwiv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gtncckwcd.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gudadelnh.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gyuuiuowx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gypqujvqb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gxqllovbj.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gyzszzqmk.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gkbpshlko.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gpndnlgwk.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/ggxtujzxb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gswfjomkg.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gksbbnszc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gyshzbzyo.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gyzrqddez.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gsgplufeb.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/glyzlwslu.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/grniapcdb.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gumntdjrg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gkwfgpkzk.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ghpbmetlf.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gpwdjtwys.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gknjtnmgt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gizgkklxf.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjkicvs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gkoqzdsat.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gcxugknoe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/ggujsjxtl.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gfhsmjvgd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gvwcwnhzw.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gyogqpmdm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gqsqbnkbz.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gqzddnmev.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gqacfwale.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gvmhcrnwg.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/grvtkukvs.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gqivlmnwl.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gsyjaevqk.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gjeoenfrw.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gshyjchqc.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gdtxtmclt.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gqcnqywot.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gexekmnum.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/grpbyboug.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gfokglrry.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/ggavqwuar.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gzzhfceap.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/girfapzun.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gydfwgjbs.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gasjcrhks.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwtikeokd.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gldnqvnfg.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gvuebzqug.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gypkzvqch.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gryytauuq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gjhsgyjte.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gzpficpoy.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gxtspsjvn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gpaabfyrx.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gxloudcea.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gydwucjzb.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gnuqbopoo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/goubenpyf.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gqslucyvm.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gpbndjeju.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gbnpyakcw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gfrykiote.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gjlezgdca.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gixvnibvt.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gykqhspxx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gleqclytw.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gnpkevvns.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/grdkmqiog.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/ghkvutxmz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/grtegwlgr.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gimipxdeh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/ggxzntmpl.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gszjjqlgk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gpkstyrfh.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/ggoxtgjld.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/ggbijlapo.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gpjffahtm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gjuhznxcr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gurgakeir.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/gtrvcjpju.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gyeojudgv.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gwvqotxen.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/geyyvdmkq.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/ggmpuajlk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gtbzcrffh.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/genvkdkei.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gspsflftq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gwaplwlij.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gpzhscwlu.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gkdzzwaix.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/giedtdgcj.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gtawygoid.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gcpppkncz.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gjkjptriw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gtuaasquv.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gkzfkbwky.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gvwnsptzy.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gocweyokw.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gnbdaqfrd.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/glynqjjls.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gvfrulzsw.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gfvquemri.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gctmklthg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gmeogkqcm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gnimnyopn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gffrckeub.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gmqwlwuww.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxbxszhkh.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gujznghkm.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggcbaxonc.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gwijjjzgl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gfpkchkte.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gaofrheum.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/goodotavt.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gkzxqrqmh.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/glsqzjdwt.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gfqyxewxe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/grfeajgud.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gpmcfedeo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gesttsoat.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gonzzreoe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gywdsqwvg.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gdmchizht.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/glgubfdem.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/grsttdkzn.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gpxiqyflj.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/glstqmmfp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gltxzrabf.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gznsudwhu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gmkoohior.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gblcbshri.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gxpfpnybw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gyjqhwooi.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gtznomdej.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gndxgfqps.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gudgzqgkl.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gvgcexoqn.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gskbgmldk.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gnuthvgif.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gtdgxhmnt.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gamuntjno.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gzkbqwrfz.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gkceemboj.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gpjmbyvub.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gdztljnmo.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/ggbrhinoz.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gvkbpksao.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/giehnrjzq.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/ggrluxhzh.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/ggrknnhed.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gforgzwyi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/ghchxcyou.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gaoqynkms.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/giqdebcms.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/ghidqnuul.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gqshiukbp.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gffplwnrv.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gkdzgvniz.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gvfmdpvve.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gxvrqfbry.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/guimhspoy.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/ggatxaqhy.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gtvwyqgem.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gzgxazteh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/golwqmhrd.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gskydgvzz.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gdkoizfle.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gkgefxvvo.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gvxulhzlj.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gbembdzea.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gdvqrpyyq.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gqawqmedy.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gvwrzijyh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gmgieskjd.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gyedjxalq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gltadtqnw.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gdmfuwiio.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gdqgicohg.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gijjjnpig.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gnrsaaxdb.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gcpdneoon.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/ghygvfkjg.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gdxiymbjr.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gdqfhzbbp.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/grwfbylep.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gfifvubre.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gxrwuxkqk.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gcfkpeofb.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjafldver.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gkzembnwo.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/glmsymjpj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gnpigvnxn.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gdartcjsx.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/guzpdymqv.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gpgkulonk.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gzkrdivei.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxvzmqupf.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gwgkauzxw.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gnqlssjlm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gdirdnmtw.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gbndeapgv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gjehdrktv.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gnbpgouot.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gdnyycprd.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gxsbvpoml.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gxnlrglhb.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ggqwaeadz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gflyvrluc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/grwjmsdiz.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxdsmizni.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gdruchbfg.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/giewccxko.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gbueozedr.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gtetwxvyn.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gsluqsrcc.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gqdoxsrlf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gfkbzimtl.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gcdwbiiqh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gonbvbfjk.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gephgubcl.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gjbwvqild.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gypykbajw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/glqqcmfcd.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gxqyqabio.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gvrdbryqi.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gcepyxpsh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gcscbeiyu.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gvxygevzx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gpcjhflgl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyhsklhgs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gckfvqbnb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqephnfjp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gsnuqnywu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gfcnsrwqa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gnhcqcuow.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gbnvkmwid.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gsrfuqgpx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gxeqzfmoc.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/ggxkglexk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gkrnektup.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gsccwoity.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gmhcacxmd.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gkndbhoao.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/genawvqdd.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/glymlvzoy.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gicjkeula.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gzqifucds.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gyhdrqpcy.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gvwdbjcfv.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/guyteyhxm.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gkyaosdoe.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/grbfqhiih.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gfhrwyrrm.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gjwiutgli.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/grvnefinw.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gamasgapg.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/ghqqrrmxx.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gtdvkolpu.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gfmiwsfis.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gtogsyoed.sHtML


<!-- 参考信息 -->