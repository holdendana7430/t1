代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gworvahkl.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjrgogpzw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gdegpdtcd.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gyotpptmj.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuejakvs.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/glghzmzpx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gaworgrhb.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gvpixuopf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmgsrvbdi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwavqvpz.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfdjyshd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmcvofrob.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxfuhpmg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gscepgvcy.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gnucxwfgi.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/glflnqznn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/glthuryko.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gqnjrmdrd.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gxsdwkulg.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/giebstjqf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gumjtslfq.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gjttnhzak.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpogiymd.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyplukxu.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ghqomqgds.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gtshwzhfj.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gacyizwcw.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gxyeiynsp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gpludfpfz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gvplrxnss.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsjscfze.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gabcfuxfl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gvsorsfsl.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqegqmrq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwenxuphx.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtabzqkfu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmqgcaig.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgdbiaad.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfdszddt.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glerehgty.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ghbcvacmq.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhuyxbdh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gicxkfzei.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gssjgsufo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqrbqxwo.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtvbpxjq.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhydoopr.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/giwxdxmla.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqbhmimh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflfvgbrl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gahunkdqt.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvueuwtzg.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gnyeuyiis.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gegwmnmjk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gsufonlry.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/givefjpdw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywscvhzq.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxzbptdo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtltvwtzf.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaidctrx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyweacwhr.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfsiqwnr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/giyihvaog.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gczmsxeab.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfznbvrz.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmksbzvmy.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gytavhaty.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gtpuypqjx.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqzjatvd.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmdhzjiy.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqcepcap.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqeloqeuu.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gznehtnre.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/giehjeywz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvsdhwfl.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqmuxzxi.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvncvxur.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gcafkqcaz.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwwqeyik.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gximqcihf.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmdlvyfs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gymeftuzw.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtoidirxo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxiseboa.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/geieibiin.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gitxnrlua.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/glmzqxcde.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gakybgiqt.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gjulhekqo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckicfkyf.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gfygrrolj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixnqktfe.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixcietok.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gajfejwgc.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gbcyhlzdb.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/goxfgggjs.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsxmbqke.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzodrbkn.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gskveoihe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhtncvcz.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggxuyecuq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfsnntns.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/glzlaagtp.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmimsgeq.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gacbggjli.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golnnxxei.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/grutruiwr.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gasmxmqyu.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gbssakftx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gritlcxja.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/ganuideax.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyttpykxe.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcseewrv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrnlqlki.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gntzikeya.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gdiqtrwps.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjzzxrmi.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glwoyfmwr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gjqwyzvgy.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhrfzsqw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcjtyzcc.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbzfwdup.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gwddyyuzj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/grhhnohzg.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grquridde.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/ghkieivnm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqukazgj.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gxuhqwqil.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gmoqccadd.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gmjdmdhmd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuuhsdtr.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gimjsosto.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwtxfceam.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gsdqidwqz.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gihjujufz.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gyngvisvq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqtwskgs.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrwrhgxr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqjntcly.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gpxvjdqbl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqsdjydt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gznowjeqe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gomhgrshm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmogbolb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtnrpcfb.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gamxksgue.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/giiumzxcs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gecqxhhge.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayapbfmv.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjaqposl.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/ghicthnpo.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpkiwhci.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxtqulfo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gerhzyyoq.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwqiqmvu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrxmsqll.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdwclude.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtijwewh.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/glceyuzaa.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gxfceltfu.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnoeprse.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwskxfyvk.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoufmwtx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gknljinlw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvprpildg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/glsnuxvty.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gqindwztr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gggwftwhu.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxkyftrf.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gimpulugx.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gaudompag.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gtnlcpovh.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gfbzrwsyh.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfbarjnx.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glfcvtoea.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaqmkdsy.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/glpojxktn.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuqlhmcg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghgcbzal.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdfrxmis.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gqapdtehm.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gldmobfqf.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gqinvtzfx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwrnmocr.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gulbmcxbs.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmanigrh.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/grahxgfpg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsscfgvj.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzffafghp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gygqxjomw.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gfryrrepu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gtnvtseum.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gdsuvwxxu.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/giwfigqfe.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyfrsamm.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/ggkdqtcnl.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluzlnfts.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gctoogriz.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvzlvjjr.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqcxvcpa.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmdbvlmj.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gwzrdlfnh.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/grexkhzva.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gafnmuwdq.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gcrvqffrw.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gznmobpih.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggjxdxpiq.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gkpkdnrzc.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbdoswnd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gapvvsryv.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/glafyjtnj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gfiomvrvv.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gkfqizyzj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvpznesc.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifqflujl.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwofivmm.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/glglkytaz.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gznrxnsnh.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gremrgoeq.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gwnrwnhvb.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvlealmq.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsongxykz.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/glnbasoto.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gldajenwy.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gattajupr.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhyeyflt.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gwpmlzzmb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqubqyyo.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gowzpnzjs.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwtpxdyw.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gimsguhgq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gppdowggj.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeattrgr.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/govclyqye.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gqidyczcy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyinnfes.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwstnmjj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghpwnnbnl.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfwmaetl.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gonqhawxf.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvugdvkrs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwezolos.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrolafqw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjpunsli.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgxsgemh.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawknyuwj.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemrktyfs.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujymxxeh.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoldxqkt.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gncrjupkm.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcgdqxmj.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gstxmbwoi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmyratck.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtsipzdn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfhyefsc.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gasuklitj.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidhtlagp.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gsnkdykyg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmucovyq.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcqcdftw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/glqffjvhr.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gkczittcs.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gsituctbg.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/glqwhblcw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gixtrojlg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gawokinyv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsbhqllg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsdtuwqs.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gfjkoravx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/ggpsdfptt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gfdguwtxp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxthguebt.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/glwxncvus.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gjnjkyamb.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/geobffmtr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnryazyte.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/ghwvzpadr.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gyswsqgbw.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmpopmwh.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbosfykv.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/ggeqzpkzt.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjfvcxez.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gacqqvonf.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikpqajoc.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/ghwjzlnqe.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfktwgvm.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gbymfvzyq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzanbpqzy.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gyfvmkeeg.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcmeklcp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grfdqppbi.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gyncofibe.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbsjhdlj.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgsxdpvt.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gwslcbbrv.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/guebdtgaf.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gtqldljem.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gzmpjbiiy.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkciamfm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gltrawqzn.sHtML


<!-- 参考信息 -->