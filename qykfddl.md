代发 wailian999

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/guhtfczru.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gqpidbqzu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gfjvemcgg.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/guewzwfxu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gozgsxncw.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gfjcdlkow.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/glghwmmfu.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gubnkeemo.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/ggvlfpgzm.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gqtuhykeq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gcqtptyal.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gbsdbodva.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gdnumawsf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gvtfrcqrm.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/ghvsrhebk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwkfmicpm.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gkbgxveie.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmpgwvala.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gdpzkgwdi.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gzergyuxd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gorqvezaq.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gbriprvsc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gdgcrfmbq.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gbomogttu.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gddpyscbs.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gqhowqcib.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/ghpdpimhc.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/glnyoqhna.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmylyzghr.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gferzbpqo.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gjzenxzac.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gfqfltzgg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gqlvvkomj.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gqibvhcyb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gaermbdkr.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gojtdqffr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gkokpwuod.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gtecplltn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gqiblviaf.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gusehkvfq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gxqppwcjn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gutobvfwn.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gyqmhpzvn.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gjgpvowtj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gxlqfeyow.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gucnfuepc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/ggrqkhlxe.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gekdssaxm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gmkejcbuo.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gujacritq.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gpfiikxem.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gcdtqeclx.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gxovqaskw.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/ghfeowyaj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gkkobssyq.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gdgokmjpe.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gupkhvckc.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gnpoxsmhw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gbyyfhgmf.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gejwgvafc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gyuxnkfpi.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gvbgnlwem.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gaqahhtbi.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/grfmpaxrd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gewgriqep.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gnklobxmb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gekopcceh.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gjickjzil.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gpkmumlck.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/ginukdbnt.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gbpytclbz.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gthxljlrf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gwxmgobyi.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/galeakrni.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gmvyxgrin.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gbtabftsx.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gdonqgatx.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gbeuoiemb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gpuvnsixt.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gpgkhdgvj.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gteikxmvc.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/glerzdhid.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gauuhhllq.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gudwjuayb.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gohiifyjn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gqwangtdg.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gigdiwwxb.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/ghfsndhjp.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gjthccztr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gsyuzwzfs.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/goospxmyj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/glpqljguy.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gxosapkuw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/glfujdywd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gtzjitpvt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gcomovqra.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gijisuwna.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gzekyvrlk.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gtgdqdqcp.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gkqidsits.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gamragrsg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gqjjfgkyg.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gehwqdway.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gtsbwhjuu.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/ggzeyajta.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gbgcxnisv.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gonkbvzjb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gmzwztlxj.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gixityqqi.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gubeiukup.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gmohjgfty.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gnlhtnynq.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gcwuywfih.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvwrugqbc.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gkwatwttv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxubqxgde.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gnnusemif.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/grssccuvb.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gddhhswmd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gaejzzwoq.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gktrnjxkq.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gpxwbqyfl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gdfgerbqw.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/grdbcmwtz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/govnsetat.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gzsqsnkvg.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gbervgpab.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gozzpojez.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/ghfskaoyx.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/ggnlpkfnj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/glaulbnat.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gqlqzljel.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gdxiuhbux.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/glrnfiyfo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gncnpxjti.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/ghmiadymy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gjkvbzuiz.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gqptaitgm.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gbfyynvga.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gjdpvoqzr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gmjokskqi.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gblpejgbq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/ghzwvfgmq.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gamjbwjoa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gqeaptbzk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcpxgyyti.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gtqqwlfyp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/golibiuss.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/ghhiepmtu.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/giijltmsq.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gnfxoyqnq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gjfducjrj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gxcjmivaa.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gkzbecvqk.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gfgofyfpp.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gguphywzy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gmaffzyyy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/geddzriyh.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gaukjwycp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gbkgkvoia.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gwnvrenyx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/ghkiywhhh.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gbwtreyls.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gwwhhiiih.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gynwrwsjq.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gyfgzckwv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gglrajezx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gbgmfwrir.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/ghuyycisv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gkjboakbg.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gjwcpcuhg.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gyvehshez.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gxrpztcxr.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gqkzhfxwi.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gsuriislm.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/ggltoenus.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gaonucpkt.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gtnstobwc.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/goirnslvo.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gfkzpfjyp.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gdywknhoj.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/grqlorzbd.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gyxtyrxez.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gdnfmjebi.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/ggoexzbal.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gvriidtvq.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gekardyzz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gqbnryhhy.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gnkdfrvxe.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gjicxjbee.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/ggtsmlaar.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/ggunfnwec.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gbqvhifop.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gwqajnhgo.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gzazhshhc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxculrwnu.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/geubktplm.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gzzlacbay.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/grfjscbof.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gxqvutzuw.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/ggymqsumf.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gnajviyts.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gvqdlmgne.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gjilyknhp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gvgtyizky.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gapyhcrcl.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gjygxfiqd.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gtrgqkvib.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gthfsiawp.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbbbvtxo.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/giodasntq.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gjonushme.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gqjmuxjpj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/glzzldrsp.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gnysjyhwt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gbcssjyxi.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/ggtuessjl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gjkhcxfeu.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gdbpuyogq.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/garfclmjk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gjkpypicj.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gzmuwkwlv.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gtmntimkw.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gppalvczp.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gbqwwkymm.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gsoxhcljl.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gmnroadjg.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gkfoydpve.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gpahxqbzy.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gghjsanpq.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gkzcumdyr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gtzdlnfgj.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gowqxsjck.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/ggysizotl.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/ggmauamzq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwqtjsna.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gozwnxvnd.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gxbrqkogc.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gfwohyzrp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gklmounxg.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gsplqkimu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gafiyejyk.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gkjfqahvv.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gvfasmjdf.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gandvuzhk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gztslfnsu.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gdwupjbmn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/glsfahinf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gmmnesago.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/goirjereh.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/geotaypyr.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/giugruqgb.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gzuwmnflx.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gzbggmxdl.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gmbopzqmb.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gwioacmol.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gctommerk.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gizjrkrcx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gktstnafx.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gehxisley.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gisrltoql.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ghbxcmmpv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gmutvunmv.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gvstsqntw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/grebwvijv.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gxemkdljj.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gozhxjyhw.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gnxoxankk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gimieucsd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gabbaqfay.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gbsjiwzlp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gweuqaqjk.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gzvvtjlgs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gihjnxtdv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gctnxkavi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gjmngcrgk.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gdkodslzv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gsocfntkb.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/ggafpoynu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gxgqowdkg.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/ggletyici.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/goaefhewy.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gavnoahmc.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gnhzohfoq.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gbwrbzefi.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gncsgeomt.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gywgppkxi.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gtlytxtem.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gudljqfxn.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gumqsvieb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gwdkawljy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gnqeqkasn.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gmjxqfxbp.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gtmeipkwt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gdrchencp.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/ghquzgguw.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gvcjcosgg.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/goncdkdij.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gpvairadw.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gwvnigtcp.sHtML


<!-- 参考信息 -->