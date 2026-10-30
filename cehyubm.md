代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gublhvnnp.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gpooamzje.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gdjmuxyfk.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/giwupebxl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gosuitupl.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapszezpo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxukqmau.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkaeikhf.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gumoxaeat.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gutlneecg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzdtxvirz.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzmdrqjhi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/glbmkoirh.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmncbxvgy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswajuegp.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpavgili.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpcdqqcu.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/giqnatejb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipclxzdg.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnffwfjm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gccixfikr.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gakfdwbxx.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/geglmjpbn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpapughzc.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/geloreveb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gructpgfn.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gpwnmndbc.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvqbuxqs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gikquzggg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gquvooytv.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqilwvkxs.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gnzgazwzv.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjjkgvuz.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzaxulus.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykycwydn.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuuschtw.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeiggfeu.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxisomfbi.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxeelvws.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/ggdbeamos.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwkoespa.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gbqacmwpv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/getftfqvm.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvhpxhtb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhotaxox.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gqumkibeq.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gjnyyqlit.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauruabec.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzcdsezp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/guxvkujhp.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gksqmsfmx.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzajikqs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gamonpxsr.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gqydgjuxh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxostuqas.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/geffzhmgv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuemxtzk.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gbcaozwzo.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gdfxlhhuq.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/grsnzeoag.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gcmxfrkcb.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/ghwrjzloa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gdfdvvgyy.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gspjlhtsi.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglepwxwl.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gdptidbkf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/goivrokat.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/grvzoojqi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gmotdwdhj.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/geqteacue.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gwlbubrsw.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhkforet.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gzroijoec.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gdbslstrm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gqgmywwbd.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfucqiwfd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gpqgstgrb.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjupalmkp.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhtxdgtj.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gylxiaeek.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgeiukky.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gwcefezel.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gedwsbgxe.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcluemrun.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gpzsbstjp.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagrfhpxz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmowcobno.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/guosesosl.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gjycmqkqx.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/genohcafq.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkoeatzh.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkohjndy.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxxdqufa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocqwnnrf.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxvkwftd.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gfgxcjleq.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gvcxahaim.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqumcifdd.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwkmyudm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcssbfhu.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gprzdbhgf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlvdgiqn.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gdsofhwnu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/guzxvcnzv.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gjkczfmra.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gbjidubxo.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgdokbdy.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/guvubufat.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gccgfeeup.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gadeztntt.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkqpoums.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/guvzqlmie.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gruacgnel.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gijsmldlt.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyggykgn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gxdbqrked.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpumkcntj.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gqkhzrpoc.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gzplhpwcn.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfqxksut.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gakfazimn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gwlkkijec.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gdrtwcpmu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxzrmwbhi.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/giklnppgv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grtafuwxv.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqepjqrng.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelrinyrn.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlamipbz.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjmbseom.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gashpxnty.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gsocogxbe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gkyusdfjx.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/grzsuhzho.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqjaqblg.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gaoibbunw.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghiailng.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gdsvyuemv.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyrwnstz.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlcvpfaf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gdufxtfzp.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyoghyce.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gticyfhkm.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmmyztnx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcybgbhsq.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gfjgbemtb.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gurgjncyk.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gegtrkhgt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnsgjpwg.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gzdlhrcbp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gyremyjoh.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbjmiwxm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gfzwmmfnq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcemesktt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gmafzmobp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giyyvapdw.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gzngzxdcp.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gqmymexnm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkisitmml.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/glrfmtgqj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoliyugb.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/grgmuaoca.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqfbnvku.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqxivopt.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvtmnoci.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstcrybmp.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gmktblluq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/glctfxpfs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttyvomfx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/ghrozonfu.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gvgrimmsv.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzkexrsf.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gabtfqbep.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvbkahcz.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmdndrqu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gwjfcgqbt.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvxzwian.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuqehccs.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrsxakoc.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzfwpzyu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjujowid.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtflezujo.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gfpfoixih.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsejmycvp.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzvxllgv.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvboiyulf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjplvxuy.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdabnvenb.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxfrkwde.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gdrlzeisn.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gcidvpaxi.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwsmurdm.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/ghstqchkt.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gjpgaumnl.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gaydinoci.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gyijtxnui.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkizvmyvp.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfyntbvb.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geetvvowf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gzviitpqr.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkwcppnvp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpepwmglv.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gdanivobo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuomklsn.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/grjhbyvhq.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtadbtrzb.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gvhkgeivx.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdaxxjmn.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/guwgbkprd.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gibtckjim.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gcyhchwym.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoqghzoa.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gclxhwlgk.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gzgpfxihe.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnfujvcz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwzjtera.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gjjvzuzbp.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gypmlcmhb.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoghzmtg.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gecfwzptw.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcqdbikv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gywyeqjcc.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gkudlyduu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gtarrxort.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/ggskahmrz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocxsqqok.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhhwcsqt.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gdgmkzszq.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvrwqdmw.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsmfitno.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gifdokvvg.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gznocgech.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gysoqiref.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcbnqoke.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyinjdth.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gomkxayyt.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpogepue.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gwmwwpvvd.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqargtga.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gwganniub.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grboxapux.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/giyaqhpmg.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gyakfcjdy.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbaaivpek.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrrggjid.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaetekzqm.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gyplkfgnp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggvuvyift.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpxanwcz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtvmaagpc.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/glyfebsfe.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqzllmlb.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcbapmjfr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gezvxfbkf.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyrlyhfgx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gfzopxqsu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gznfjagtk.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvqfylmo.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/grxxmsurh.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnwdpcjnk.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowbbkaxf.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gabppyhkf.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gvadsxbgq.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjcelprw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gbjaoswzn.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gseuftxvz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzdtxgglr.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gxagorqti.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/globusici.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gmstfnwrs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkorxfqps.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gibgrwghs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhzcehfp.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gwzuyxuan.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmberzslm.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqqunqxp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gayhwnotl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqlsmleil.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/geormmqkp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwfdnhomh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gbakrqvjv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gzjtrbcts.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyfgfnqi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gowmvzkqi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gonbqxnmd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/geemdxasf.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvmgdogg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gpvalnffa.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuhbqdaw.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsgejerp.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gyerwenna.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnadjreuf.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/ghcbkxgjt.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnutlppjf.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gzhhppuzl.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtheaope.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/grgapyqcn.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwrsucgn.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gbrrldaqm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gpjhjnqej.sHtML


<!-- 参考信息 -->