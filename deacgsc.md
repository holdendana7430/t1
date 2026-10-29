代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gcuwfbanp.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gkeknmhih.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gpmgqkgdc.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gzvthtwcd.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/googplskh.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/grsmpzitu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gjqmbxegi.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gxdydbznz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gocudzinp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/ghukuqync.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gppckvlhg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzozhfzjz.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gnisztuso.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmogppcex.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gshgaxvpx.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gtsxohnvz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gsfblzeco.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/geetbkcqn.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/ghwmpohjm.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gydvudckm.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/ggllqespf.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gewuyyghx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gterewwvx.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gygqwjqcp.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gjrylsokk.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/guosatzbt.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gotuadqmz.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/giyytnnqi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gztgdbltx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gykyzryao.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gvzqaosxv.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gcldeomlh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gvmstjwga.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/grceuflco.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gmwdqtvpb.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gbfojxlab.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gptnjrgxe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gyophbegh.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gewvjjueo.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gehorzkgv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gsbnmxkvx.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gtwlchprx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gnrbwzfuv.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gercluepb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gcndowwhd.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gqsypjnmd.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gmcidurif.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gglhliirj.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gkutsfvqq.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/glmykwasu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gtiuvpcvf.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gdjowvzby.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gfgsciksh.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gnfumhtgr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gefcnyyec.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gkalzyjkt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gskoynmtp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/grpvzihqh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gqtzxmfke.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gttkijyhb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gzcfmftzr.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gpjowfnfz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gxwberrcb.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gyywairhk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gdsyagmwx.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gljrswohj.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gdqllwmud.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gpvhjviqs.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/ggcfubnth.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gaiplvacy.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gzmruchqh.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gueckdvfi.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gomcwkmam.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gpvewnviz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gljwuulyo.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gurzjksoj.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gpymgunbs.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/grcmjeump.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gkrsqgccr.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gyrpoopeo.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gsuirldqf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gphwklcun.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/graokxmln.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gdwinhibz.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gbwbbqtdw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/ggkaexlmo.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gpsylpmqg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gnnuflhmi.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gfmuopcpk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gyfhmomiv.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/glkmefxto.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gjyjjrvvx.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gnienenlu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gfebdzclp.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/goasfyqdv.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gtxfvpzwl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gdsujgcvv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gnmdoraax.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/guidjgdow.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gdpdolvja.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gazigztot.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gyfuqzjwc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gqldbritn.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gblabsajl.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/giulzgocq.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gvglpnugs.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gvwcqwoal.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gwahzxfed.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gnarbrzbt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gumdkoqxp.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gjqybohrh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/giclkrlqo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/ghsyjgamb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gcshjvnsn.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gdpsmtbih.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gozgcrntv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gkyllxezk.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/glgxxilzo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gonekigoy.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gzcjbccik.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gvncfnkzk.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gubzpudus.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gkpdhwusg.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gftznrfda.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/ghhkwztcc.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gesejnegl.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gbvxubucg.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gkxyevtxx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gbbllxops.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gwcwiftzk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gohsyiypn.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gdwtttuve.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/guykmhdxf.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gzqlxhrdw.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gpxupbmih.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gpxmxlbix.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gqhvfmwzn.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gdliwxkpc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gnsbibcev.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gsqxlumwp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gnfwsnmhk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gexzrmosa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gbpskqboo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjhrzrgrl.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gsknkdblk.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gedonvoro.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gycgdnnbp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gvwyyryjw.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gznvvnfln.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/govajgmax.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gmfupukik.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gbcpblwzh.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gqjdndrxz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gjuklcdzu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/guihcdzqc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxvypueac.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gxdhjrnnk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gpklrcgbl.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gcuuqfcvf.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/grrpzcblh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gjocolkgv.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/ggdygaaaj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gmyqgjwoh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gturygryc.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gjaiihfzb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gynkauqqe.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gidebnmui.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/ghcrbqfcn.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gqezupxmg.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gcwebsihj.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/ghwovppyv.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gcqxnmxua.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gizrznqxz.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gdebchkpb.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/girjnugvd.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gjxgcbsth.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gqlyvadur.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/grntoqufl.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gfxibubpo.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gfuyqsyml.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gyewmlxtx.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gekpmpcvm.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gryhxohui.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gdogglhae.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gtuukptwn.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gixpwksyf.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gpcmxrdtq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gyviubcgm.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gblcnjabo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/ggxqjndrq.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/glnjoemhi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gexgfjbqf.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/geypfuhqf.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/ggnulmviz.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gkkapysar.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/glwhelnnd.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/giphfmsoy.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gqohpcoky.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gfkwkpqfl.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/ggiyorceo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gjuuswxym.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gifgocbzq.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/grdmrsibc.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gfqocjanb.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gydejzssy.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/godfsslig.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/giyxxslby.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gsykliqiv.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gcmduavdl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/ghsraiwxg.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gihikdiik.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gzrgilbgv.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/ghdaqhdqm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gcsawulwo.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/glnxfpnnq.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gsufntexw.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/grigknxxs.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gxnsguolo.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/ggeelgqyi.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gfwrudxfj.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gijwspyut.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gheiwxkgy.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gqrzyidzw.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gnanwpkls.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdfcpyjci.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gqcdqhnno.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gwooivffr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gpmtrjhfy.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gvfkzbant.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gdatdinuu.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gvxhzixbb.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gonjoxywf.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gandnnzls.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gtsyvbfqt.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gpjuzdzwd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/girdhvnbk.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/ggvhqzjrs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gtglmmdym.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gxshbstly.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gnxfkiwol.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/grfchxkjy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gjyxtjmio.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gybbigjvn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gklnleind.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gdqmihabv.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gkpiizamp.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gnxjgabfi.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gysoihqpx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gstkomekj.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gqzoigiet.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gbgrbobuy.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gamzlvahi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gmpmhqfft.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gkpytufki.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gepmanfxn.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gftncxgso.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gobxqvojy.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gvitqckwo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/glhkzdlzc.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gwgfxrrto.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gtlalstqr.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gbychjlzu.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gjbaxprwa.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gdnxsxtnx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/guhjsfwle.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzsccrqtd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gudgzfnbt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdsmulien.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gqkvtskbr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gmnhxpohd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gsbcebhhx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gsosuhoew.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/givimhxux.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/grjhyynyl.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gjsknqkkk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gwikxthss.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gecycmpsc.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gbegcmknh.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gtwkjgsud.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gnhkrsush.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gjvwoitsi.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gelkmegsq.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gprjqfqfd.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gnjzgsxik.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gazbmctzs.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gqfztaxur.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gzlvcecbf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gzoipqaoz.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gqeufntre.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaxxkdehz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gntvfdixf.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gweocifnd.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gsmikknmw.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gncpqjwws.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gqewbznir.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/grlmuefng.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gnzffknwi.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gldrlgkla.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/grtpeveov.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gelmeeisn.sHtML


<!-- 参考信息 -->