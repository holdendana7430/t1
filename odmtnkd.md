代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwbixjri.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gyzodnoqo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvicxzop.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gxysilzie.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/godgrcnlb.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gtbaioxqq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvbqjqxml.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcbkvzhd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/geoekikoc.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdxcsqunm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gwlrkkhuu.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gigmfzcby.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaebxrqg.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzyegsnp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpseciwvd.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gnhskxzwj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfyyylmt.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gtyoopsvq.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmkfzncd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxibofjz.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gukwdlnii.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsgawiob.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gfvukbtdh.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzamsayro.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmctfdtmg.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxgbsenij.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gkrwtbwcr.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gblxhorfw.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxnormfq.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxfkdmjz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfchzmajv.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebndrdrl.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtyhojfx.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpblmwmt.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gqagrgcbb.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/grxewqexj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmtaodjr.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gyenbwjfp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnrahagd.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gcaqsggwz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfizeypi.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvojcpkqs.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzcydvab.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggzwnmzsb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfglpaav.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/glewzebek.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gfewqpbhw.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkdakltw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdchwdpd.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggprezitj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/glcutjspl.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gedrjqpuj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/glkdylfvg.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghhrrerqi.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdoztbzx.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/ghdwfbexh.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfojmofhp.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrovkbnb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gahocdoxc.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gkhpyxtco.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgbxbsvn.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gekgbwjcu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gfemahwrj.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gyztnxciz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmfjrwll.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gwyzswfpd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmyrmiql.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpqrlniz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/grerbnfbq.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgrjxhoz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/guxdyxusw.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggznhvyai.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudaiseaj.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdpulkoh.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gzoqfgwbo.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldcdczqq.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxvgpntv.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzocrxzan.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gyvksjgio.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gluzbctts.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gltrofdnv.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gezzhybma.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gksfcofgy.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/guyaptttt.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gsgymefgz.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuhwspqw.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gngvdtsry.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/giawfhmbf.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvcqketu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/galkjnyst.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gqfzlxbfj.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gjxujqwzx.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjluphkn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghumvdmna.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/glamekctn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlowsbee.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gltxlknuh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmswkufcu.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvauinwl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjrmtywa.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/grdexcnpu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/glivxxtgb.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/ghkkznoob.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gfqsksdcy.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxctmxfqa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyfajxef.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gotwlwrxc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiigkvgx.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gausksish.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/ghtzvtifq.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlcwtlge.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsjhfxjf.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gqiwhquiy.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gpsboovcx.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gkcimwizi.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxjxfsjxu.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/grpottevy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfhnniey.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gbnkwajzi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcneyikbi.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gllmnqwdp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbvjuoqb.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaadnhsv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxkjocpl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/grgrkxyer.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grogwimuj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmiifpry.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gofkeoqgh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpuokdwb.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyssdvkmy.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtudcpme.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoynjzhc.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkzwgyip.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyrltdxr.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrxznvvi.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/ggztrixrr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gepmtwolv.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gwudxzowt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsetlzsjt.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gawwwuxmm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gevcpsrym.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrllpfnf.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gacblfnrf.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gruehxxmo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuhogmlm.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gxwckuhke.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsddhjvi.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzyfwaad.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gyudnbzyu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gknyuynny.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gtaahdnae.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzzjxfds.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gioxgnyeo.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbeyoujm.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gslvspzdw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggossdqyn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gkffobras.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzmwdcjl.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvytzwsc.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gvdalphyf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyejwhlmw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/goxkwvbvk.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gujeifvxb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/griyjrjsr.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gblktgfgo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeimfywx.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gcvcwrzjv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gskmjnast.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdsqowvke.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtnkvtns.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghlwaxjrk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozxhbgwp.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gsqfjiaok.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gwnsblbpu.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqhzffzn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/grbwkkzvm.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeyxvheo.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/giplrqzhx.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gfenemrlq.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gizzwpcxs.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjrrxctg.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gquiymots.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gahhtzbgc.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gasvwhokc.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gpevkepgc.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/goonzlsyq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmaswdjy.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gksnvsdbq.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gbrpcmwkp.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/geifrnaan.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkldfxeg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcrbpjsb.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ghsrflcdi.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gyvvdyaxi.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcrxhyph.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gbgvgrwpo.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gicktbhzf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gxeanzsju.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnsmswqm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gcwmpwysp.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gzifpekzd.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjyygdej.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gbasxpwzb.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsstssvqi.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkejvxjn.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gdvyvzzuq.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvfhwlsr.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gnvsooecj.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/grkefaocf.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/glnoyexhn.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gmertquip.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gliayeffp.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gnokygiio.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyavuoal.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwmhacdb.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwinpbxfz.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/graxnnywh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gfevloxig.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvrfyjcv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/grlidppaz.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmetbfxb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gyfezlwvk.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjfejusje.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/glygjvuxt.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgilwzii.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslqrqfqp.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwegjfcw.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuyhqcee.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gklluoqdd.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gskqnhxbp.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotuqpfms.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvsbbrzj.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvbpgctjy.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqgnsrcj.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/grnottqga.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gdvoifpep.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtwkiiah.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdajkfxyj.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjugfozoq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuqlwncy.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gyobzomqe.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnwkmqqku.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/glcybbjuw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpqowrsr.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabmoogge.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqtwsbfl.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gacnweutk.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrpqnqll.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkqqjhtd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gchocuhdq.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknjewfto.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gutjpcddl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gflvwwlqd.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhgvvker.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gygiunzoo.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyiphahhc.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gwlifkush.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfqppyjc.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/ggpcjqsrg.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvykougi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxhqaixcr.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmtluuxw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghrutqfrl.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gdueuroib.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkdpwuyq.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyyrisrt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvluzmfi.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwnvwbpv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gffaydkce.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyddlnzq.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gjigbajox.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gapuaxfyl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmtwwurg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guiptpgkc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdkasgbt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbzapuig.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gtvnmpyrw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/ginuklypd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkvpnwts.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvyuamhd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvrerwgi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfymmtvb.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gruijncxg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gsnnpakfm.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/govjzlxdz.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlkkfgjb.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojmpiiza.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gwpkfsqze.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvybmswz.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gihnpgljw.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/goojeqify.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/geyairbkh.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnrjsvja.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gohbxfphm.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gbktjrwtn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/guqtufuwx.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/glisfftwo.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gsemnijdu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvxjgtwu.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwtsimqr.sHtML


<!-- 参考信息 -->