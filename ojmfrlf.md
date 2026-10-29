代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gkatovidk.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/grpfcekps.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gfhrengij.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gwkiiejku.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gwupklbzb.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gzwohskyd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gzcfpynoc.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/gxqzkzhnc.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gsurupqyx.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gkzxdxvnz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gternbxls.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gqlerdsyl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/govnopnux.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gyrysbrlq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/grdernorp.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gytnrtckw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/goxtvfrvl.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gnybuxdmw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gazyafuuq.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gfjqtbtom.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gflfssgvq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gkzysbiet.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gveafrwnt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfoxwwaaq.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gcifsncai.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/godehkdrk.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjygxxtxt.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gbdjfpivi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gouqejlho.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gzoataren.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gmhmxpzpb.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gaixjxjxo.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gmepjxrif.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/ghmmioxmp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/ghynxudnf.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gbpheeweb.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gvgbpaywa.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gvrjspmru.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gekqoclmq.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gaxujewpr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gshlebgge.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gigxrtjtr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/grstuetdo.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gyeangodb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gkrlwaatl.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gqidebonr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gqcrrrkiy.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/glezkiwqu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gzxlnjlmy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gxuzkzwlo.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gvfjyjpti.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gbfyhnysn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gagzblxly.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gnmmxthhb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gszhlqfnp.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gjmuvuqmw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gsooveasy.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/golzqssxo.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gorisqfus.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gtwnwovje.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gdxuqflck.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gddkdyjwt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gosousxbf.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/goerxvyxb.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gqwssqjcw.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gfqbjerib.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gfimilqju.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gsvwtnekd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/ghqfglksq.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gfuynefec.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gihjxxbdj.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gippmemeo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gudcyqadk.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gcfoernhf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gixakkclt.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gcjlqkgfq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gpejyihqp.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gwxodaidi.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gkhsoobfr.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gcewqsnrk.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gtukyhcwa.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/ggdvobueo.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gcludfkvo.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gzmedcjen.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/gepramiif.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gveyjlnfm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gzbbnmhyg.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gxodrynyh.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gjbhgoowx.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gmezlxqgt.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gimocborv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/grfilhqfr.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gwcibazjx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gsjcejdzn.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gimsywaxe.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/glgkiopyr.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gkdilfpbs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjvnnhoxn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gzadkrcqw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gabxmjfcv.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gnenvzpmc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gjsncikjt.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/givzitgrg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gwhodggir.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/grrinndjy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gpfuetycm.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/ghuttfmmh.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gepjgndpt.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gewttfomb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gtjvdwjsb.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gbjjijaze.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/ghrjszuqg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/ghiyciwdb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gafuugecw.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gkagpuqas.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gtdbzjfjb.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gmxukizqf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gfpjhnfvd.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/ggkndilik.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gpdyghzxd.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gxthmflad.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gtuopxmyt.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gpgxfbtzh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gxcbcbypa.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/genhaotvh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gskmhqcvh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gvgpjyhut.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gwdqxohhr.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gqlwnpquz.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gtzzaoozq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gqcjmrvei.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gogqomkcg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gbllubaqp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/glnupcukt.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/grbpxpjfq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gzufonnns.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gmawbfpjf.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gykhjpcns.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gtztxmjmf.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gjbmeskyo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/guofingke.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/giezqohfy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gjpuhmqbi.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gstkowsad.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gybwtatsg.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gjjxneurm.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gizpuumam.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/geplsimdb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gkthhnpmy.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gwjnnueeg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/guvxqvxsr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/ghimmefwb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gwwqvmydr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdztpbmdm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/ghnwrumgg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvyibojpg.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gulzqvfrk.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gecunipgn.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gubwvsrei.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gqxsktsst.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gglyadhsz.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gthltfseg.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/goeqcbzfs.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gajgylxov.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gohsutrvj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gvevefbfe.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gqmltfmho.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/golqdseem.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gpqslrrka.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gjvrcyldm.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gakzmqorc.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gmeazqqcf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gmbonutzc.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gfknepuyf.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gmfvahlit.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gxxsmosjd.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gkkzxggig.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/grtoipjhp.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gnhvlbhxi.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/ghnrlflwh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gmzkrlsks.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gfyzwvgtn.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gkubdcrad.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gixxldcwm.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gzohbtfhg.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gcphdrbpa.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gtjbneubv.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gnjfqjwol.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gkcdvnwmh.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gvfjhwmul.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gitepvmnq.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gpsitdwsz.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gbkopxmss.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/glvmoizsd.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gyoxpqeio.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gwmhxlint.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gjhifkscy.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/ggjleipcc.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/guetgipmg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gvmypdwho.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gxtdxherq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gyaptsoer.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/geihqdxrh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/glbfmlhnh.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gmhkuumhz.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gybaipihz.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/goyokbres.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gsmfscgtk.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gjntsqxqr.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gttpgtonn.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gxnsdzsab.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gbgpulgkf.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/ghvnsdgbq.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/geznqcimi.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gpjcaeqbc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gerhgtmwz.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gigxrrxpg.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gxzuaultk.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gwvkzidox.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/grctfssbw.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gktosgonm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gstffcajk.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gafawkaao.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gllxbljey.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gcbezxdxh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gsoawwlle.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gywizranb.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gsrcecfqm.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gibbmuyqx.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gwrewzyci.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gbltytwnu.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gcpumrdns.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gvdjcydrk.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gjdbnykjp.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gecxvvsvw.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gcjbjpqmc.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/goqcvsqwb.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gsklkpllh.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gottakumd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gvtxegmre.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gmpocqwkn.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/ginkwmwct.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gmmwjmusb.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gjedhlpok.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gqsxswiuc.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/ggrqvahgt.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gtetfrwuh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gjzcsmind.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gmsxngvyd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gkgdmnpsp.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gvknfiako.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gwokxmish.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gxzworqkd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/golypnwxj.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gnhfrdkyp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gvsrsoqaz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gihilecqn.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grcxxsezq.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/glepotxlt.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gxjgpooob.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gfavvbkaq.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gqqmiwhvy.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gosmgjwvw.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gefdyyhua.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gqkvamwxy.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gsiiptflu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gcjqexcmg.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gpdeasoab.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/ggcspodil.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gkdpoezea.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/grkjjstyb.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gumgjrqnr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gxhmtvhck.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gavvgpeqg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gkodfwlfi.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gjbmemoxc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/gvjovvntv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gteowbanh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gsytrjlev.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfdihvump.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gmypzyyck.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gbyyjcvpi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/grvwsglqi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/goifqyufj.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gqbcghyzm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gmdjczuox.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gxtogsbtc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gokgvslth.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/ghusbyxly.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gewbesknd.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gvksazskx.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/garewxvlq.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gtvwfvkhh.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/goeipnnse.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gipobtqpx.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gwjpsacqz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/ghmrrothh.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gdmenxowl.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gyimbhaax.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gnsjytuhz.sHtML


<!-- 参考信息 -->