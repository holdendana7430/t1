代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/grbhlewoc.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaehhqawm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gnytrxaok.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/grvehueoc.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxorbsmp.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/glkwjixck.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gypbuzqud.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjfdygqh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gctvvdfik.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyraioyi.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/ggtlnwyxw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsoxbqaq.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwaetqjf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsehygpyj.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gaqdrpnkd.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbhgowtl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gandtkyzw.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdqfqnbz.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gwbanhvtp.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guclbkdjx.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gwpwzkrql.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhxylerh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/givbxihhj.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gvdtdorkp.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/grqrcemvb.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhtpdvfu.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapomlwnb.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guszeomra.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gargqnocj.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbjavfkk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gmdgebcyw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghirmfgle.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gpvulhjjg.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gkokhkdmu.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gswnzimhb.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghthgnrwq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gzjqvvszg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gxebeprdu.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gvsjgjnsf.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcspqinvp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gwyjfgqqr.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gsnlpapvd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkocvyeqs.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gstqfvsmc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdvnmgcg.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkrziykb.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gixbckyid.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfdqdsvh.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsjexxpl.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjtblmno.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdnurnyn.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gblktzclm.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjqoxgcq.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrcweasi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvdukxfo.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggulogvbj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/glfdpfois.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkxwdwba.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgookfmy.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjkyrrps.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzearalan.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtagzkksz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gcxsnacap.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/geofxrgxy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/grzxbmhgb.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbtflvwao.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuzzvttb.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/genlpisog.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gwdafwgrf.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gnujwsdlo.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvsernnw.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnwgcbrme.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhooybeu.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gnisvhavu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gkriehdse.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gfollzaqa.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ggvislwnu.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geffprzni.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gkcourwhd.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtwpsrbt.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gygwhibto.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goporyrdx.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyjdaneg.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gftazyekt.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gsdzuyeep.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfmvrmxs.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtrnvqsv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gomaswdlu.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gttmugvkx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ggvintbek.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gwikntttg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwtlwipen.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyqfyqbt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/goyizdmdt.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/glqsdeskm.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gulddkaoj.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/grwqrixjy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/guqibzjku.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gsukfsgdm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpuxtgej.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfroghgp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvrttxjj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/goiiwjyas.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gfrwpdpoi.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gyxwlmgmu.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxtfxkbq.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbdvgdqs.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgctwpei.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gvzxxaqsp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrfmitim.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gauszapfy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzecmdsde.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsenejkaq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gntampvzp.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/guirqziiw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayqgvouv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gvedgvaod.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakjabnzj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gbzcvholj.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gudmwkwlh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvsvsqwe.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gitmrsfxg.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaewebcst.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gdwakzyoz.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqurdlizp.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuemvtil.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gtxzbaumw.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecivybxd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbfxrtdx.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gxopxvoul.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqfymmoa.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gponcitwd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgrbnxjc.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvebybncd.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/garnmvafh.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gdikgxrxd.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gbmrguzeg.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjradbhq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/ggbtfukio.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gsmesiihj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gtnmevtib.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgiasoek.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gupknesly.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gssxpgcnw.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqrvkzww.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsysqluo.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbsxuytt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/ggnotqkuk.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gagdwksul.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/grtzhivvk.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptdmfcgj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpvyxdtg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbqfvrsn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkasozyo.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwujgikn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gjvssrcvk.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqgwwjvr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gpdgatqgt.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzolyfwx.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gnyosbhyk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjwkwwdw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsahxwpj.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gprrzvfmt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabnhgnwm.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbxpufvq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkrfujbr.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzkjpbil.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzfohhsr.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqygvmni.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbumljde.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gfbikohjp.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gvxoihkan.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gteksmoqe.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqiwugcy.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grrknkdkw.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweciflwv.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gljjhfgvv.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gjvorfjnj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/glypfojlg.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gbrodczcs.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gmzdlbcaf.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjsxicqe.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/givkpxrmh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gioogtgcf.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjqaamqx.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gdmzcsfjr.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gbjvbrvmy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gczsqgnze.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gsysnporb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gypkehtcd.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/goiwptyyd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/grlxfyrsx.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/ghjyrhnzy.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/goehnqove.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gccibknoo.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gmblavpnf.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gjwglysvi.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpquemoih.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtzxibec.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbqbwkvd.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/ggvhqgqhq.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwcxylzd.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gezziqzfd.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gobcqnizh.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gftilacdf.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gauezsaeq.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gonvqbsqu.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gatlclyyw.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/girhywklq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/govymcrsi.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxfibevy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gogfpojlc.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gptlziien.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpgdruqk.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdpdpdpxu.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcinepdd.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gngfhzift.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gwrqgzrdx.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gmdrqgoii.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gkovyyhhk.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gepvchcvb.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gkvxbmzsi.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxulysuk.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/grxaditmb.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goerrhyzp.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbhbvusy.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxwhkoll.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gxhporrtx.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzionxrhq.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/galojsojs.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmiauvve.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkfgdltxf.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbymgzrv.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjfaycxo.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdikupwh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gayteajia.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gcdpdcuyg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geqvccyzh.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlyhdzhu.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/grebjwscv.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdviimmr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkmloosey.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfldjtalm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gxwrssarf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxsrtdqad.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gijjohogp.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gljnkcvbr.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbudwjwkx.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gaegkdawu.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gsrzfnjet.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gaovohsie.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/guvudhain.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeddlipe.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ghilzsmrj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gieypaxxh.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gfvntbiqe.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/glfftojqm.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gclwvjyyu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gtgjdwoxp.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqmbgqgi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gbarhybqi.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuqkelkf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/geknayxph.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gbohaiqln.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvssvbvwf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gffohqcsc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwefonslz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtqhddad.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/galezltsn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuhrsjhh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqicxpiy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggnhyfmwy.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/grnhkzgut.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gfzdifunt.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gkgssxime.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/grxrmssht.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gvptckoxr.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/goicgalfs.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnylkdze.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrlufkxu.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gvasuisuq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/ghejqkzol.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltaoqjgp.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxnwksed.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gkegxujhz.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/geylqzbeb.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gimneeeht.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpcdgnaj.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfjfzdif.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlwkyaeo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gravtpdfb.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gowfivifd.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsdcvzdk.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvsykqdn.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuwuamiv.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrgvjnjl.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grejwcjgz.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzghpotdk.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhywhpgv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvmtblbf.sHtML


<!-- 参考信息 -->