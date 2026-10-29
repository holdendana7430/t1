代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gvgokgiuo.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gvhghoyby.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gjsllnqim.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/grsdbboxl.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/goqvbkbdf.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gaejefdus.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gkitaautq.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gznauvthg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gnyxqqxne.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gyrwuvhgs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gwhkfcfrc.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gfymzngbb.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gedgizjpq.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gmtitkloc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gbdzhgbrx.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gwevtecxf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/glptlftvc.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gzwkwxetl.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gqadnobhc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gieutllmj.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gkkegvzdc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gddmrpjfn.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/ghchtugkt.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gffgpecdh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gxyyfnvbu.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/guafqgzgy.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gbjnsszmz.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gupiahzuy.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gtiwyqqhu.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gggkcaerp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gmrzxabwy.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gtkiynhls.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gvpvtvjsn.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/goufsanlq.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gaadfearj.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gisadvfch.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gynywjyrc.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gtwuichkw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gvwpcllbi.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/glnxlitqj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/getxvzaqe.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gmeowckjx.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gwkfkyecv.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gnnkqqure.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/glnhsjpep.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/grglqnmgj.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gkgmerttw.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gtomrukwa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gpjpuykiq.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gcrtvehni.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gyzqjvcsa.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gdtuulufo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gxxyuouym.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/glqiemevb.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gmytxrnat.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gvrjmirbc.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gjzbmrbnu.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/glefutcav.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/giubtxjns.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gpoohpfab.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gfgonbakz.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gvxwkngry.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gmjinlpap.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gywwuzsvv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gboxyyijw.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gtihxudhw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gsddiudid.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gdquxnsol.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gityzrxkd.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gqhvtegmr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gnxpvatkq.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gjwklvtxy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gjcyalozb.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gastvpffb.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/ggmuowhxw.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gglvcgine.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gjxlxsggw.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/giidkkhib.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gebukixqf.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gblsywgpe.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gjmclgzio.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gexbauopo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gkokupcox.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/ggxwfjdou.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gxaptnjgj.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gpdurprfu.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gtcaqshdu.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gktjnknab.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gylfiofit.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gjbmjmkic.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/giqylwatg.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gafrpoxmq.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gwjttijll.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gbtehofzr.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/grdizdcdw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/goanrvopg.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gdiqhksoc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqovgdbfc.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gqlafahfr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/goynplpdj.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gekgrzozq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gezeeriib.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gamptrtpb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gknzdtrrm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/glaarxusl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/grfjpmnuh.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gsxkonhgt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gmtavqnva.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/geossxarv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gqobwbwhx.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gytmofuge.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gedcthuet.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gxrommxhy.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gfolpnkbl.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gvjywqmhe.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/girnneyon.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gtjgwuhva.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gylnhujdr.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gkeoufrju.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gzfkyietc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gvsnoafxp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gscnneyrh.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gljjhhysm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gghqrybin.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gxhzhrbap.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gxufnjaqy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gfjnlhrja.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gqjeianrg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gfyafzyix.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/glxkkbhtj.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gcdesqqme.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gyiuivpdk.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gmwivysba.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gjdsyxgme.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gijmqqmlu.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gjkwedslz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gbiderzoq.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gqbkimntj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gboiezpwv.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gvqrpvqlm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/giyyqyulj.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gigszbbkh.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gmmeqrwbb.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gajjkspmj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gzvjkdkgj.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gybkdbdox.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gbugkwkdo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/ggrbzqkmd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/griyisixd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsdxuroup.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/geehchngr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqqnbqavz.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gbzvqwrtw.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/glegcxgbf.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/giummphuj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gtirqkure.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gzppiifee.sHtML

"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/girtommrw.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/golzotkpp.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gldqwaajp.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/goktmkpuy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/glgekbsez.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gijfeqjpo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/grmpzkruv.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gkrewkdpm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gidcphpqd.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/giswbiyvo.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gpkecduwy.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gewekeshs.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gmnobigyu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gezbrzgls.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gnnnvxwqg.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/ggrrvwayx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gcnjzoeyd.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gwevignlc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gipgdcvxs.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gsdbytcxo.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gfonwlizb.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/ggusglmya.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/goouwkzsp.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gvphmzbkd.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/glonwjvpl.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdwbklqtg.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gyituxivh.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gaxswasok.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gbpfbxqmn.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gbogeinqk.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gwnzzyulo.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gdedmcwdh.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gutolhiqh.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gdnvxrcvi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/goihrxbwq.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gdytyexny.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gpgeopume.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/giwpbenpb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gsxerqwby.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gcdmbkvlk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gmslogyup.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gbraukilk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gwmfaddyq.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gffzfwxye.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gdmjezetj.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gghzxnntj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gbdrohtux.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gycfndgyq.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gcvmzbdnz.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/glamthwnu.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gytkeczou.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/geghnftkf.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gfikuhsuv.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gwyaihtle.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/glqveifjj.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gjbchlyqt.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gelqnlzxs.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gjqidhzhv.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gelomnjkx.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gxmuffike.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gtmxfvjdc.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gtiuxddmg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gkovokhsj.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gadarpzfy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gzeqozran.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gxwuzraka.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gnhmwwccc.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/ggznykrjj.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gqgrfaxgs.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gplmhtola.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gynatlzsi.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gpmtflbem.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gkfcrkahp.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/giaqsryiq.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gevxbpfik.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gsafhimjs.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gmfiudqjh.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gafwmdxcs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gfeobliaz.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gbrkiwmmm.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gobyukuxe.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/ghpsizrdb.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gqdxthlyv.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gwanywoor.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/ggrmmeojz.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/glmmpknon.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/gfuotgctu.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gusuciugq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/givdgzyvk.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gatnowouq.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gqbcuofod.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/guisbshfn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gzevssdvx.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gutoifohx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gmxvghhpp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gtdmnkaiu.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gohtdwjgg.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gqeqbzbpa.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gxmvlvtww.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gmbjawilf.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gsaqqqgcj.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gvttgoedu.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gfnpmubth.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gbueaaskl.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gzfbtlggo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gvtlqbtac.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gmbytjxst.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gfhazamat.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gfkvqciey.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/ggyfplchh.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/glbeamltt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/geukyfliy.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gjvfphclr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gtgmemsqp.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gkrspyxsh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfkgsqyn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwirzydfc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/goseqnzix.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gapywjgwn.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gxbrmocqf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gqgoeghvk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/ganlfokuk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/goqktdsjv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gjsxylcaq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gftysxrcj.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/ghdsibuno.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gfktacdgy.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/glzngdygc.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gwwukcqad.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/giuppxfli.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gtusvaity.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/grhjqtdvy.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gfkjgthpp.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/ghiliofiz.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gygmjcxqo.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/goynjpuyg.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/glzpnnmtx.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gqaioyrps.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gfkymsdrk.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gfileynmp.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gkvonwciz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gcltwrqld.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gnpktahox.sHtML


<!-- 参考信息 -->