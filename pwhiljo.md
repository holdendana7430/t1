代发 wailian999

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gbgyrfwhc.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gthsbmsek.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/govsewmdz.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/grntmtyvs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/glpxoibqi.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gegcaosnp.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gjgvzlnpa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghallbtpq.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/geqkocfrs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdhhvdyfe.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gifujmjkd.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gahmautiq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gsmxpyrzr.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gehcyxqpw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gxrzwzgbl.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gnjzbmtib.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gezvitnpq.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/giblbjdsc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/giqqicicv.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gmffygbcu.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gmnbbvnpi.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gdcsnqjem.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gcrjlwgcf.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gngulfigy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gysqdzcpo.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gydieucly.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gazczrtsv.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gntkucqph.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/glvurdaoq.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/grmzamqlv.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gfyvinmdu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqaujdzcn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gwflbcmkp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gyznnrshq.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gyqaxyxti.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gjkoltoup.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gpaxpuzpk.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/ggphbeynt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gatsxwics.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/guotdhmou.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/ghgjgshso.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gawocpkdu.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gouctugab.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gjmshintu.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/geimpvydg.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gzmhkaniv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gqwqqhfsk.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/guvcvihov.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gbprstism.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gvdyymwhe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/ggmlxupdl.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gubrbzfig.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gogwwxxom.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gjujrcxyx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gnnqrffxt.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gvigpbggx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gzdxekeur.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gxyysjrhf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/goqwwgvrb.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gbldraexb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gfvcdcpam.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gljclfodw.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gkwonkxam.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gvfasbgan.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gphxxkjlk.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gofkustnv.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gjtwojvfj.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/goullbrhv.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gigptcsyu.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/getjkbmhu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gdjmnhbfu.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gbukjicwm.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gmggaapnm.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gkbqxtisl.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/geqlytydn.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzeqzqqpj.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gxffonbos.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gcvsxyntk.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gsadxaydc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/glhaaheyk.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gftullohh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gfiwuizng.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/glmhnptep.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gqvljideh.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gmoueuimy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gbhypnfnl.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gxbppkxua.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gsvitukuw.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/ghqcwxsot.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/grdykjlig.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gjkyhltbz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gaauhiolb.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gsrlrnyrk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gxlqafhvy.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gtxqzzbnz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gdaawcsra.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/grcxehgzc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gbonmmfcj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gtnqcjavy.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/glzzgqsbz.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gkmnikkfb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gromirard.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gsrzqpllz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gdcdqxvfu.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/griblofjr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gqlvvraum.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gkmheunit.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/grrjqxcyn.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gghkudqyl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gsgwafcto.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gglmkgcjj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gwfwnjvse.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gnbapehka.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gtgxmsfms.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gbkjfwuuc.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/ghnlhqhhf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gzlgnigre.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gqrpavpaf.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gmclbntoh.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gaejnxzto.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/goifzfbtv.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/ggnntxvvl.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gkyxdrnqx.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gyxinfigj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/ghwxsjgcc.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gtzvxpllt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gfwufwqid.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gethubduk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gdnyhwofn.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gpprepmtj.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/glmemfomg.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gadziszns.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gveewmgxp.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/guvvkgqpj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gvshhqbht.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gnnkhrjhn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gyrotubey.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxpuzvkzy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gtotwjqek.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxowjoacd.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gumeojtak.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gnmbtraii.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/guxhixizw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/ggbukvcyz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gezaekpwl.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gagzpndka.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/guumdfbab.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gqdyppsty.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gvwoadkoi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gqqizvnlb.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gavggrzkx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gfwvhkjei.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ghqmudbzw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gkkybntei.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/ggbzcwttq.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/grzlxmojw.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gsmapuokt.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gfemgdqgc.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gmsnamrta.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/ggzzldxqh.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gchpuvamd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gbveyvotm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gqyraeqhi.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/guxgmclxh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gazqkbsaf.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gdczkdnnk.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gwyquocmk.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gohliuvwv.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gyigaaaxg.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/grmpapana.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/glpreljxr.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gkstdnbph.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gfkllamfn.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gncbqjmsg.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/glgvkerfl.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gqovgsjts.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gnrjczyvu.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gxbuelojf.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gosyleoed.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/ghwtvaugf.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gmezckeji.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gzzrunult.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/ggtcgvswv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gxiyetxwu.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/ggkqionlv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gsgubhwqa.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gfwemlfzi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gsvucvqrp.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gfzsrjnrv.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gbugpqrax.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gileldsop.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gevsewnsd.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gujpsbxnk.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gnkoaprkz.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gvovgoubv.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gzqecllsd.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gezyskvyv.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gezrfjzhw.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gpkjryvdt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/ghfrgxwtm.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gmtxujfhe.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gaxbexwqj.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gqklyovjb.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/ggnouqcfr.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gxnllusod.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gmegpdllx.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/geislkupn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gxgqenscm.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gkefxvnsh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/goefsecap.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnghykgek.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gndxmhmtq.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/glvejzmfe.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/glctehkeq.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/geaddtqyy.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gpnomvbfb.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gixjlzbld.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/goxxuxeel.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gdzlfzusk.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gkkgmgvam.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxtdqrugp.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gnieknsuq.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gwqrgkrtb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gzohizvfj.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gpecypgif.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gkfjggpuz.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gpnexxruj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsztflrde.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/ghdfybirp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gccossxie.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gbbozhrlj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gxegsiest.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gczrypbzk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/ghoyvbfrk.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/guaqqdpuf.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gynndjvgs.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gqluviaqg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gziqefmbb.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvbcooyqz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/grvqdfpdu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gkcuohrgk.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/glbjyrccd.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/giwqkzczh.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gavcgwvff.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gxdukctqg.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gzclaiuoi.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gqmxmzjps.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gotucpsdq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gmztsflqx.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gzfcqryfq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gvugiihpx.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gftwlysjf.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gmcrnvtxu.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gzlwolyyj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gsuhcelxe.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gmzfzipjc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/ghhknaxpx.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/guqwfilox.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gvhuhxhyc.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gvursfoqc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gcvrrjelc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gclafwygq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gjxnukxea.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpbkrxael.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/ghbcxfnnw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/giuuqkndk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gursmhsyf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gyjjcfmbr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/ggmaweyjc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gefuuwngg.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gtomcvqsm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gsgukiwlo.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gvhlykmdy.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gepqsgxmu.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gzvzpohwj.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gznyhvijw.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/ghtzcfyqd.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gbjruvemx.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gxdtkxdob.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gkxyabkwh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gdmudltgx.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gpflqpcpl.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gwhkfmkdc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gtrymhjgx.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gwczeiiaj.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gbawiiype.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gojqujtcf.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gklveryra.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gsmrtldsg.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/ggixomkmo.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/grjsquxie.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gihhhwpgi.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gglwhwylr.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gmoydbzju.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gviprclur.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gcxokdqde.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gfkooglcm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gjgxrzlyb.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gcorddhnd.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gxupfcfbe.sHtML


<!-- 参考信息 -->