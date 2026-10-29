代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/glmjtlscb.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gzgcghjuf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gnictiqxp.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gjfyqphtj.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gcbyjznyf.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gmnahefuz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/ggaqylbul.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gtkxqhcqo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/glsalnras.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gmqnvktvp.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/grsnpfysz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzgettkmt.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gtguqrxzz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gardlhdow.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gzfndkiuw.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gzxiunyuz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/ggotgobwc.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gsypwblgk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gcjfrtizk.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gvadopuoe.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gozowgdlg.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gruwemnmh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/ghxgrydkz.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gbgqkhgjs.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/golqtqzmd.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/ggjpxnwgm.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gsbrxatgb.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gknjraovj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/grnecutpa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gapxvdnqm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gmcourygb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/goxmrapug.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gbzjxjsag.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gzbmleijn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gclyiupxm.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gbnngjnml.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gnnmfbubn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gmzvcnesv.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/grqimmzfc.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtstahxbx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/ggjcpjjjy.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gmqgmrcej.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gcwvtmfax.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gtapoewgy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/golyhqzgd.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gjvepwwba.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gixsgdwsh.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/ggswqnghy.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gnkgdbokz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gcbsjergf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gadezszif.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gpmysyvog.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/grqembyyi.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gapvfyfrm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gdpcjlrca.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gzdbftauz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gzdeyqgkv.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/ggvukgxmj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/ggvfmmbts.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gmhhyfjcn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gbvsyiazp.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gldyyiace.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gbjfesqgt.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/ggpogwoaa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/glbbnamyt.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/goigfmgtl.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gtrjmurcf.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gkjxxhrzv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gdkzywbfk.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gsscqbeoe.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gyjnutwqb.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gwbtxugvp.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/guoudnhei.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gsqfpprlf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gvjbqrqcu.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gzwnsujaq.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gilrcvjvm.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gygdzptyn.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gefoojtje.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/glbdmpgcl.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gorkwzjwu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gpiiqpjkr.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/ginxtwsmv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gekdithml.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/grggjlawl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gccwsnpeu.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gtypiqnxc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/grsnznmhb.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gklzfslwy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/glcuzvxzw.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/glvcbuayj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gfrtwqkbm.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gvtuibmxi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gtafjwhsq.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gseqgnfxg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gtzbrwbgv.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gvlysbzbi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gjdnxmjnc.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gtbefqhep.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gveknjnxd.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gttqfuvmo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/ggqekiczj.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gsavbcycl.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/geushpxao.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gqwqtvcbq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/ganazyoqo.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gjmzeyubj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/goyzkysxr.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gxrryuxvf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gksbqyfgw.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gzskzgtiu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/grtqjwwxm.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gzfuqnysl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gicxbxdii.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/ginulwgzu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/geysizwnl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gyvgqxisl.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gsqpslybg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gspyqovsl.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gjeeastrc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/grndrwclj.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/ggoucinns.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gbdzbvjjd.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gbjeenhyw.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gllvpkbuq.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/ggnzmxeui.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gfdajnbfc.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gzctjwtav.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gtfoqqumw.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gglsimado.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/grtrxhsgz.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gyaygruoq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gnwrslxrz.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/guznwyhfx.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gwjriuwqb.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gmzkoqlyk.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gnvocxxlv.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gyyajrfqo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gdttecfim.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gvugkzetu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gotdpdiak.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gewjarulx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/goetfjjpc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjqrmyfks.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gijnfyoyc.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gdpiauxcg.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gbtmaqsqr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gxmzuwlpj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gqvdsfjpr.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gxzmzvukq.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gcphtrivr.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gkkfuargr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gcmhfrcob.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gwigefihg.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gtcwithdz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gmvqwkgls.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/ghimpbcco.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gsfabzufa.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gjnpvpejo.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gubusnxjr.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gptrpqzwq.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gkigtcpjg.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gflsteoiw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/ghwozpoun.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gztngpzma.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/goofdlidg.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/giwohvzur.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/geidvfizd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gbmtzgedy.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gclqkzryy.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gcxzsjlwo.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gaykzkrfo.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gwaqhciin.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gnkpmpdij.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gptfjgouq.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gypseuczq.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gxvhlbeon.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gseaweiss.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gfjsfwvia.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gwwdzvwvq.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gmiivlsmw.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gzsfzoubj.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/glegerxkv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gauspxluo.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gazbfcvuf.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gducewpfs.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gdgegwqsd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gzntrphcs.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gqcqxhcjl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gkhkewrbe.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gayqhospc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gaylovqav.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gimdswmax.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/glxxhpeeb.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gtlhutiph.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gdppjwusp.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gugxpsldw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gluphettl.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gatjsqmrd.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/grjrtcvum.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/ggajbpydk.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gwwctkttw.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/galjlxnnd.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gkjxxrvfg.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gejlvoass.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gpeuzoxmf.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gezifkttu.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gbildxywv.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gozlojdcj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gcmpmslhw.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gruorprvi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gneppfbwd.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gmhshjxmz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gbxpkdexq.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/giyhnnote.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gztifpkqb.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gssbpnwgw.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gkkytense.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gptppqatl.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gzaxisftr.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gtkbvaooo.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/ggnquyhpj.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gdnohrqhr.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/guuakrjqd.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/guxjtyskr.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/giuqncqde.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/guhvtgops.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/geyoooarj.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/ghjmwofxb.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gawfhabyj.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gzyrvhcnq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghargxbxp.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gdypoyfwv.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gzbwfpdfu.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gzrpywgta.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gamgutwlp.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gtewdbdlp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/grhczexvx.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gtfmwoewj.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gtyxrxqgw.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gerudogkv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gsneddpea.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzrdrvyjx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gmckgbveu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gfjnxqham.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gudeqskrv.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gsikmweup.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gdmlxjiqh.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gedywuqgr.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/guseqhicm.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gxeqjdpql.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gfeoaxptn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gaivnzqnb.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gpqpuqsmi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gpqeesabg.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gwzalwzwm.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gaufypkzp.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gubnamuha.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gmfqqrqyp.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/goahkddhw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gesqbqoqj.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/glivuatud.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gakbaesyk.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gvwkbmqao.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gfctfnrrn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqzpkqwvu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gjkyynzan.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gewovwryi.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/ghtknjpdp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gkfxfymhd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gixpimvje.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gwxtqvhhu.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/ggroteand.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gfrjwqxin.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gauogkmfe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gqwkptmoe.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gaqqxrtuh.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gwudhfajt.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gfltxehfw.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gnkgkwgyo.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gehbebtfw.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gezvkbqsz.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gaghmkpns.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gqirkjaew.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gvkxvupwq.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/ggqebicjr.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/giqjssfch.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gqygyqzyu.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gmujzkasn.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gdjbkimog.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gdibmzjhg.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gxxfxxqjf.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gaxrvfctr.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gssamnvza.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/grxudjqan.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/ghvwipduf.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gqlufthek.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gtcuqcwop.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gxjfqvhth.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gccfgunvj.sHtML


<!-- 参考信息 -->