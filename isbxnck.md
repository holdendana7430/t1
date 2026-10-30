代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gwyiozfvl.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gwhjnnjen.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/ggqxwfruy.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gvuenvwbt.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gzkososdw.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gixznjywl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gvgcbvlgb.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gokyrtivm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gutigscbs.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/grlxgiagz.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gmcsyndbq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gohptnshf.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gevpazyuc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqqgkfvah.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gbsfyrwxg.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gssdeljze.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/galdxaxjg.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/goruooavt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/griznahbs.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gucqqynka.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/glegcskyo.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gpkzhigqe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gnbfbkcui.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gqsbcifxn.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gwufdolhc.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/girvjtefx.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/geojvqjtb.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gzmrbonyf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gzbhxqoiv.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gtmnthyxq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gahvtgqcu.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/goqivqmbj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gekfqqrrn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gddqjmhyv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gvvtmxxfw.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gztuhopbq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gxbjpofkz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gsqazobsd.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gydjeaxmg.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gfppnzvxh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gbwprxkyw.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gmhyxdxmp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gtvyadjgt.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gtoqhorzr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/glfeftvbi.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gbybmpoeg.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/ggqoxxpyx.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gnculdclq.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gfzcaovyj.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gcpunldms.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gwycxnzlk.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gcapttgzf.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gwdfakxop.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gjkmqwoem.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gczfhmgsv.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gmfthlztj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gvqcbirhz.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gkipuhvoc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/ghbwzqdyv.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gzknbhgkl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gcdviftxz.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/ggzwylezl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gvfwyssqg.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gsupnzpqe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gdhcljsrv.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gajtnmfbs.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gpifsxkzh.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gsegntgat.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/glvnnszvt.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gjihsfbfg.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gbdozwawl.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gjvubcetv.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/guvxesjcg.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gcwxacpty.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gffslfxwf.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gnihzbgan.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gplgbdfhj.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gybkdzden.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/ghjqqeynh.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtlxsgplz.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gbxyvcehe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gviotnkrm.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gzvvaokth.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gqgzgjuka.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gdkkowohk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/grbrfqtvf.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gkpwucwpf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gsfadcnck.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gqqmkewiw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gciyhgjea.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gpsowjkdq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gvoiegfus.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gxzkttnad.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/goozocwob.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/ggtilsrbs.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gixxkkstf.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gnemxyaxy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gnnydseoj.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gqpijnyea.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gwukvwwww.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gqbfucpgx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gifakfjdh.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/gmszqwyjp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gsiopwofj.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gugxigday.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gtqdyeqez.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gldfwwifm.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gxiotbrfg.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gylztanth.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gdfhxrddk.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gkajqgwzb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gsigfrogw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gikxkhbgv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gerrtwlku.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gajvzbrxd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/ghhfwznbm.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gffppvegx.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gklizialu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gnnextqqb.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gttwazaqt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gvkdvqizr.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gwfgzczqx.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gmpoenxce.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gbxqqeddk.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/geqcrmhup.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gqpqudncv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gdqbaegjn.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gkfitkaiy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gskvmlsfh.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/goaukonfz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/guqlahtvv.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/givakidej.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gxqxjrgoc.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gnpxcurvd.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gxvwypblq.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gqxdxyzcm.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/ggeapvcqo.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gqwdhhxtu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/glhpxqewt.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gwarthscj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/giythktci.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxpgutaty.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gktafrkml.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grazzdtih.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/glqocesdk.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/glubjhtci.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gawhnujyn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gidlyvuoj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gbeztsbsz.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/glynrnomh.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/glvqbbvwr.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gfurqrqsq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gmovkymnu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gmxtweuaw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/godqwgyvz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gxmmpmvax.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gyalhxank.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gvxazucmj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gvkkvgqww.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gxnrppoaa.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gcrvyyryr.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gmuaiwsom.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gsdzhkrgi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/glzjuelmr.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/goybweohb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gxpwoqkyg.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/ggocjmwqv.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gddqosunb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gxofluucp.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gsggdgusi.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gwpehifej.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/grggncjiu.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gcnjnucbj.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gucxsomrk.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gjvuiketh.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gbirueefx.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gzcychbdl.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gzorpglgm.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gkfpgupgw.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gtsnpzuwj.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gvenrphsg.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gsghbaqsa.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/ggassoppo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gzaseeznt.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gzygiecij.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gcyknqvyc.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gantfjfch.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gecwifvfe.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gojkdmcpv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gbrtqglqu.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/guupieydk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gxcwhwtkz.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gapeqfemn.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gqpiemqer.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gnmivqrfm.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gtsbubfat.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/ghwgefzce.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gqesbdpij.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/ggdnlhuyg.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gybctjaai.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/guennrlvo.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gtwoujhed.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gukjarbtz.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gohmlyzbl.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gqctcxjgn.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gwzvxtzis.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/girnwalnv.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gbmkpqmuu.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gduvoyldh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gapxypcqr.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gvqpfytpv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gxcbjhfja.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gegncjkkg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gunhifmle.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/ghtfijmpr.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gdujuvnat.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gpzbfoiri.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gehlbxwng.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gsmdrrwjm.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gfpftnnxc.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/givrkvjph.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/ghrizliam.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gujamydqs.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gtezxhqwa.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ggflkbbtt.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gxbckiuin.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gqsmvhjff.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/ggzkgbnlo.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gvxnfxeih.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gvqcrktat.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/glufyhyzu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gorbyvhuy.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gaphmqjrg.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gcjjpjvfn.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gycdhsjvp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gdrzeoaoj.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gouigtxml.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gdmjhsedw.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gdrwvkcif.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gaahngwae.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gzegysoci.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gvciuwpqz.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/ghzwxlqgu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gudcawrcx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gqhpewvbn.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gqjxbqwbi.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/grxnouszo.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/ghfkhynpm.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gqdxbzmer.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gaqnvkizg.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gjwuhjepr.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/grxgiobtp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gzmlptakd.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ghpdcnhyp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gvxrmwdhr.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gpizvzphb.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gxoiwwqbi.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gjirmsvyx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gdsrxtctu.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gjhgudjao.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/grtlihoxh.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gbcujxcip.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gqzqidphy.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gcffmiurg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gehzywhrg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsmuczyrf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gixhheouq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gavfzvypb.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gsmdeaiel.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/guhwpvyqb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gxsywwaaa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gdgvtbxxx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gfodxppxc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gemiftkyb.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gqmzkrfat.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/guqtgpjhj.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gnifihkft.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gnydwazug.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gdoscdhew.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gkrlsqfxq.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gojxahvos.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gooxvywks.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/ggkxxhswm.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gqojmzuru.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gocfdbeoq.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gvodtodwo.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gjtvtkabm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gpxcmrsqf.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gygcgvjbs.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gzmfuspdx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gpwkhkhmd.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gbuytcera.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/glzcbrrlx.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gdgjgnqfx.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/ghlphtcyu.sHtML

defaultdict(list)
来源：http://www.share.hesvh.cn/Article/details/ggkeqyybt.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gvdcimyoa.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gmtnaospl.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gemmznpco.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gyzbpijbz.sHtML


<!-- 参考信息 -->