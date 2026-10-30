代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gijvvquer.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gdnddlfun.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gjdmgyuat.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/geehvtfgp.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gyuvqpjmf.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gpwrywshe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gyxepszst.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/guygudlbo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/ggfphgfet.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gpshuodwe.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gazsaclli.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grcoluvqi.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gvwqxlkvo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gchxufwan.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gheumvguk.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gxmaywptw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/grtyffnrr.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gftjkgdok.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gezkysjja.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gbtyxxwzu.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/grqretloo.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/glfujbwia.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/giduepgjo.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/glofdyneb.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/geucdvcog.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gzvhqrgtc.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/guxpazwgz.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gmbwoprzt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gegbujgnc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gmfdwlfeu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gzsfhaeoc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gngwzldhk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gcvwzlocn.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gpysoikai.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/glhobhpuh.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/ghqpredte.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/ggqlkqcou.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gswqpqvmc.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gvhsftflw.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gvdyzlbmz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gzecjryvr.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/grzxgcbqh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gpmqqoxyn.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gxefawpdk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gbcpovwnp.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/ggxkiljfp.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/ghliwiibl.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/giqiolkbs.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gldrbrxzs.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gsnvkvrqn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/glebbnnvs.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gjhgtvbyb.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gwxebhzct.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gszizhsiq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gfdlsvttu.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gwqixbbrw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gksziatbc.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gdrveijdr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/glvtlzgbm.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gpdxnubaf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gfyceutmu.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gmkopghgn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gzmdoxtml.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gkvywolzf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gtxcowzev.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjdwqvvny.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gotwrjkgc.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/garogqnhz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gthniibkg.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gkjzojjes.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gyiifdvig.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gxdmkebng.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gseuxccwm.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gbmjpxzvt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gyxicbloi.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gqkqlppzy.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/goabrhvmu.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/giedxrnpi.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/geoziybnx.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gwtbjkkpl.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gqsarktzx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gyilhrssi.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gznvhgjwx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/grqycvhah.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gathhjrxk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/glxrohhls.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gfuavzzrh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gspqohamp.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/getowvkve.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gxtjepimg.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gphspbypx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gnvemukkj.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gmrpjjnhv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gcnilbciu.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gkkcqibey.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gizjazmll.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gudtubdde.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gxahovafg.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/ghakhstae.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/glqylzahu.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gbkbzanuq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gtjjiusyf.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gqyfojppp.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/ghabkjcwo.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gbsbasqup.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gildjfbua.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gnnmefvrd.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gzfxmmaag.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gamoutfxr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gmyvcnezl.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gqtqsmzjh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gpifujfet.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gslrafgot.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/glzqueruz.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gnxhatmht.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gxdezvito.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gqlcgcbsb.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gdhaeoafs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gmwvwmnda.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/ghbydtkgu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gjmibodbc.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gvvppawef.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/grppcynxa.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/ggoedrapu.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/ghdaquqei.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gbaoofbfy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gkocfburj.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gfhkkqufy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/grpligpud.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/ghfdlyyxl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gaqppqqsd.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gwflxlufn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gtqumhwfv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gkdgcyhsz.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gcleoayyi.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gvtjbxxtt.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gumznhpxt.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gejwnatqe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/geqnpwayi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gnodwplwj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gxsdrrzjt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyrqvibsa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gtcwfssqv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gesnrjvrf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gyhykxicx.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gdftwpiux.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gxbgzcmjo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gioxyhgtp.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gdphtnyxi.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/glesprgjm.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gxdmlwffg.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmltoznln.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gldhwsevu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gmxvithgk.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gtolkbghz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/grpxaycxs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/glpvievgf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gertsredw.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/ggpltvtcj.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gfskigzan.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gfstmfgyg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gnyrqmyfz.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gzytfkxbg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gdmwjarbi.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gqugwaxdm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/guahlnkch.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gyywjndkz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gyafjjhyu.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gsvayjnrp.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gxzfhinbq.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gwptklqzn.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gejinkxgt.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gjktyznxz.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gdvbiufjj.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdxuuuqey.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/goulabucu.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gozphcjwk.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gapxwkagg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gksongsby.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gvauojrya.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gmowrjcgo.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/giflkloxk.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/glvmgbkmc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/gabfwedqb.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gbongsvfu.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gjasjrmtz.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gjxkejuqj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gmkznsxbp.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gtzcfnxtt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/goecqxehy.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gfsbzfzqf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gfktubdfd.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gnwkkmkhk.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gyozqzncs.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gxpqeyxot.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gnowdnnun.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/ggshefyqn.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gufcxwadn.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gczyavdny.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gnxnukyzq.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gvacjrfau.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gkpdywvoh.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gdshvtgnt.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/ggbxbpoyv.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvswwzuog.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gieavjram.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gtdldvxjt.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gsnszwekh.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gwxneydrt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gfdpmcdne.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gxucidhap.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gpmcvidmv.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/guxoqhmoa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/goprhoiow.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gliqeyber.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gsuitwlqr.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gpjyoeutu.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gfnrpyfvt.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gpbmdtfzi.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gzexfamss.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gzcwbzotp.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gbmtioenv.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/gmbjtxguh.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gbeudoise.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqyvqzprc.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gscigdwlw.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gsbqdkkvd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gmswpvqma.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/geeulfvqq.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gbavxvszr.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gpdffilcn.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gkmadskwp.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gkrjwqswx.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gzfnsosai.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/ghidtsasc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/glqcnjwqi.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gqpqvqtph.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gxiuocbbu.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gfltyvvsp.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gmcrxiwqw.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gqxmaklke.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gmsjtjdom.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gszmqgzpo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gjvrlnwef.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/glvzvghot.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gbaergayl.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gulumtzcn.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gxctwlubi.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gkkuntxwl.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gumbpfoqv.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gylukngub.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gbjtweadf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzkwmxofx.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gklhxjrar.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/ggjjsibfd.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/grcdpqkyg.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gzzllnpuk.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/glxcylcfc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/ghcuvqtbh.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/ggqhqbdad.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gdebxohdp.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/ggacggtgc.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gmmhbdete.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gffxcailr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gcjmzbbyv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpdifdqfq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gptovclgz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtqylljkv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/ggfrhugic.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gcbqcbyst.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/glldyjezz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/goqulxirv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gipromray.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gtodfippv.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gtvpyosdf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/guchalqhh.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/grjpgdkun.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/ggwurtjjr.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gqtcarsof.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gvsgwoiys.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gaqxbspnt.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gccttvfht.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gjgpqekpa.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/goipzvljx.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/grqdyjkpj.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gdszklnwk.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gidcgtilf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/glaqklrix.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gtxpdyylh.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/gfdlnhasl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gemqqrggv.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gsxscjbts.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gaeqweesn.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/ghpjoaxkc.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/glepxpwoy.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/glilzonbt.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gnfejrbrn.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gvttvsxzi.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gysgezjhi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/giuuqyrrz.sHtML


<!-- 参考信息 -->