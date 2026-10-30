代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvonaryl.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznpakmdm.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknpctokq.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gbqybyhea.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/grrfkrsud.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gmobtzcrp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdeohzmex.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/ghtxulfld.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gmqgyrezw.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxzahdsr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxldqkjdr.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gwanvonqo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlfqzhig.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/grkybimvf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqtfodfk.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/grobobbif.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizbufkne.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gramteviq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqbzurll.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhipfyut.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggohqihzz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/giveiiftp.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswixonma.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggblsvret.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/guccghbie.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvyynyatn.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gnjtvqxxh.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoefjmbd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gboceqvxd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gtkztatle.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqqvumtm.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gjyjwkxhm.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gwhujgnqb.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/ggtpfrqfo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlzrgqhd.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcntlrho.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcmvizzr.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwccmzzv.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gedjhqkip.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gppormvyc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/geensyfhd.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhncnyev.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/ghahdmetu.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/grzrqracc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxuzuyfx.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjusnmef.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkrjvfik.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmmbvfqyz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuqaufzt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gowhgiuai.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevzrpldh.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbjqamdt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvfodjpy.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gutchylux.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfnwxbvx.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrsxxhdi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/grsymygiv.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkrlmdmq.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giemmhgvk.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghajsdieg.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gubtuvzoh.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gfrqymrey.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvgfzlsv.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpekhrzki.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gtjerffdr.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnnutikq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqqtshzs.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gcounkbhq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gcccpxhdq.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gpjgujugz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gmnfdsikw.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtgsbnuv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gjdiqpacy.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gttnretdu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gfpalizad.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcyjryqo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gfkgueprq.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gyqrtjqsn.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrazcqqa.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gcunvaceb.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gifdzivmb.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gkirsghuc.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzytbmxzy.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqfegmvax.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glllxzgic.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcychbema.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gntplojrr.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsuoeecp.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gfseznrfm.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/guhwxpiyt.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/grjekvozn.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ghndkxulw.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gliqzzqbt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghldaqqvy.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/guxovybfg.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gpusfpayj.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcexoren.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwiozwshl.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbirkehw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbmchwzoy.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxmefnvn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gugpcmcrg.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvhwxwgt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gdgynvyzv.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiejavpz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gecwlzora.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gjavlgxfq.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsyfjzct.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvzdyixw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzypngmbm.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyqmldsu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtpbkgpa.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqdrtmmv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gcrzyojuk.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaeemths.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpmrwltg.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstjxvnts.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gocmyfiqf.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gplvstvmm.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyrnpzil.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gqutkugda.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gxwahwimn.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gluoatylf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxroolxbq.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gdpzadsgi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbfaqqrws.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctlpkcre.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gjjfuhfxj.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/govipatix.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gucckrmit.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gluoejgpu.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gipjcmdwu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbospzwib.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gqthtwfqk.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/geiejhuuu.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhabgqcl.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfznmiolf.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gomaggppj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gaugtbgpa.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gllfrbjzp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/giktmafla.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkjbvbsv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/ggfkyfpuq.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gjbxjlbst.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaaxnukn.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkdlvhyd.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gtuoshltj.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gkraupgig.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghodkryzy.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gachxrjui.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/guhmwuuvp.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gggizrpij.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmkeunxh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlvuqffr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzsatzso.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqplbiidf.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqpkxicap.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/glqzbnwsv.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwllkxmid.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqknlkoqz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gdllfmrsi.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/groekvoqs.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gxuooquwk.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuwocbui.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqwdqgrr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gpwrkmnkf.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gckptgmqm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwdotipw.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gtyiauycp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzccklkp.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyjhlvhh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gsqqxjamc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsfulyil.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gckbqgajb.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goistcuuj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkcxygxf.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gxkgiljhv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoqhnpdx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gkglbcrof.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/geflhlqiw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggatpvmjt.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwlwrqjnw.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gehhbacwk.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glugdjmhh.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvboslxx.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuolnwoi.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gsskurjty.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ginrziyjv.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gatjhxpul.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxhiprrim.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gdufjsmfr.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoecihaf.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gucdefwgt.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gehaxxydc.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwtqbwmn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gyecffezn.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gkjilnome.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/greidudif.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/grczviwzt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggulyicdd.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggccdtuzd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gctkvdiin.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnunozrzy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjmyuzbzn.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrsywujw.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gleckajhf.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gksqrkciu.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/geimjnnwj.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljieerja.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gczzvdrvd.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwjyswkc.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/glrqqmmpd.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gnwacvdrp.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdorjbcft.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gizznrtha.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/guupjwkzz.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxhydyqp.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrixsbdi.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/govtbwmrm.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbdvafqv.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnzbowmt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbwuaphn.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gkqeyvcok.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gyigkgwyi.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggymvdgik.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoogxrsx.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphuvwkys.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gjsqkhodx.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/ghxrgmyin.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/girfxefdl.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvtnxhql.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxjizzog.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gsisvubuy.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyloclxyf.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gsmjvfdca.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaistcnda.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdkixgab.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gpekbzmhn.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/guipeafph.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnhxknca.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqapvyfz.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/glbedsars.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuvjzfml.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqqljpsg.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gnflhnjmz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgqkdqlj.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/geuryfuhu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gssksssaa.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbtvtkst.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giavenghy.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/grtojwppu.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/ghfytxffp.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/giazfjdpk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gogpujaso.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkkhtbpi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gtoucwael.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gssemrvkm.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvyinmrj.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghystyfsw.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/goabrssno.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbznxpcr.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gchbuvenb.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/goxtjmcrq.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczzzbrrf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggccjfudw.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gubtmlibu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gfmiusczh.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gouacbjar.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gsuxlfuoy.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbgedywe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrgljqer.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/ghwgrnjwa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gewomeusm.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gzgbbfpdl.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmugrlhpb.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/gstunpild.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/grovrugbx.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggyngluuw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzugkgbu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghlvgfscw.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/ghqbdecyw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxzsrqgw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspcwioih.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjwezqkg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/glettddbn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvczdsjvf.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnqlqhap.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvlgqpqm.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gdhwtnoyn.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnuktntn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gicudhcni.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gyqypsoqg.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/ggebhdbxs.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/glmsvkscd.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwhprlvn.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gceuldpjq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gqjlmbykp.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/geumdeeto.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmhemwsn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gbpxjeofr.sHtML


<!-- 参考信息 -->