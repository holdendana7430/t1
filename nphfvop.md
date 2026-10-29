代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gslfixypc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gilxsbomp.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gowxafcun.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gqnnpcgtd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gihsbpigy.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/glxsxwujb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gsuedemhd.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gnjpvvfuu.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gknqhsdfv.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gmagfikyn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvuqsuiuc.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gelsgesyb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gclibnghi.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gdrnjhlvd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gjyghxutp.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/ghfytjefa.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gpuyyibjp.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gvjimlsqe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gaikamohu.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gdnwmrwnk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/ghakmqohz.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/glamygwdo.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/grrpxtnlk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqyimzyni.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/grcmpgwxa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvwscnocy.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxwrrftun.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gfgepqcid.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/grunwdfne.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/geovrtiwy.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gymjiplrp.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gvfqytapj.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gnkokpcia.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gxmyfobri.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gcjtcummb.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gzblzizsk.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gekhfezcy.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gqaqrtysd.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gkyqvzldn.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/glzngtxta.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gzncrnvgl.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gjjetalzp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gptvbmnut.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gyryfnwkp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gbgnrsapc.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/grdmqqces.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/glbwlkxkk.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gkfxilinf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gjoatpgms.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxlcqxsw.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/grmrrxwwi.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/ghnatypho.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gqndwtzka.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gposlossd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gpegrnzct.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gkzygfnpb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gsxibpfci.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gvxnbjrlt.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gwkfsjibo.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gyvbjffin.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gslbrxtmr.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gsfzagckz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gjoabswvw.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gaapqrrpq.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gldkzzvbl.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gremfefqz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gxtkwdxdl.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gewulueye.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ggzwdghox.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gzmjhehar.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gthflcbls.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gjixrbhwh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gjtakxfqt.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gagbyekwu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gafplhgaa.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gqwuxkcmx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/ggnusoqcj.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gahpxwrsz.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/ghauraifc.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gljqbfaqm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gofxaxrek.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gbbtgarxw.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gaikkygil.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gpnuktigg.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gwovrcimp.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gdljpflaf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gcenyjtxn.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gdtmnrcmx.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gucoodpqd.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/ggvsxmmlb.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gqtiacoje.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ghpbzuiwm.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gvbugocct.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gqapkxtrd.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gdgytopsr.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gndhbdgnf.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gzcibgvgb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gwsupaupn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gjbbkbbzs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gtkqfgrcz.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gekyjoaql.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gniexnjbk.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gdzeohhhc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gfalvmzmf.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gzoledkkd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gbklyqmsc.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gxjuqjcni.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gakbtoiit.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gnydsxrld.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gqjfdhbmc.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/goohfytcd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gkfnjljly.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gtewswwyf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gjinduwis.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gqarundqt.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gazmwsmpo.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gpmhflgsr.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gfpjnqogx.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gpqakjjcl.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/guzanfntu.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gzlwntens.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gotewvehs.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gdmnodssl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/goqzzvtwb.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/ghtejxkok.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gchcenbfe.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/guqexitye.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/goayaiard.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gtzwivehr.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/geoxizvdr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gedpjxzcd.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gdtmhyseo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/guehabwbi.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gfszjwyrn.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/glownrhfr.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/glubngnbr.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gkymlpiqt.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gsasvlyxj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gxseduury.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gpgzeqbaj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gbqvfnbwl.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/grscfxxbf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gymnpptds.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gbbcrqbzb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/grjbvrthy.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gkztcglci.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gvzypzssy.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/ghtvxufni.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gexsjdlyv.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/geskkiepy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gxqakqsjl.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gqjwstpnn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/goragneqw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxkhnwlvj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gmtrkgfiv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxmcrbjbh.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glqxkcvyc.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ggmedsten.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gqmbjtqqx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gadjkptpc.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gijkpunxb.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/girsrpacs.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gyemkplfb.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gjyudoixh.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gswttnegj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gdjxbwfqb.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gowrvajrq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/grvlcukzc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/giwgaghti.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gbovorkeh.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gncdrigct.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gphaaduen.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/ggdvmbflk.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gckcpsuyg.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gemwfevgh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gldcwktha.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gfothiaym.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gylziagvf.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/geqsyahba.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gmzwgesft.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/grdqfxkfy.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/guxyrskeo.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gqdnatvtt.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwjamuqb.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gspkqkqki.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gwbrcrcws.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/ghhofmbht.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/ggckpduho.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gpncvmqjo.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gtslswcmk.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/geynfciry.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gnffvtshw.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gjylxfskf.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gmcgnbdkd.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gbqemmnfu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gqijliwqm.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/garjefpqh.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/guvrjbfyx.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gvdkauzzw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gzftwzsxw.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gksequadi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gnmjvkraa.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/glqqlehig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gteozsplo.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/guamqjwbu.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gvyadilfq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gmtinhjrx.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/giunhpcjo.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gqktfkgln.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/guvvwenol.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gkigdbjlz.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gutjmesvm.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gulkplfkp.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/glckexwoq.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gpfzttrxo.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gipaezgyi.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gxhyyhtwc.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gduqmldpj.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gjhflkxys.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/grhtijtop.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gfmqhpziy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gvmvkgxuk.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gluojnjdg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gmntojkek.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gpiarqmgf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/ggzgfgqwz.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gpjfxjmcn.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/giymmwbgt.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gsdbngpal.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/geuvpagkw.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gqybwfepr.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gqoptwudq.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gpilqbeqx.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gnakwlymy.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gpbrhelrb.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/ghjlgiwmb.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/ghabhkksq.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gmrftyzfd.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/grtmamahi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/goptrcaxx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gtwytflcx.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gderxrzge.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/glmvcpyiw.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gknybfcpb.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gmbwejirv.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gugecmetp.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gvffhynoh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gmsmudzag.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gkkdovidg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gjajwwfjl.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gdokujrzd.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/glqxgdcjz.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gpwtapvfm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gqdpsxwlk.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gywesojlo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/ggjkrlrqw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gjwutsjmk.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gvdktqihv.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/geaxixknh.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gbmtrqlof.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gdrvwotjr.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gcvaltsit.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/glwxwsifz.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/ghbcokruo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gxuzkpgvk.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gmrufstos.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/grilfokjo.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gbyklehyx.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gixjwjxhr.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/guilmsxhj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gkyccpeji.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/ggdkydywt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gifpzqkbz.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gdmauoqdz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gmbpgqrcm.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/grquatuaw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gmapkgtjq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gypixjhwg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gdegriiso.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfctfnnsj.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gptkolcaz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gocjegbjn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gefkdnprf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/glahzqbbd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/ggkntfywk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gmdonqnhi.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gavgnjcqd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gdcqzoyjp.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gzxgoodls.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/giraygzbi.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gcnfdngub.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/grruygzqg.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gpbnhepoo.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gxynjzaxm.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gojcirtyd.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gvoixvokz.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/goxllxfki.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gznhcmdcz.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gpqptxisa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gqnfrybyu.sHtML


<!-- 参考信息 -->