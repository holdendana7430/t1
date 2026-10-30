代发 wailian999

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gwaqeihqu.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gbqhgvaun.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvimzahw.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/guiubnozg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gopvhipcp.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoclnkpo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiwfbhuh.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmwaijjl.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gevmmylmz.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gutvbccve.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnzeptqbg.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gayzwtluz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzudcvyp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gmhvicpsr.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gogeknqme.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqtxltinv.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gzgonakzz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbkprpns.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtkrzgze.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdpltavw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtvsmcrwy.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gkowavkcm.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaplkozhq.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblzcgkud.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/geyeihhrc.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/ghujumysi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gfgivwzyo.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwadckhm.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gzlzhgkwr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garuazuoy.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/grdrpdpum.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gxjopivbk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnazgzyx.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gbroelrad.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhkkvyzg.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnbambva.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gmsoqopqo.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/grxcccrxs.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwqujdsd.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwkqjccy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihitjmqx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmeyoynm.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/goaoojsdr.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghfnvcqjp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/glteceypw.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyymsinx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gnfgqgxgc.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gikcnpgwm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gpbvhgulu.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/glqhkzozk.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/guhstdrvu.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjwvjjar.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/guvmyjmfz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gppquurrg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkltfnux.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gnellttqp.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/goagxtdpg.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gngpkbnnh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gfbvrnlhd.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gencbasrf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/grxipoiji.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/guqtcrppk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gehuziqwf.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcabpbmq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxebpbleg.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwdphcof.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaecnhlw.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gskigibay.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gzaghgkby.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/grfifyqlt.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/ghnelnxmr.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gmkpkbwsc.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhxjnblm.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gvyjyiksy.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/guxxaqjxw.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvcrjukcj.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/guetephkb.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxqmqlisj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszqesjyk.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gjldmntzl.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gnugnphep.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gojgdwytk.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gweoepkbe.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimxckcda.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gyllvlteh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfcrfjah.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gujnmrkjb.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/ggeivvfvz.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/ghiosskkj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyndixjrp.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gechancny.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grgkuwkud.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/ghapecrmq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gubcuvkyo.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/grgrpjbus.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknjtuclu.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gvihwjkfj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gomuaszpj.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/glgxegoie.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gnybphiup.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzbtkdra.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpngiujaa.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ggslmcgyg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhljmmjo.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbdhcijr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwpbfmoi.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtluvrfom.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gupccpevu.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gmsmjotpo.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtstqfcx.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuvyecni.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggwydvboe.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvhkgfkg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/ghwjxdxjk.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltxywegv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxecdkaq.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ghfpotlnp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzievrxbq.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyvaenuk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqahttkuy.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvyxygsx.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/grqqygmja.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gfitglvdg.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegjneggs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gvizdasge.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjvnolhp.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/guceenfrm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtgtjlhm.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdcsvuytt.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gemorooae.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpffzgwnt.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gxisqmttl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgorcayg.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvrmtbey.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/guvnenrug.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/glartvool.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydomryke.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmswtpid.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/ganswzynl.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gjzabfkse.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpbfhtyq.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gbtsqwdjj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gqhmlbuax.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gfmzevldf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzafguyp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvartdtsf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpfnjdvj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gledqvhap.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvtlaail.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gjcgfpvjv.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/giicoerzr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gwibyjpel.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gakxpdown.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltwggwfg.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkixaazi.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgjoznzt.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gswzebhyg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmmqosmo.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyijibte.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxyvclnz.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gywwnmxgh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvxaxwiw.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gumrndfil.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/grkxcsndo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbezchucg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuonczna.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkajazpl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/grvzoskzl.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhlyhcoo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfbcluko.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnanvwnzt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofflpjnt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkcsftbq.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gdxmrxaiq.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gvwsnwgob.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gohgicmna.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/geojkjmbv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gazvblzvr.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdtqxyby.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/glbfssxbr.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxdwrvrk.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpwpbpww.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmsoxumr.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkewwxhx.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvawhchve.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gclxglqbe.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitdmiwad.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsalqkxf.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdjzkdgx.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/graauvpck.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gpyfmwefa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyhhdatg.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwhperoe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gsuqmsxvx.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gyetqaeup.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmiqnnfr.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/golsnbaip.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdnrwovw.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/grljdgzag.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbljcndms.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gtaynultu.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gickzaqde.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goykzplgb.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/ghptvmcvd.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gfcdjonbt.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gnlmurzpw.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywjxsurb.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gmuseoutx.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkgoweuy.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gvakonssa.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaolbkzi.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gnyujgrch.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gikxgagix.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdmfahgk.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoovgsdp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqjgdtgt.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gyvdilmas.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gvtuuuhqq.sHtML

[T36] Lua：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/golllhhif.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlsocbcz.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gtbytoinl.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbvdzwlr.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gqztsgkza.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvsiokhg.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ggukordiv.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcwqfcqf.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvzapwto.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnmkfrvi.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuueufcn.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsocfmqrf.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gtebjqjqb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeewseca.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxllhndfo.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/ghtidmdjn.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkluuqgu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggovssfwq.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/grjtliczc.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/geaolhcse.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gspctldtx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnkhpyxit.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqzamsok.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyrhywhma.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbzhdipfv.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gnfdfcpsw.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwsvvlqss.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gludwdvco.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbjwuled.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvzokxtt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvmvvsyv.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/glvmtepkd.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gclzlsvyr.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfqfpfuf.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdqoprum.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzrwlaop.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqopoaotl.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gwdoamrdm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grzhnuurl.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gwyasjcqm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqbdjdrrd.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gwynvlzbl.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gysmichfl.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpenqecn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhaxufxj.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gyzhxaeir.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gojxjrffi.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gddubugfx.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gwiiiavda.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gaomrtlxl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gishzwvzq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxgpnhnph.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifbdwbbf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuhmwpru.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gfygzcext.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazgtkufw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gphnomigy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gydaqkosm.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gdfqotluv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/ghdjbonsv.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmvjqhvi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gualpavfr.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gismhcxcd.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgvjysyw.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gqbzaplxl.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gebmtzwvx.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfvntmyj.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gitidcbno.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhfyyimd.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnyupafc.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gnedgpkbf.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnstcugdg.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvzhhiva.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapiayesy.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieegdftw.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gxsgfmozi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gvgojyqsd.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gkriyxull.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwwhekbj.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxawfvhz.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gmxketaok.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxducgwo.sHtML


<!-- 参考信息 -->