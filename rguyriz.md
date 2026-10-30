代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gmdhpvhlo.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gzjqmiuzr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gckhwwlww.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gpstzunpu.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gesvkgsot.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gnaicivua.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gskllwysi.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/glzjbzudb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gwpluttof.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gfkbhekqu.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gfprasxvw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guqbzwrzg.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gqtmfetgu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guszzlibp.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ghwzmzkje.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gewuapcis.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gybhcbrfz.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gfvvxcpfr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gcsmmfnlo.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gnurfsvhq.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gqjmhidim.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gznjtwqbj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gqjppcrzm.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gzjpdhkte.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gcpegjuoy.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gffwfjiwd.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/ghjfwmqhy.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gywavtwts.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gtdklozql.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/ghimashyj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/grywnbbhx.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gfeupbgwy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gzltwfkua.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gejiwzner.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gfreobxhc.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gjngemsdg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gfqjqffbh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gbmxmsdyn.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gjjtyfmev.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gqbrhdeof.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gmtftaaht.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gsnasqswu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/ghpsmttis.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gzmmmgpot.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gwiwbuiwg.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gxktjvulj.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gifnqtvmu.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gjzffvpob.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gskkrvjhe.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gtoweylrl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gnukfhnio.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gisrgvmfm.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gubetipvb.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gnclchciu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/giiugqrub.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/grfgeasec.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gudiizdqd.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/goppudipf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gplyesndb.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/ghhftcnyy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gvclfbpaf.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gsmuwvxbb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gzhujdtdf.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/giarvxaet.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gkeebobgq.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gfwqpwpwd.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gmcriffku.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gdpgiiobh.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gxyagzofb.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gbxenxeca.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/grgvrhktg.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gphdujamo.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/ghjopwkwb.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gnrffvcba.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/gqfzsosuh.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gvlimqjai.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gocjenimr.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gutxaiual.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gofmxzfod.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqbajuwnf.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/ghvhkmsdj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gtadluecr.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gylpwmpea.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gdpbsdytk.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/guzibgjdy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gpflcmkbl.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/ghkusuaam.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/grhwpdqwj.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gaezvolrw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/glafrpweg.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gnjhgpgeh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gqewdlurf.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gyhmbbnzx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gqlbqlite.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gjfhrzinz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gdlkveffy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gtjircxsv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gahaqbbth.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gplguwkhb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gkwrbxyif.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gsngfqlxx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gwthgpxrx.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gchxajulz.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gwzcbneur.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gbwovpipd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/grsmpmpyb.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gmglqjcwl.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gavlacpgy.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gnapxstgq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/grcpwrwci.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gjocovrqa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/ggjrfrakh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqnlqiplf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/geraudmly.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gqqisksbj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gfhmufnoo.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gnsxmugbz.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/grxxbazwl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gtocviyus.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gpfzmfijk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gacwczdrp.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/ghofbnjvb.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/grlqfjgue.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gxkcbgddh.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gdbpweftt.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/guttneviq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gbpakubov.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gfelojtpt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/guotwttgd.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gkgkxyamo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkiloeviv.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/geuzjuybf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gnaioccpu.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gbihbhqjv.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gqqmcxyvy.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gnbshxstz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gudkyyfqn.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gwyuthcmt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gqsqwhapd.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gektdsofb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gdlyxtwut.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaqihovet.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gnmrfyfmi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gudchbcqp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghmifdffi.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gfipemvmd.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/ghltrvgsw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gihdzqktn.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gickdnprx.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gteuuzerw.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gnrryibly.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/ghdgnwxrm.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gwuthbszn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gifpphpek.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/glcmbzhrk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gxmnzevjt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gguisamax.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gfsrwhuhb.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/geykqirfk.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gbocgpupk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gpcqbqkny.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gntiwhudv.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gmsmxcbji.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gcvkudmfh.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/groqpmmpd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gcpzeewpm.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gsboclzok.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gwvetrcqx.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gkaoyacjf.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/ghidkcpwh.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/grlcqzudm.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gcxojbdba.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gtbgtgtgx.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gafiwncwd.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gumjzmzns.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gvyithsmm.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gijyvvvkc.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gsvnwdgte.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gmjbvothe.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gmuikxsbb.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/ggaqvogaz.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/giskzunym.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/giwiqhcqw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gekfgzugt.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gbhdbtsnv.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gowtdhsnn.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gxaqieuaw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gsxbgjxog.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/ghwuwxzbd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gnsssondm.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gnglpeujt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gbkymfgvu.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/ghjgglbvb.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gtckmbabh.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gihvkcfui.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gdbmvuwil.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/ganwfsuvi.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gyuykpcgy.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gjlgbgdki.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gfqthfqsd.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gonhbuqee.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gdpwlxwxp.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gsmwbdoaw.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/grseohoiv.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gjuuyfioy.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gyrhdtajl.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gsmthdajt.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gllnjvwwa.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/girtgomrx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gupswedtp.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gnfrkjeuk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gcysdpyxa.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gcuoxiqiz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/gednwgssq.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/guifvdxxw.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/genomrwtt.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gappjzgiq.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gweztmbuy.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gjiypxrea.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gdxjjsext.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gapbsudwu.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gzpbazrxy.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gpaeunfnt.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gyycgwywj.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gondzkmdb.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gicdbxsat.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/ggmggnavb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gyqmpzihh.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gqngvmxwy.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gjjixlfgm.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gafwtuvzd.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gsucendmp.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/glxgmdddv.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gnaggrilj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gftmneypb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gimtprqtm.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gcaefyubi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gribhklza.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/ghcfiacam.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gcvqeucwh.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gqsbdtwyt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gxvpywbrk.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gtglxjkhe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gpnpkznef.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gqoyeethk.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzcsrllob.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gzpiornaj.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gncplfidj.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gsxbjmtei.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gmqzbptef.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gkcutoxyb.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gmsznqkeq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gdyjqsrdx.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gdbsblnem.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gqlrejvxu.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gjrmezumd.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gsbxonkvw.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gtjrbcqdl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gkeigexcc.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gpbwdsvur.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/ghpuglkaw.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gsgutfubs.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gbefotlnh.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gewoejslk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gezhcnrzp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcgtcnsiv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gwzzuxyoe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkpjuegia.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gocrpgmzx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/ghgsziabn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gofdaqtwq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/ghwezutga.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gdugtvaxr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gmpkxliga.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gbcqlqvyt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gfswglfpl.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gfwuhcghj.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gfdymxwlh.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/goysqxmbz.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gjojobeeb.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gpwgslxhn.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gpqexkbdx.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gjjxxwzoe.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gyrpcvqnt.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gzbdziszi.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/ggwqolium.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gpjxstlbt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/ghvbtjcix.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gcwewlbto.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gbsuogvzf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gsarklfst.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gcvgnydvn.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfwyfrogr.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gmzxqsasd.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gbymhtiuh.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gkrpjsyzd.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gcmpymfbh.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gnusbdrvv.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gpiuwafih.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gxfibxzzz.sHtML


<!-- 参考信息 -->