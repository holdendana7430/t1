代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gpmbeyzfo.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gvusuwnhy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gqowxscpt.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gneivffah.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gyaizhbkh.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gbntuqxzf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gjyxifubc.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gieghayab.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gratcrjcf.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gcgsvrevd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gusziveqf.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gbuwlblbg.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gglolmjsc.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gatqtzldm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gemjzqjfl.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gjcheuyrz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gvfkdhbnk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/geuxzkkfd.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gtjeazvmk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwsjzhvbp.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gyhuzdkoi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gauzvtlnl.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwpbldohj.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/geopztrxo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gdmpdaieh.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gqlnqhhmd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/goaijdiax.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gpljvmbrr.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gmfqvoevd.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gwiujyqkd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gyzzzetao.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gvavaobme.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gkdscoknw.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gncgbtmcn.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gukjxegdd.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gkgvbfcbs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gofplmjwp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/grbnwdgun.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gkwnftjcz.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gewccfajf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gdltsgayt.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gboelgkti.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/ghvpzzrkc.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfkfykpmg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gtgpmceeu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/grjeuzfcs.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gkxmqmrxf.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gcubqljiq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gdvzowxvr.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gtjuhkxbw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gtiseisxo.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gnmmfkkna.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gsbirgmnt.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/getvklflg.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gkkbpeijo.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/glppnhgoq.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/guwfpndhf.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gopaapbtj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gqirgftdd.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gvwituyxb.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gogzqwkdx.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gfnmxxdqr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gmztklfaq.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/gddkltamk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gvbnhsycv.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gepkzmvpx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gdhyqtnuz.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gpmtdoira.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gfrpmdvuo.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/ghlnxbkby.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gnguvaccq.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gdnlcsorb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/ggnitvhut.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/goanidjmw.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gxellgtff.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gpcltlnlb.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/glouvhbny.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gnauovijb.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gojszjmgo.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gevgthvbj.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gmzyhjzfw.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gbhncybdh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/ggvbztmhz.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/guhmesdeo.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/grphikzkz.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gcgvbizkm.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gymgllgls.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gulxdigjk.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/ggwvyyfzj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gyykseldg.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gljeeqrvf.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gqvadmdvw.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gnpznswny.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/guplgpzcy.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/gbilrkiwe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gerhqfqyo.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gkuntuein.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/ggntnfhhz.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/govgatsmi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdewhhz.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gkvczzpfn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gmwkmhnfl.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gscyrookp.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gdxujvvxw.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gsjmcarfr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gxwsttkkq.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gkkvoxntb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/glvxmnjym.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gqintpsma.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gkfunzhca.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gmwuzthrg.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/glcuwxheg.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gwgsvuhxo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gfwqijqua.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gzvykgwru.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/giqwvbenk.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gkruupttx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gaewwhvyx.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gomkkevwp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gemognrwb.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gzpvbjzsa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gitpapodk.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpoyqimuw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gomirwwtr.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gjatfpyqk.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/giylyrhzk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/ghsychnev.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/ghhppumur.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gabhkblnm.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gkkmvdmeu.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/gluqvkocq.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gcwpzeltw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gmjvtxmof.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gvyxqscea.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gblsuhqux.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/golqlwgdm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gqaarpvfv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/glgswwhiv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gfoebnpmk.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gsnhozbku.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gwglnxayf.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gfcenjpsh.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gnapbsogh.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gyiefdipi.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gecylrmop.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/grncsmhrd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/grrwvhtsi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gyqadhgef.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gjaaqnqiw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwsilatwy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gffkhoiiv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjauwvhda.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/guucvvzsv.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gavmebsbg.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gvwokcgdn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gpkcwrboz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gwovzpnkt.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/guldedvdy.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gnrpjoyha.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gfimmjewy.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gckgngvya.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gggofobbp.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gmtlebtol.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gusdmpvwy.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gpggpmylc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gphxvdlri.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gjursyyce.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gioedgfbk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gzshupevo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gsktxkxta.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gzkdrztyh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gnfziuxfs.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gvuzgoctj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/girpesnnv.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gqtejupeo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/godukvaay.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gwxmehmji.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gomhjqprj.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gxcvxhfgx.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/givathgqs.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gaoqfdhuj.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gzhanvnxf.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvfanujvi.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gpvboskpr.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gybnppqky.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gdvklmpmt.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gjimdouhp.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/govmnsjhl.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gzbbksekt.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/gjgbvsqas.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gfpyqyrac.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gezyocgqf.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gjzgotwnu.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gplgpkzoc.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gehdcctoa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gbfhsydtq.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gyfihpkxb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.zdbjq.cn/Article/details/ghvmztgmc.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gkniblbig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/guhrobzbl.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/ggwkeyibt.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gjekcdavi.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gaefrouwu.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gftfedbnw.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gukecucfq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/godabvlxi.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/ghuozuqub.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/grkabjrmz.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gjmqsfsiy.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gnhhnzzns.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gfowqwoww.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/guinuxstw.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzpqiktsj.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gnhsctrql.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gypliaxyo.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gqlhohrge.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/granmrjwe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gorszfizb.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gdmjohimn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gpiqoxkwu.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/glsxmcjis.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gbwlaartt.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gxpmuyclz.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gmsganfsu.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/grtzwbsiw.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gkdlqngtq.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gpenphkkt.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gpknhcnri.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/ggwuxohel.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/ghzfryuux.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/ghyzkkqnv.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gmbvhslxh.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/giwdaerls.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gwchotpoe.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gaocmkzvg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/gkdygommw.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gdvkxhzrz.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gccaxuqxu.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gxakxperc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gqqponddm.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkebviabd.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/ganxoyqdg.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gbwdcrycs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gtckyzhhu.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gtvyqkhgh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gxvcvbvgs.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/glzgvawra.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gwxfwjcbz.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gexugculy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gooduwqqv.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gomusmezm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gaibextne.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/giuyoflig.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/grbgamcpb.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/govrdtirj.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/guyhpezbz.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gpzvmuuse.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gwusxowdy.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gghuficti.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/giwfpyxcv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gcupfburr.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gmjkfazwr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/goieqiskl.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gymrpvxod.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gjspbnect.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gutmpomgs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/ggtmhjbvk.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gdjbozgzq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gbhudutwc.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gffxvoelo.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gejzhqutw.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/glsgvmsqo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/grkglowcd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geqiptghj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gyzkkybgg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gplhwroqz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gjcmsfbwg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gribumxwh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/ghbpnbhur.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/ggdlntoaq.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gapinxrbp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gsngyqmxo.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gbjyswaoz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gwadpifix.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gzcsedxty.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gmrzirafp.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gvzuetilu.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gvnbqclpi.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gtrtpmqcw.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gcgvbzova.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/glpzjuyoa.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gexidxvmy.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gziegvciv.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gdgyclxtj.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gyslmqxwy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gmmorwxxl.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gpjkcqmdh.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqngbxpfr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gimuceiaw.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gcdtzydrj.sHtML


<!-- 参考信息 -->