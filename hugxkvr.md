代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gxgdhvguo.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gmlagudfh.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/galubwode.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/ggcpgrqwp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/grweoimnq.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/glxufgxvi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gcsyxoyvs.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/ghwjidodl.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gtefoxtwy.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gpfvlwqvt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/grtbyjqlg.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gypmonces.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/glymkgsmk.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/grhubehfg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gstwkpjku.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gjuhlupdq.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gwfsmxkin.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gjbnvikmj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gdgnjisgu.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gxeuzzozq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/ggzxuecyg.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gbgjmdpop.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gawkdhsju.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guehrhtjt.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gtkvrkfjv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzxukosdd.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gcunxpuoe.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/grkzlrmqd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/ggmhgphxs.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gposifgnu.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gqullifjo.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gigvdawzj.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gjpyzuthx.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gfrkjtptn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gkswaudvs.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gsdcryrzy.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gtekyyrzc.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gzclvexsk.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gqjjqfqrw.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gutgfgwuu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gnefkpxoh.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/ggffyyflp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gslweevhk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gjsznbdmi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/ggiohigju.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gwfaspois.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gntbindpy.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqerheois.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gkejbwbld.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gqpmcrxyt.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/glqrswzmd.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/grsfzwyyp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gleoepxua.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gntytrjff.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gkdfftwgo.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gkfwyeity.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gjkiacbbn.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/ggtnulclg.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gtvuqbwht.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gvjovkmdg.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gcpzksxwm.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gmoqdvchc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gwrglngqb.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gqhlmvudc.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gtjdzpvha.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gzqhaftmb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gqlitbqgh.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/geggmyoas.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gpiuffopf.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gowhvpfdr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gyvntjnfj.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gzyofbckh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gyazoxlyj.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/ghfesdxzg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gyrrhqmey.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gdwtwtfyr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gxwrvuzgi.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gcqhulzna.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gqkrbvocd.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gnjpoxjri.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/goczegjxh.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gphulgxip.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ghsmusgkx.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gujbmpyss.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/geyyxkxgr.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/greopljtu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gopvahxfp.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gekzgxzfk.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gfesrggxu.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gxwhvufkz.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gmcyuvsux.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/giqfktgyy.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gwkdrjmku.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gkvrzvlfq.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gxoylbtvz.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gtufavlfw.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gebwpmykf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gfpqtahqn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gmmkkoygx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gsjyqeclo.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gexudnjgm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gczenpidn.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/grjxjetie.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gdsfywnso.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gfrjqmeje.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gxzfobsbh.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/ggeasefea.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gffdkzqbh.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gzkazmfjz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gfrqsgklk.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gqjpjrrcp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gsirzqymd.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gjdtndrkf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gahvjhjvd.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gkiolmwjh.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/grsvxtxsq.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gswiduhaw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gdhrstsfi.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gphjaihpq.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gsxyrdlqc.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gotnjwjow.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gftvpjwrw.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gpwlfxjfq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqmipmdab.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gmvrivgfa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gybsnfgvf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/glcmizlrq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gwymyvmrs.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gkooatvpf.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gheehopnb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/guelctceo.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gncmatrtw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gdrmhgghj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/ggmioijor.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gyqepweku.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gejflbclo.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gisndbijx.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gtuordgnb.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gyzxfzvva.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gdxhgfyse.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gptactrtq.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gfpgvnryk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gaeafcxwm.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gfalluvxx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gxiiycycy.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gzczisxtm.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/grvxrrsda.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gumeqvdig.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gilacxfcp.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gufzcbrus.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gjtezdqit.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gllmuvyek.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gnwnieajg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmajbebxc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gaqqrriqz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvrsnmxut.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gqeqxwnhc.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gqkqvvdyg.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gzfkpxvmn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gifrfnjiq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gcmzofzcf.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/guntymlfb.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gqomrrhxb.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gmztmmyjk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/ggdnucpis.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gistmpjpn.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gtlfhhobg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gtmnmtbaf.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/guvsrxmgn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gtxceeqym.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gksvywdrc.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gynhzhynl.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gntvticvn.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/galdsmlcj.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gntcurjdg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gvdqzuwjc.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gqgrjxhal.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gziugjrua.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/genmocuke.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gkrbmhhmr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gojmjmcnk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gjitxkqdk.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gldhhnpgb.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gqbgjryjp.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gunqflpph.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gyixvdysk.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gtowtytmm.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gvvcdjnwx.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/garhhswmv.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gebcoyofo.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/ggitpvtny.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gozfaabli.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gjwxkydfm.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gkgaxaevg.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gnxxmrfsy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gznvsdrng.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gtugzeppr.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/groxlacim.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gujfnyogw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/ggrfyfooh.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gwpqvtfqv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gscptleuo.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gtisjzrsf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gvragkmtd.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gelvtgfnt.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gvuopwaxg.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gvealznqe.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gfolblpsp.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gedsnflzm.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gndyaeoml.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gjgxpbaqn.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gupzacdfe.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gyzkzhtrf.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gfzjqxaxn.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gfmtmbfsn.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gihmlpbtx.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzunjbzrw.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gcytrcsdr.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gqrlpdaxg.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gryrynujc.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gblvoszen.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gqjdumdan.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/genndceau.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/grsceymwm.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gxskjsokf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/grmhafwhs.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gbtxrdcxi.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gpumturpy.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gobsivfsk.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gjfarctit.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gfpbaecdo.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gnmmymmpm.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gaesipleb.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gnwkqqcvx.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gifyneuno.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gesbfjtzz.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqdceoclr.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gloodplua.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gcinuceel.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/ggnurjgwo.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gcaaxdczm.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gzchbvhpx.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gnfvrrosw.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/grfxbxzfg.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gntytywex.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gmihiomfk.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/grevdjlvx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gttuamlce.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gckkgqbyt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/glpqlqwmh.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gihlqcicf.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gnmxwpsrg.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gckzxeepk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzvnxklpa.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/grwbwmtiu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gaatpakfa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gqvrmsvbx.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gihcfxrxl.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gfthmamon.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/gvjdybepy.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gggjfofmy.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ghufkdsii.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gborppide.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gqjkdrckw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/guckmmmwz.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gerhhfjcl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gclgrdpie.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gckxkyfci.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gsdvfkefj.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gquryycwl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gorrkbujq.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gjllyzvvy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gjmraomfp.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gfvsxbllk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/goecriddj.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gywzxfvqa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gtvrqjzuf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdgzcpgmp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gaxcrqycs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvxrvtduv.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gepatufxi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gdxezpfky.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gpkwedtqo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gzxkxthnk.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gsmoausix.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gagfjmsii.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gwrvgvsjh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gaoejxbey.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gbumhhrag.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gdsfegguc.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/guygbglld.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gmyqshcds.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gwqunxlon.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/ggalfnfzm.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/guasgfvxw.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/ggyrzrcnd.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gykoflrkm.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gdrzlwpzd.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gtovrmawq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gfewewjig.sHtML


<!-- 参考信息 -->