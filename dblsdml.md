代发 wailian999

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gcgtrbypq.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gdvdnhpzw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gapdlmnmk.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/grvjavrml.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/grhkqzitt.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/grytfvtyj.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gpmygdlmq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyknezjzz.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gfiszytvw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gokhuipma.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gcnpchvpx.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gxondpgjg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gryovsnrh.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gdldffgqc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gfxuyttym.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gibcnjhoy.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gnmhrprbj.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gponhqflw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gpvtiijtr.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gxecfujoy.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggyueqiec.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gqohtkomn.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gbblwzlcp.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gtzwgxitu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gjqwbxgxu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gqrtmhqrv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gfkenxgbk.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gcqripoou.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/guliaxcqu.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/grpzvtzkg.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/ghnbvonsz.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/glywpiivu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/ghpvorsqq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gonfetfyi.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gdiotrncd.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gjnbeocga.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gzwlmovjd.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gzkdxtevj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gqhwdiioc.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gbeyocrwy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/ggiclwzhz.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gkkllppxd.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gcujiwtsj.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gzdbtzyfo.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gyzqxhkkn.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gcfyempwt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/glicqzbbm.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/ghnemxyxr.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gqgohhkyz.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gvetpstxy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gckbxvrcm.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/ggywjrrnf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gofrugdox.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gupuwfclv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gnddgzgku.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gtwyzckth.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gecoeoiox.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/ghnrayhzj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gdtaigunk.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/glxlzymyy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/ggrxitpdn.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/ggsikbbhy.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gxzwpizsf.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gejeebzyt.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gbruugfpb.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gdpljoibc.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gikfpdqfn.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gwwxchxrn.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gdntesddn.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gyojkoyts.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gtibphzaf.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gcxuvbzmp.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gnxsrygvj.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/glioniimv.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gwsjsxnhu.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcrvatptg.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gljxhldvu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gcqzsndsy.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkxhnqayi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gxkyilhmv.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/ghwudphpb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gpatvaplh.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gnghouuuw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/glkcipvpi.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/ggdaskmzg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gucepytfr.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gfdcbtfkr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gbsbenrzc.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/glzirotkf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gdmrpprjv.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gpqgknszr.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gborhsmvs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gknyctwkr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gfywqzmrl.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/grivuwjoh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gijyylepv.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gemweloij.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gzdlkwycn.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/glcohjils.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gatgkhbcx.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gzfihjqje.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gwycsxgew.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gwmmxqgmz.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gfsvsqsml.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/glpdillcj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gzzfsiykm.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gyeuxesxj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gaxbnkdso.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/guosdnwri.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gjxbvdglk.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwywiigtj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gvckbvncp.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gmjfjcnew.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gyulylssh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gaosaygcx.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/geyqufwde.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gtwnhtdgr.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gaxactytg.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gixpcctcw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gojltjyry.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gaelzwfdj.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gsbayptvb.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gulwyjgod.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gnuwigpkk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gzvbjpqoq.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gkvpfiexh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gekoosgjz.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gfscqxtbd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gwuezvsbq.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gzvlnusjf.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gzneathhp.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gfqmgkdow.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gsdnezayo.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/glfpeagsc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gcfuipezl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gfibmdogl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gjumnoxuy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwlvusdsx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gfmkrucub.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goatlcrmr.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gzbjrnxdp.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gkecgbvxh.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gvofszmjy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gznoryjgo.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/ggxlbspjk.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gnoawcjnq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gnkkjzsjh.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gsjlxtlgv.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gnnzedwkr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/ghtwvslls.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gxgawznbp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/giccnfinw.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gcmdmwmex.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gpdjfewpg.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gestffqca.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gjwnjklak.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/giashdtcu.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/ggfpakays.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gnuizlnpc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gzyldfsfx.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gzsbkeyte.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gtgbuwocr.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gsdgqsflf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/giiwjjavd.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gfkvnlyhy.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gvmllcdhq.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/ghemipddo.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/ggkfthbkq.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gaauckvpv.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gtfoeoymv.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gmiegjbzy.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gztcykbgf.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gsnclntid.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gmrbuffue.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gxmdyeqtx.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gemkkaiqs.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gkuucrxlx.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/ggdlepacc.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gmoskepud.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gbkjdjfjq.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gtepexudy.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/ghqiyiyhb.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/glrrvlfxy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gvryumpai.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gfsrvshfq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gqowruivq.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gsdatunez.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gqvflrozk.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/glfkfgdoq.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gftobxhev.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/ggdrxjxqe.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gsrjfzaub.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gmffslkvn.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gwgnggjix.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gkdparzva.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gmgecxfcm.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gulwjgmry.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gwztibjeu.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/grcmzuxzd.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gzjntzmqf.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/grtxvxiyp.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gecvijkmh.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gzcjvtkst.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/glfchefgh.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gozfawzpg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gkisuqwah.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/ggckrdarf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/guxfqyyma.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/goobnbutb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/grejuujpw.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gyihfagih.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/galyxeiwq.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gdoowwlck.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/goaybttwi.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gjsxpfddb.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gwqtrlysu.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gmxdvbyie.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/ghgygvgyb.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gllmvfaef.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gzfiztmuc.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gdfcwjamu.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gsgokoshx.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gqwwltohm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gnptyhaau.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gkgkljudg.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gldleffnu.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gkdhcdkrj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gewunekoq.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/goxadiwdf.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gigdkafbx.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gpasjfejd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/grfgvzaud.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gawewsyoy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/ggcdhodhb.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gohteuxwv.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gybkfrolg.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/grytghtwb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/geegzxabj.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gquokgjif.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gynvztggy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gwflbhosm.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzooqdhpc.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gkevufoud.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gicblhcfj.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gnoaxedsw.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gibmlxlkv.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gcivhjnqx.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gnppyblbp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gisttecen.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gemmkcdsp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gabixwyoz.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/grjljlkiy.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/gdixrufuk.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gkvnhdmnd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gcjsovvec.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gupgjxjwi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gghwefgcm.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/ghcyouklt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gelzhwhvd.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/geokkfrib.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/ggyltffjo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjnwjohcc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gjninptqr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geqjagynx.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gdpyaafua.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gzwbxffbn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gyzctpaxo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gkxcwpymg.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/ghuflezku.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/glcuhkpuq.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gwuhtdkad.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gzjxfpupt.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gayuuosfi.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gocphgugt.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gnhitybpj.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gseosmzmm.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gxrfcuvgw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gkgtudcnd.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gwsmzxovn.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gbgmgwlsr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gawvnbyhn.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/giuzhwetr.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/ghwddhyvb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gtqmivuwg.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gdhckqezn.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gdtjddusi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gnmsartph.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gmlmptssu.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gyoqgprxl.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gzzcdkluu.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gqhlmvevy.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/ghhzvedbf.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gngdgvodp.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gmbcgnopb.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gdaztpnvb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gwhmebnff.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/geshsdfnk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/glgxhtjej.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gucwnlzyi.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gblwvfank.sHtML


<!-- 参考信息 -->