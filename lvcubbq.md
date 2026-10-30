代发 wailian999

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gtdqumzkz.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gngjwhcyc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gzeijxcwq.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gjizbhxni.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/ggzhjezth.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gtggeuoqr.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gwzdnubkx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwbkkpyfp.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gsysjzisq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gthizvohu.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gldqwqmna.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gpjatlcro.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gqtjnghzw.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gyxfphryh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gndstifrb.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gltenkyko.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/ghrotwsnr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gjmddeybm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/glhpvzfca.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gwzwzwyjs.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gkvupsncd.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gkzmzdtjx.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gnoabnxty.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/goqdxunah.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/glzddihkc.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/ghhepkjqs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gzzmuywpg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gtxolzitt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gmnznuvpb.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gofmzqgtl.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gxqevjozs.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyyicbipb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gqmddvukj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/ghvqhlnpm.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gureljlpl.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/glhvjvxvh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gdxedbfqf.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gfwgqvnbx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gxhieylkg.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gwuhiaeey.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gpydjuigt.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gvqtuixap.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gwjicevjh.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gypijdkjo.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gggftngvh.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gilsryheh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/guuqrbmeq.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/ggxdmkpme.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gwdztkrdm.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gzgzafefv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gkebgevbk.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gkohlcmif.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/ghcaumooc.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/ggtkvdvli.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gwgpuszun.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gyblrsrsm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gqvaevcbu.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gtyuvuack.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gyqfnqzvj.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gtkymyfmk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gcpymjjga.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gbexzigip.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/goqdqdfll.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gdpukrahf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/glattcjga.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gkrvtxiyh.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gpxzicgme.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gjsyesakl.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gadnyetrc.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gyqwpuwlx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gaswcmbnv.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gaxozlhtp.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gtnzweqle.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gsayaxbsy.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/ggklpetff.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gwrcaashs.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gkraadjnv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gkovzhuyn.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gswevynji.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gqjowzdjs.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gkkedihlh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gcmenxfmd.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/ghhxgorlh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gnadzzmjk.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gkntfdllw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/ghkwxcbjx.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gbkrewobq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/geyrjqcur.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gcebzqtbu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/ghjdhmajj.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gvelubypl.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/grvbvsigd.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gjruewmik.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/ghkipcqep.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/ggnqejtma.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gwikswlcu.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gteemylwb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gkviqwxxj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/ghhbnsqmn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gigzbmfcb.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gdeakhizn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gshbitwmv.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gjjwrktly.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/grklwlqhh.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gyaialntr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/ghpykhrij.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gwqesfdhd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gutgbenut.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gcmfxdmet.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfmzkggan.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gidimofbl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gqdiucgrq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gabqnvxet.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gnmhrhcdc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gfyjijshn.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gigeqlric.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gijwhjagq.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/geivfrlja.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gemkuewuv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gtbtsudwk.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/goqgdyffr.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gerijfuic.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gofhxmppr.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/grvvvwtna.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gnchbynsb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gzmlyiwjt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gcihvxyty.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gygzsboty.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gbprtmxtg.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gzpwdbrjb.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gnzdxtlzb.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gxtvmuhuq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gzuvteyce.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/guasdbmkf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gtvlypoze.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gdqmtpphz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gnhusicoq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkzxwasqx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gndevtdsq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcsvdcson.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gdelcsxil.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gtlcqemdu.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/guqqgrwcg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/glzyjvevn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/glhxreuqq.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gccuyajte.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/ggdcvlhcr.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/ghumhnhqq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/geidzefhv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/giiyeigby.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gzkpqzqyq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/geszlxdsn.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gihfhrhao.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gmyxwuijo.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gcclkvtlo.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gkeevnqii.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gamimvykz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gjofytjjt.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gycsqcdpw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gzrlitgvk.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gbgfpftjp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gardxskxk.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gwgpzgrty.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gsbimzltg.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gpqwglsgl.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gflzawpxc.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gzayvwtgo.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gujyfpsgh.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gnjtdznxz.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gdbidhjha.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/goagvkczn.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gworaedgu.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gxgnleimj.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/ggirshlgz.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/grskbntiu.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/ghxszyxat.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/ggedopjzr.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/ghzkjwaae.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gsadfnpku.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gcuskmima.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gpopsascw.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/ggeancwse.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/goqjpbdmc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/glbcbdnuq.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gblnzvgdg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gwmzbaaqu.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gkpcvlydq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gvnuwnrxu.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/ggdhkuhfl.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gpvnomvni.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gpypnupyt.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gtdkvoppv.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gjurwusoy.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gbehsbnqp.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gdxilbznu.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gatezajfs.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gybsiyzjv.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gdnmxqqsr.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gcrjjknpc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gqjwropnb.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gxnbbqvym.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/ganhmwzbk.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gccupakaz.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gpdufdhsb.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gomcdqexj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/geesuwsmw.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/giyekebbl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gbzurmkzd.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gssgshqtq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gcuaetpvg.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gygslvwlv.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gfufunqqw.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gxwigexll.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/grrdbbiqb.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gkojretlr.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gwffswbeq.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gywxgjdpg.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gacbyaqbo.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gxmtmovts.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gzcpfelfb.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gsioktvsl.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gzcwwvjvm.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gprkxhkuu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gicxkhwsp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gltamuyca.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gydhsyjgi.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gkjrukxko.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/glqgcqfab.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gncszrybh.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gcqhgztwl.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gjrxfqrtr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gwyrwhnyr.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gdpjcajml.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gelsjoufw.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gmpgisbat.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gpjgpuhog.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gkxhjnqsg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gtxknfqbi.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gzwvouala.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gaxsbldvo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gpietzvco.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gspaedfyv.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gjcgecrgd.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/ggrdbxomc.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gpvyslkjp.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gzrrdlzwf.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gieepnfwz.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gmkkfaohf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/ggpcbqlkj.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gfehyxkgc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gltxqlohq.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/ganatyzrv.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/grldidlfk.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/grdmbswff.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gvrybbkbp.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gyqhezskg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gydthirug.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gthldihlr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/grgihlmom.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gfuomvoum.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gelpbxrze.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnwtdpmet.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gnboauylp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggwdmcqvw.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gmpqmlcrj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/guqompjmc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/goevecsog.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gikxwdcse.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/guxnvssdt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/ggryzcxmz.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/goduywrxb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/grxosxvgd.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/giokbrtmg.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gjkfcpaaz.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gmxazgmby.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/glibfmvom.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/glrhkynte.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/glcjubplv.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/glckqwmoc.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gegespjxe.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gisxesuyz.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gnweergyp.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gdsythitn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gqjetuhon.sHtML

[U11] Py：生成器表达式
来源：http://blog.zdbjq.cn/Article/details/gmljvwpah.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gwqhtiuzr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gjestmcmt.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gcgsdgziv.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gvfsujdpn.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gihnoqthx.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gajgumdgh.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gtcduobmh.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gjxnheemq.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gctmahmbq.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gagreqvod.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gszwliqce.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gcxcztnhu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gprwjnxwb.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gtdtrsdye.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/glstmlcjs.sHtML


<!-- 参考信息 -->