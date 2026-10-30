代发 wailian999

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxlwjshw.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/grnwrfwyn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gbijdujba.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjiacyuy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtobkaekc.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpgmfyezm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhfyamgo.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/ghldqsmcy.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gekwijndj.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/guvixckkp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrrhhxql.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gonocjugn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwecwntge.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gofnwujkg.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gqgjcnmfo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtgorbdw.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwntjgfl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtrckdco.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glhgppzoi.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gmyqtrhba.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glwxzodss.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/glebdlpms.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkkiilks.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqqguvyk.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmhsvbnh.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gdvejkzqy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrxrmhru.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gacfvotqf.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gfxujdfvs.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkelnoiuf.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gdcfgilkt.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gumlmavon.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gkfadgure.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyovzihsb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gbepuouxt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkwtbwvf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwzfalyi.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwgszvhq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gpktdylvk.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gonjynigp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gisihsneh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhlybggl.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gofcmwnvg.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glmysrzuv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girqlwznm.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gepmvbiux.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/grqspjshi.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmornjcd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gckmqnqfy.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscrvyvsq.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkanrxik.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzlevyhe.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/givrktmur.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcrrcgcin.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gmkcqckjs.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geusjcaxv.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gghyecbif.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gturntodz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmhchfbc.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmjjufvm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/giwiunbsv.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/glvnmhanl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gypiwrdvr.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gopzsvvak.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/ginflgvhx.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbmqvupw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gtcyvdtoc.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gamrvlotu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfveznjr.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gejamrksl.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxguhivcu.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxcojtbe.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxvndysj.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpicmmrhw.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gxtritkmh.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdyntarpn.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gshqhfglg.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtxpqvtdr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gooyjyxor.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/grqyofdlt.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gbrcqhvkx.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegqrhjhr.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdawotcre.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglgzgurt.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gwvpzbjip.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwaqztzd.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/glmtlaghi.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gimszzqdk.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gonlnwkkp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpizxrzp.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfehqdmsn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gafycphjr.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gqonmolel.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gfvuouwex.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwicgtab.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gabjdmmsx.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gbhmrekaf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvbzpsnw.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwaudzpz.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gvpjaiqtu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghccyagau.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gxoqhlkbm.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gxndraayt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gbwmvwkpv.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkdqegxbe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvdgcibg.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/galhmifhs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwckmtthy.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnbfkhxa.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gatfzmesd.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gpzbchasr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggroerttn.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gkrimxbsr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/greuiajam.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzhuawfl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefxistlq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ggghmasbn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfppuwzzi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhvpmnlm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzxwndxw.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlpktmqp.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqiciavh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoghivtr.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpsovumh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflaxalqq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/genwmrqlk.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gpyxznmmt.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/giozwlifh.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfyuwqae.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gzynbityz.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gomlpmify.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgqmqkcm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ghzcvmjyn.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrtxildj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gabutpheo.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwumoxvj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gixmvpijk.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsygymsm.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbspkbknv.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gmujleels.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gjhgagmeh.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gmnagvaqe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkuiqnze.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gqtjkuoai.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gdknduddn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgpuuvyb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzroxnrc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grzbrbxxz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmzwxbczq.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gzuxcurwo.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzydqdph.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvckkaulp.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gjacdqrrd.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypqvtvqy.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/guvfryhcj.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gdpdlfjnc.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gfkbwxxcz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gsroxjyyw.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsltwgpfb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpsxtosf.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkvkiqzd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcmsjwyi.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ghqjccfkf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzecmkqy.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gakrbdpiy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gknivyxke.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gujcltpeg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmcuiviv.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gvnvlmfms.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmjodpjc.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzukzwsbn.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gzlfgnkja.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gdntejryk.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gkltzbuoa.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzxndhap.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gbxypejmx.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/ggvrnjfmi.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfuxyzrf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssbvbjwf.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhhfamay.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gbyszgbhz.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvytawnj.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyyoactl.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gylozxroa.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gyisisxih.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjllmhvj.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gtiienlzj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gepkftgpp.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvbhkcel.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrwpggdi.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmjeorhx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxafuocju.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqsovofdu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/glabhjokm.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gtftxjmto.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfyshmfv.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gmjvulbft.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gwpekyulc.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/ghcamhfgb.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gksblcyly.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gzsnkijzi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtatrussw.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/glhnrjxjw.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/geprkcdbx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gondykwmm.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvnpjsin.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gwqapugfj.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gaqtnsflz.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmdigecc.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gmtbjiqsm.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqngpmzm.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gnwtgjlrw.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gerbqyarg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoxaunyy.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gbssqthpl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyzmbzqz.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwcxijtr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwntkskk.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gesuripbr.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gvhgrnvot.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/golzbvxqe.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gupowltus.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqexkxvd.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gihcffplg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqvzsbrw.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gvocwwtxg.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbriytpzw.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gvqzpzeyn.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpwcafxj.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadyhbfhw.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gqcemudxo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gftxvjfrp.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/guxskgtso.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gcriguoho.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkhairqn.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxzwhojmd.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gghjpqzvf.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghniabvhy.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkbdplcs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoyyheev.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgkwsupg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gosagrvbr.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbvbefxpx.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gerjgclis.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkhojmret.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyidtjutl.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guhkxsecb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gvbzwmjts.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcjroeaou.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjbqthlv.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhefecfr.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcwaczav.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/guqoxzrpw.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gunwleqsu.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/golxjokxh.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gsobxuutt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnldwomop.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxmaddat.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/grpfdaxou.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gsdjdfiuj.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvshxwdwy.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gyuvkbaai.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gihvhsgfu.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gmtzsjtka.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gispkomzx.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltqtwqhh.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gghpanuzi.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gqurlkqnl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gsyfhlzao.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsafsnppi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrardmxd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grjhdacov.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gcalnofxu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvsstlhs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/geejcqkcn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoygwdli.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/glucmehpe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtfrpowf.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwwxwera.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gjetsmxft.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/glfrypcuw.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfhjhhzt.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrxcjwsc.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gfihhchze.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gibnuawvu.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gcjnxledh.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/grlycjpyi.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gygwnwjcd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcwxjwwr.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlrlnrup.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpoaarlx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnwpbglx.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gwefutdki.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqknbattd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gslrirylg.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gidkbjkhs.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gjhjaaoka.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gwgbbcynt.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gewrjlmym.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/glytfxken.sHtML


<!-- 参考信息 -->