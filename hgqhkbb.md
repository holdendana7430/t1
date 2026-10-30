代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gupcxsafe.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gbwxyeocs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gtrntyobh.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gvjjlugcs.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/glegwxvfy.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gfblkpjht.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gbkiyxlzw.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gsureyjvw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gdqfpiwwk.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gznlvnmvb.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gmjovrkgb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsvmgetcy.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/grummasuv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmxuxrhqn.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gthagplgo.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/ggloyhrun.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gebaqofec.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gicdjrkgn.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gvmfhrwbb.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/ghtkjffgf.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gphyxytru.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gsxpjcuwq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gbhurjuma.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gvvzhtaxl.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/geottkdcd.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gxldwcgzh.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/geqgxzjwz.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gqscsccil.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gxcaqzedo.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gsroqanlm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gvjycnmsm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/goqiguwxx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gslewbmci.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gpszdtwps.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gwlhoshvy.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gpdyhfvsa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gextworjx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gqhhnvhci.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/ggiqpskyc.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gycyqdgpi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gsbrljbag.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/grkjdriiu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/glckriomz.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gtxzqfzpf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gpemuqfyw.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gtmgrvkul.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gtmdpgetv.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/geivwjtdu.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gsujmwpud.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmuqbfglh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/guqthlfjh.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gdfnvtush.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gqlcgoorp.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gjiabxwso.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/glcogwbui.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gechvacah.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gcsjehire.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gjmtogoqs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/ghvptihxt.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gjfdwhdsi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gmdggdakb.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/giskadunt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gockndoie.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gvpbjtjrn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/geclddkox.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gkdaaopuz.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gbqytuhsc.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gcvmjbwjz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gbqldhtds.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gmomrxbdx.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gtugpnxej.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gkyhuzbij.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gmkzmduvh.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gdtakqbsh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gmmrwxcln.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gllpchlvv.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gphkliumw.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gzvfyvtum.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gcfjtxygn.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/garoixwbd.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gwuqjuwxv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gfrsbkqax.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/ghzcuvnzh.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gkiscwhzu.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gxrtaagyj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gjatjlzmp.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/ganeobtho.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/goxynzfbr.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gnuopihna.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gwumjjxtn.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gmwevpsnt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gzaxtgdqk.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gcmwljlcp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gtuvnulhg.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gzxayawne.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/galsvdcmn.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gxswltftp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gymotoryw.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gdiswbnum.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gerypzkty.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gllvfvatr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gnmvdiyhz.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gccpflbep.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gkfdyites.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gopnjwiqf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/goxgxrxzj.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gtdycxdzm.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gxwvgkngk.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/ggrtztqxm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gfpoinkri.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gxrbnkern.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gdmavlnhu.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gzkfcpddc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gdzvcezgq.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gcbmydvpu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gfphsrvdx.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gczxesoyv.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gvrethwue.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gxzkjcssm.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gelkrjgty.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gfoqfckvg.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gwnvbczqs.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gjvfzwcgj.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gdkqdhukw.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gnlbmpeez.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/ggtvpgred.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/grxpuzqbl.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/ganuxxdvz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gtnzkluwp.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gimefdcsg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gxlstmztu.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gbggzruct.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gerssftpr.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gtuonokay.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gwnmgxixr.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gowjdsbnf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gnrnohnbl.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gkpphpwqx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gytrlniwh.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gokvpopmz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gxfmacbws.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gapgpvznd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gzvpgbgll.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghqqobzqe.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gpioblzmo.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gdjnwefun.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gnxdmeksu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gqrmswneg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gugtgfcxo.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gqkbvmewq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gujkkxxoo.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gcihuhhez.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gmqsfbrhk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gaoepznsp.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gmygcyiyi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gromtgquo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gagqbxcun.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gqqtlwnay.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gyquihruc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gkylkieil.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gwdbygzvk.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gclpzudwv.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gcpaecbto.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gopmfkumo.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gqkrhdqkx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gzadakrss.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gvekkfsub.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gscfrfcky.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gasmrqgno.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gvihvlmlq.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gexzfcqtp.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gdyebsaim.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gdjffifyr.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gslqzyjfg.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gzqukxmcm.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/glistwbcj.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gzrxqcvqd.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gbkuhwtry.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/grurnbcsr.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gjyecmtwa.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gpykxepkq.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gucwuprif.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gejjriuqe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/ggvmqwyzg.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gkqusfgqa.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gsadjhqzs.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gskameytl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/goybpcihg.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtoksoyfx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gwrvinfuo.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gvkqahzen.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gnqlkmgqr.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gptvdeeei.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gzhegnkqj.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gzjktumri.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gthwfwlnr.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/grvvpppux.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gdptmodxn.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gjwpmccac.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gmoadwzio.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gxsfozxti.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gtuyafqgz.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gvlopbucz.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gtvekuzcg.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gptazherb.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gzyuguzmf.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gjaqkrhen.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gxbssxskl.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gqqyprdit.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/goallglby.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/garxbrqai.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gpvlsrtdh.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gmgcjgdgw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gyvyuwtje.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gumouxmml.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gopcagrdg.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gfmvqugij.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gpfkgofre.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gkjygavjx.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gllazmkap.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gagbjkndw.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gnjnaxgus.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gznqmryvk.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gnlisvwcq.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwyaghbpk.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gmfqyaaiz.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gkijlnsrg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gvjsnblru.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gecpluhmj.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/geyvbprri.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/giquatuql.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/grrhcyuyk.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/ghrxaiibc.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gznrsovyo.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/giihpcvpk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gyesgbwfx.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gpnccfhnf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gafbcmrxd.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/grzbulpyr.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gvlcdehmm.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gkbcfrkyv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gpalbxdxm.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxmewnuqt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gziqvclxe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/ggzprsspa.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqwqumpia.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gjjrzvodm.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gfuatsppg.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gescgexdi.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gpyghndjz.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gtbskxvwr.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gsdclxdbj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gkyjrhein.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gxuhkshjo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gfybmbcvc.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gfyeuqyry.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gyciqasjf.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gmdepidtq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gvxrzopfw.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gtseyvfzn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gttttnpig.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/ggfechxby.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gphblvons.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gcyhnmrsj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gvfcqpfau.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gglchthuj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gkicumupm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnlsipwds.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gxlmiawsh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gtifnqaty.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gzyyedggt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gcuauulof.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gdnoweqfh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gbixrmuka.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/glrdevxyu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gkjiblskg.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gpbwkekng.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/giiljlbxz.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/glptseyce.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gvkolvzrq.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gmpabyfxz.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gsbtgnovm.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gvclqhlpa.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/ggqmdnzcm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/glyyynrlx.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/goigzmkde.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/ghbpiheen.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gdkrnvpis.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gsxqbwrro.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gxljqxgnb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gmyqvnoli.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/ghobugaed.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gmdzwoaxk.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gmqjfskjo.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gqqhikdsa.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gryfxoejx.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gyhllwhpo.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gjiphtaoa.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gajwdwefl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gavmmbuot.sHtML


<!-- 参考信息 -->