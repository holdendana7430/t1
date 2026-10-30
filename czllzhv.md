代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gdydobzwv.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfymztixz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gpakpzqaf.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gvahzapur.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/giisnybkj.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgssjflx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcdoyuts.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvnnrzwe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbnxdbefn.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gflholgcf.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfiiwbyc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gavlfjsxc.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/geggojnmi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfheyidge.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcrnotle.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gbimhshto.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfjfuuclh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqpfztmu.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gumilkuzy.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyjrdarl.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gikeoozmp.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gufhrbwbb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gjvlqtdcw.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnptqrpkp.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/glwokxjgy.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgihhviv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdunjvrop.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyukkzun.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghloesvyu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloskovyu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/golsxgsnc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtedsrlxg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gucrfgbnk.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gwrfmwopt.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gswqfrfol.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvgobnwm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjjnubru.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ghoemlwdd.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gwrhhhpnj.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbgsmmxt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gdqedyzjn.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwiangsq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjuiozyq.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gufsasnsr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaguzjapy.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gtcegbmcj.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwjkoimw.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gogcrghot.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gdzbqdqlz.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbbafosy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqzsmicw.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gsqhguysl.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkseroiox.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglnkmvcb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/grophshmg.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdyypupf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyoushiu.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghodpdhza.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/ghbwyojol.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglxevoem.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/ggqmwpuhd.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfssadpi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/geebxxkfl.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmglvuzp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdkijijn.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gzsgyhely.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gcqlewcxs.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gjepbttzz.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gfhleqvpo.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpllykxbo.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpthaexda.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpguvgxeb.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgbafbcl.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwariplav.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gjqmyogsd.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/guncozhbc.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gysdlefvc.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gblodwoyg.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gimowrpvm.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxllfaaky.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gnqzmgxqk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvriqphzb.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/grfsvrxaz.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxrhxmrj.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gidesbayy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfodiops.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gzbidiuxo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmiygykx.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/glscxftbe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gahcnineg.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gutsncarh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdfpewxx.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaeqrhcd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhwylgdc.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/guwydjzdf.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gwudxnxym.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/goehgugyu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gmtsysrai.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gmyirckpm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywowqhcx.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokxtassz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gzzattivg.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gopetxnkg.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/ggqwnzten.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzrfujoj.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/ggfynlipg.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gnzfxsekw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggxfzilmi.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlrfosyo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpdobwed.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkeubrtq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gksnccxvr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoqkqmha.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gifwpstrn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwtdnmta.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxynfkrui.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gswtchgif.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvzickwza.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gompumnkk.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gpvxszzit.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwpijqlk.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gwjcmvhaw.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gngkqeyhu.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/ghfhjlysj.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gglmibcau.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/giizikdbm.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/goryfxbgd.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgoisday.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gfbpqwhdy.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/goxshqlba.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gzunrtqjy.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gcstuugva.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwwqoyxi.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gxdxlwmqc.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrtmvjip.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golejqdvu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbmrwxwo.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkqtipbv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gfjabyjsj.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gwukjgjhg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gagyqhmvz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvmrdxfsg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gbpxkavgz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjnpnlugw.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glbaarcmk.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixamuvhj.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ginlwhjsz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzripsbv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvhyendq.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gssnllcpi.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gksigeero.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/garralfnf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccdyacyp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/ggnpyszhk.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gtosvivio.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxxgxcow.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gpuzudgqd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrevzayf.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfybmzez.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbrnylph.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqfqfuza.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuudurnm.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/guzkvbhlc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkghtnqps.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gebgfukuj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/grlkljalh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gykuapcjn.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqolsxcjq.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gokbqsxbo.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gldshzsht.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gtxfkvfoi.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gbqxpnfiz.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gwrfdxszr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbmihbjt.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbofimvu.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/grrfiqrtf.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gzhvuvexq.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gyetmtoeo.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/goysalixb.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gaiuulgjh.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/guweoqili.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjrwffpy.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/glssxlapl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gkxxgpzjp.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gphklhitq.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gfpxczkkx.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gfahihdff.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwbjeeytt.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmccwdkva.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gjalsgeju.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gphmadxis.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gjioluqbr.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/goozpamod.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gqtwauewz.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpdzcszc.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxnklfzp.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gcifwdses.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpukrvzx.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnsnjnnm.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/ginivfrwg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqasdjcb.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/glrrwjjkv.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gyppqqbsl.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gphnbnqne.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwqxsqufa.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ggysbooqc.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gripnhewu.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpjjtwns.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gttnzisqz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmcclyym.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gizsqbqui.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gaiaeptke.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqcxejvu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gllhqnyct.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsynpuqvv.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrlmnsks.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxvtjdop.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnxjkpbw.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfigztvsw.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gtpcklquz.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gwnotgpip.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcgfwzpv.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gsmpihdxd.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxmazxty.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvottwkil.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gjarvmavl.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnhtvhlm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gepkmlusb.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/guvttjqxk.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gnjwixbcc.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzzragcm.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhneuqfg.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gjnudrupw.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfmskgyxq.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gxokkcfre.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guwtvfkqj.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gwecqwist.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggukikzc.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavxlvwqw.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gxekdpsku.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlzlenya.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glcpuwfog.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrbtnkmb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidgqexea.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkoxmaigb.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/groyllsmy.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gziguwxbp.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfoappvd.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gwcyfuagl.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzcwixvu.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/givahlcbm.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gplclhtoy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/guqkztder.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/giyrizkgq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqtrsecb.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcoqesoy.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gceljjapz.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gpwzsqedf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/geljcuhjp.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghrkwefof.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gzwklxgbf.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwqmpjfx.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gbdlydjov.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwhtaxet.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnykutrmu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnayecnn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gmgtnjgmv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvfovsnx.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyqziwfd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasiyipic.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gfprohzfx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gamrrsxod.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/ghxowaurm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcrsnynx.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpawuorf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gspzdldmm.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gqobtbdat.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gfbotkgja.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/grmfigbjm.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/guiwdzdam.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneclzpue.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/ggdyvqogb.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gocyhizsk.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gckxgvjml.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtckmurv.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/grhbtogzd.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuzntugp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqlmkkkh.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyzpwakr.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjljcpbtf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlxqycxc.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxwmrczw.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjtzmija.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/giwvgfisx.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gtofdimtj.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gsbytpayo.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gletsalaz.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmofwhkeh.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/glgjxaipx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbxkxsor.sHtML


<!-- 参考信息 -->