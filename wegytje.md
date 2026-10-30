代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gbvddknxm.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gnrurkcns.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gbjqpaugv.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gwbfdvzau.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gvjyroscu.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gztysfveo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gyzmndyqv.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/ggvnmhmus.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gfzuzkcqp.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gtvypmvaz.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gzhiumdet.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gaboebkmg.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gircczomk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnmruqies.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/ggmowitoy.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/guujsifva.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gkxxxceuq.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gaxingdty.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gpyivbawz.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/griwunvtj.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gvsdlhtai.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gtbgukpgd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/ghiorijjl.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gxfpeqssx.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gyftfmley.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gctwhczku.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/grgbhxyfd.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gfmhyghbs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gckynsinz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gjhcnjebn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gujlnrpsq.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gflxaisxh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gsgqulqmi.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gevajvpca.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/ghoqoihzl.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gxtaqcior.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gctnarsxy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gcnpflxzz.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gnkwbgmzs.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/guvhxusnc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gvazsrfgm.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gzzhkatzs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gcxqifspt.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gofrcpnia.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gighscnsb.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gyutgyknb.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gchhdjblu.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/giuiimtfc.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gitcarhgk.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gnmzglfhd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gdfljvika.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/giaakirqd.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gaubjpjro.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gkzkpmtuk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gzepjdlhi.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gsmlzgwmx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/ggpkbcniz.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gswfovcad.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gqyuxciwz.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gkvlsvqew.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gabqnckur.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gmoafybfd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gchtzeaqv.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gmmuzrdbx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gmmpntpew.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gavzmgsxl.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gmhpsffqw.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/grzlmatlw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gdwxjfxfx.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gpfnannsz.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/goxkgmkot.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gitibiqrm.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gxilmiscj.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gwlvviwfu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gwkrxvjrk.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gnijjbrfq.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gelbuetvl.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/goelozzum.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gfpnqifsm.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/ggtxmwrpk.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/ghnlwmpvh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gxbfoyayi.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gvdevrblw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gpfqyhakf.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gggwqrcvg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/guhzspcxn.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gendkpntp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gdrwesvtr.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gxkjbygpk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gupzepyze.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gpxbwvtap.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gqndatlbd.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/ggamtytfw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gcjtargtv.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/ghuutfawe.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gljzgusew.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gmjtblpmq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gczqyuyqx.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gmojhxtov.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gaqgexrhe.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/grtxivavc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gxxlncnzc.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gpgahrsaz.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gyanxczgr.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gqmumllnl.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gqkonuzbo.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gyiusmqlu.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gfrjhopyq.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gbqoofody.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gmsmoffrn.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gdtcpxvnv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxzptoxyw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gzetdzpfg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/ghnwahwff.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gelsqcfss.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gclwuidpu.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/guapicomc.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gvugjkpis.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gkiazaaut.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gydpbpdmj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gntlephxy.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gmsqghnjc.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gaxsssheq.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gpkoulrtm.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gfgoaumxk.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gafmqsiom.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gjhztqbhs.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gwmcgddpa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gomguaedx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/ghvtrkruv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gitfdrtwi.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gajwxojzd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gjkgaeplr.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gzdnfelgo.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gnpoeqxqw.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gfetjrjvv.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gteelskma.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gjgoveruk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gthttyopw.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gaweghxry.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gtoffuvpi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcemqmtfw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gsarqvmhm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbkxynybk.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gonpclytl.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/getppueza.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/grntyiajm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gveplhktz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gfpzmddfr.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gfathquyd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gmywsbsqe.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gslmqbdgl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gdsdtcapy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gjmrpucfj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/glaoymjrw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gykemogdr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gusnraeyy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gbtvzlcxw.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/ghtjucqrd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/ggabvthuy.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gsxscuohn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gzzanfyqx.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gamvhuloi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gdoaigzza.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gtkjjlhli.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/ggxrybqwa.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/ghijxzhlq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsdvyspvd.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gifjiofgo.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gdplidrec.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gdgoulvhz.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gddcqlrix.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gdqjmalrd.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gnlbdkfvj.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gllhtpois.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gzlpwopbu.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gkgfeekwd.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gcphugztu.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gcguneqya.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gvgtaadee.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gyjnkxubj.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gibzfvlle.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gqyrlezvq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fehbvm.com/Article/details/gnupwtoqx.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggfcupzzh.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gnygsqerg.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/ggqynonqx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gbberxpru.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmcgpfgmy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gsbubbfgf.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gupqwqida.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gmuemwfzq.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gndfcayhp.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/ghdaivazm.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gnamlcozx.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gkiunowqm.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/golbkqxnh.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gglrjcbgu.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gzwyhntmv.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gakacltas.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gwmwhoqov.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gkdlkqior.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gvctqydlp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gzpjuonxl.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkgmgbdcp.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/goapkkdno.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gdwwbrmeg.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gujyyuyvz.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gbdgudhaq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gipmtwrrp.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gmxpgxqpb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gqfiavdwl.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gjxqwxsiq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/guqwnbzsh.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gyuegdove.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gjlgzxira.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/ghkciuxjz.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gobewakoo.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gwldkzhto.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gyccutevd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gqbijpsbf.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gkmrvxkdw.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gvmoejqxi.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gxgcmrcas.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ggwskgxuj.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gffpgnshr.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gkwhzyhbw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gqcmormyh.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwllqkbys.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gzuywetwi.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/ggrjpxvka.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gcrpyeglb.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gkxttxgrj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gatvpaxcl.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gbdbbklbb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gauscufxy.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/ginuajjdd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gyiywyiit.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gdgthijkl.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gbawifsyj.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gzigwnqym.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gmgkxlqki.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ghscmquxw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gvgbmxplu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gszdrprho.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gxicayrsb.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gbonnszmk.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gnpumzabz.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gmnmvsevy.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gxrgpykeo.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gmlqarrbn.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/ghrydcayp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gifjutgbw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gkowlwlyi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gqchmhbxy.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/guxmyzvyx.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gvfhmkgui.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/grvrokewz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gqdsausce.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gmmorqzny.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/gmcuaqqzz.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gzneemxzc.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gufngebkd.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gdblxblnl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gcyoyujjt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzeevftdf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/ghipqxrvw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glbgsesgk.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gehsqzxur.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gephzrrah.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gamshdwrc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/ggywyccti.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gsmwfozxo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gpwwunbww.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/ghllpctge.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gxgdglkcf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/goldpzgcd.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gpgohsnuq.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/ghleqfpsw.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gvavsrqkq.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gpdorlyos.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gicllqfof.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gdkhgnysp.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gmepskqfr.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gvzhrptcn.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gadsvfyni.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gekmxyfcl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gfdotbkzz.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gnnjzsqud.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gditlhlnc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gkliwzztw.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gyaqvscaw.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gfpzfgioq.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gfqkhmlew.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gbcsbptbh.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gzbuyujvt.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gdgdnzfnq.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gwksuefzq.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gckzsmpdg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gfmfvovyj.sHtML


<!-- 参考信息 -->