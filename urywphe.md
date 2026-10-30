代发 wailian999

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeqntcxn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvhjbthru.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gvxoyemwa.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqyxiltm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxufnhgw.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gymdgyahm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyqffqrd.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnjlmdgo.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbakpdxz.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/glbjfxqhh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezklklan.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmurujnp.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gksnpdgfj.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/geivigkml.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gciuhwpei.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gucojlfcb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnoeaqjp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyidbctfx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrzgkrtk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gederjldt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gbozuazgo.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gqeuvluxw.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrstzxfj.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsszmghsb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gawjuuywk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glseeaisc.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvizhjmcr.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjxkrocu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjcpaqum.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwhbuwqt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsewihyms.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/goegusjoe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gokfoqkzd.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gkxaqdvkv.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gmqjwvbbi.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqqkmhee.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gigizribv.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gewinvxgp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gluryquqd.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwwfogqo.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gwacziyqz.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtvvbbtpu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkieueaxo.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfwhxcvc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gwhvtfygf.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gyaxexotj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/glaoaqhua.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgiehdei.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/ghsnycxvv.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/grigkrhng.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/glkixigvw.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gradijtsb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gfavcjtuo.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gtaufueke.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gvsunrgca.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/grpqkhxmh.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gwocryqpt.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifbsrqvx.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gutfeebwa.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqbrwwgaq.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gynxfrrwo.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giydatjca.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gkvexydvo.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/godsaqxlj.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gglrvcxqw.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhxxarfu.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gffoiylkg.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/goflwkrcc.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxegthim.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfqtccwni.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gokrccjxm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqoyzkjj.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gsaexfnjh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/grjdbrxot.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/guqcdsbaz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtesnezb.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gbdzdlmop.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/goadduvnx.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcywudiu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxexqocs.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gbubtpewg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gstsjmjqx.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gucsfqcsp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvgmjyfi.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gaidrpjxh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/glskbnfhr.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/grmsmjivr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ggdklndid.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gppnscrqy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gclgvtrjo.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvlclrkjq.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/guiqbhdzu.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gsgmjutwp.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gfpjntckr.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpngawuma.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunbrojmb.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmmsduti.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gccxffuwk.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gisopoisw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyojmwysv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gmztgaxwc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgwldxus.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkilrxpi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtevjdwc.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbasbwuoe.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifduehbe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfppwkadw.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuuokrpb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/grflbheau.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gzcqngbgc.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/glqfnrqmc.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwbzkvuv.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxzopvhj.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gadggaolp.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxvlczzc.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxeovyhr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/grjacscxv.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpemdisxf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gntcwcofd.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlbhzmcy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghxozmiby.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsczvhkk.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gacbxmsrc.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gndpgfhmx.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuipgefa.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/ggddrltny.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gxkjntiyo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdnpepxc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/grelnfgur.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfzmqqzh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcgjfjci.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqexmftfa.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdubjivs.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdkaqyvt.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gynpdudmt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/grsjtzxrz.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/getclnmns.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gevkjxwga.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gjyyqvvfk.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/govkzvvkf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsborykxp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gdqqtoqwh.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrqmirpe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gwegfthld.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gcdrlhbna.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gkwnyvttu.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/guxidupon.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrabnhms.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghrtjqtqp.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gvdlexlgt.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkypkfqzv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gxwbyofgn.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpshulqm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkfxwbkw.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkywtghwe.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gokynjvbz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvbnhxia.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnpbrort.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgnegtqq.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/guamcvnch.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gikqqoiln.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvozanwca.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbjttxdb.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gujtzvmzd.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlwnugqd.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvihfxhcd.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsziaulpo.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gshkvqell.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkxnpzzl.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gjmoqormq.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gvxqqlyng.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjwuqusx.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhyicosw.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gffabbyrk.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gjyxtuicj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoldzfas.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtueehcjy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gleotnypg.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxvknnkq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/glaestrxr.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqlywntk.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgfaeorw.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gjfowzlpj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gktofzdmh.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gmxtycrqj.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeosibad.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusxumuru.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gldvjvrzp.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gcqwiaugs.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnakdavbj.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbhubrwj.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gppavnara.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmgrcoxr.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gvnswuovh.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcyxdefjd.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gmlraftja.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwargiyfu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gonvvvfvl.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/glymhktff.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/goomdkjih.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gouyfkjnl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gegdxshjq.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grhlkkhsp.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/ggfypgnqk.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbdtwnxn.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gqpmudfnn.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gnxtqmfmh.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gofehlmev.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhvxzvmz.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gqahpsshf.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/guhnlppsk.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gihzonnjh.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrhkregs.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbfxjori.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpuastza.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtasyvtuw.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gejoalfzo.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyqbwknh.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnfertgi.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbdesugv.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gxcquaphr.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqtzeyge.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gpzvlrsso.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvjyuriz.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpvxfskm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmfnustt.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gangdtmxr.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gprawxiii.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtllumdc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjpwabhvt.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdekbpqhg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsxtitsq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggsabgzne.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmgagqcp.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwznrmnj.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhfddqmb.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/grvxqcqjj.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwsieueo.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzidknad.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gbuoblolv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gkxufnfdx.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gekkihjpn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gywftzzon.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gdtjfcmtf.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gyruvarib.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gimmyxvgo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqqodnwz.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gwskpofru.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/ghsvysdvv.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhanbcfp.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqoohizh.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gaufljbxt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gfwarpcem.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdonsdofc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerdgebsc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqrukxqw.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/guxuclmgs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvdwviiw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gdwghorqv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gerpjuhcq.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gaduzggvh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/gqhlzxjsn.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/goijcvafp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/godyyxffc.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gidkflkls.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwokzpvqv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gppybqcct.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcyxcmxr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/grlnhjtye.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gokhcwkoy.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/glbqfahba.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gqmdlayuq.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/geoflznel.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/giulfemnr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcyzmgez.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjgmbhvj.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnmcbygb.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gadyrxkfu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gbylvmzsj.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gkycemwbb.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gbpfaojnl.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaaxsxbj.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghucnthbk.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmjsubzl.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/grqpfioow.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbwawtrx.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/guodqichx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/ghpxdbxhj.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gyofwxdqt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxncvkpew.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyntgdjs.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqqbpgpa.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gymoreycq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/grvycwdld.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayegohgd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxmjkzcw.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaibbmom.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gcqtszpmm.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gzvtwrjhl.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuthoysn.sHtML


<!-- 参考信息 -->