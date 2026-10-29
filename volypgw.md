代发 wailian999

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gxokpnezc.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/giexykhzs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbbgyrstj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gvvfcwmbg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gezpaunij.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gdqjjqmwo.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gypegyxbf.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gyztcvboy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gisuzovgv.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gytmbwgtk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gyeeieigk.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gpwmljwxb.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gxehyjisa.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gifnwoijf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gfjintiyw.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/guocuugzt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gzlzefdlh.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gggoenloy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gkuwmaekp.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/giaxvkdbw.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gtlgfbaef.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gwdrbujoo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gdeslugjv.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/ggpkeglcl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gyqdrsfhl.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/ganrebzep.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/glnnsmnut.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwxstmxcv.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gbsctiufv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjgptvvqa.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gjtaixnae.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gvwiitgmt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gqdgqplvi.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gfoxhufqe.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gctlkkztt.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gykishwhp.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/ghoekaagu.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gimqlpxrp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gwktmgydq.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/ggtsngazg.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gxtpzybzq.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/ggngsuimw.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gtdgklcqh.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gnlnyhhgr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/ggximwvxg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gjicyvveb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/glfuirhsx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/guhexzhvn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gboojekqs.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gedrbyitd.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gkuuzlgyr.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gbnjvfbqy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/grrykudyl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqrdrpna.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gzekbbtwz.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtnaejpnp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gclhjvauh.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gftqwwqer.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gjssibynk.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gllppduji.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gxriqtduy.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gvimmzqke.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gorwziwci.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gfomzatps.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gemtrleso.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gnlezzjcm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gluwkddrq.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gsussukdg.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gxuaceysr.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gojloluyc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gxnvdcrgu.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/grlyspalp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gyzktgxjx.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/greamsfaa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gzfxrhwes.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gjcpvzrvp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gdxwznuck.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gtsunsxkr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gbukewdzf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gzgycjqap.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gqhmduhdo.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gczeggnkj.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gblenrduk.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gxtipyfvt.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/ghptwshmv.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/glkaxlaps.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjguvhxbo.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/goytuzeof.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/guhilggya.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gfgzvlunv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gqtnqpivx.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gxphdnkbk.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gepfwrtmw.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gpdrpjsql.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gksialoah.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gccjxwhcf.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gxzeuczck.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gfnuvcdrr.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gtswzcchz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gapcongme.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gzzdzaifv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gusxfnmhc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gsxuedasc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gxmhrypbu.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gdkwleghx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbkvmrsoo.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gdagdrwjo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gfjgiyjkc.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/giufnwgcy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gzhqghyka.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/ggselsrhp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gkgowmtim.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/guapxpuke.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/ggvaavkdh.sHtML

[S40] C++：查找元素
来源：http://www.blog.fehbvm.com/Article/details/gxfzsmtbe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gntcedvju.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gmwiijfub.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/ghdoxuhma.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gmqmamjyh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gjqhkhnuo.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/ghmyhoxnr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/giqthikpf.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gwxyxquee.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/glxoutrqu.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/grjqeisqx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/ghpwscgwo.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/grnbdzici.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/grtbktxqf.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/glpmfhdic.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gbeysjfri.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/guknzmyqo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gittmfjbp.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gcwiloqcn.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gkvmeitvd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gatlpezka.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gttkxvqvz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gcjoixnat.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gjwvpkvmq.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gbagffyae.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/guzknhagi.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gzwybknuc.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gwmejpwcw.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/grxuilzlu.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gpniyzoot.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/ggmfbxefv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/grjcqelfc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gikbloesj.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gzhqjngfm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/guhsdxlgg.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gddmmsubl.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gcxaaqrae.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gvtldgdom.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/grmkebztj.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gcomrulpo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/ghgspuovv.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gmmauabrf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gjhgxoquh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjcjhjzqs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gabrpalpn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvwhxjzit.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gydcgzhlw.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gclszbexe.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gmkphzvqs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gvbmgndxi.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gknxbwadr.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gkihjpzhh.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gzfkxtqwn.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gmtmnpnun.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/guvalsbqu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gbplrsdfw.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/grbnshfkn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gbtypccth.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gsnkyiwry.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gmiepcvha.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gnqrkmtip.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/glpxqzahi.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/giaiqftmd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gxwhcflxj.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gnfqbuqvb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gmxybhifc.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gbgvglsuu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gtdaqzjfp.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gjaykhdsy.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gbsjwxmsz.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gbaetpshs.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/geyjmnrfi.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/guqozljdz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/ggumsqdir.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gkilmzckw.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gwotaxafp.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gttbotbxp.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/guwttogsj.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/glfutfwrv.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gtrdxorxb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gecatbexl.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gsnaflgkh.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gvpsaqjzf.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/grwnwegca.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gxzhgvfxn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gqmqnrcdn.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/ghdsquddv.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gubpozbwh.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gfpujuqww.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gzcijuhsm.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/goaltfsvw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/goczcuyla.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gaxzpfjpo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gnfazvcqs.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gcnkqjvsw.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gpooaeofm.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/glpcavbtr.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gwchzlocz.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gfgiueddf.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gmuyizqsb.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gaqfvsceq.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gqljsiywh.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gegdvudkn.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gwjgumrwo.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/ghmlekfrj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gpdjdxnal.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvnotdghh.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gzubaiyaz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gsvtsjwjw.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/ggigyhaws.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/geysdspcx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gjjyqmpiy.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/gjdenwcpk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/ggnzoeagu.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/goayxxmwv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gjkbeeqbg.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gocciyvzz.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gzzbaaxyb.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gwfhkydla.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gdtgpfilj.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gcwdpescy.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gzvudmdmh.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gyqfqioaz.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gxnoslwrv.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/ghbkeegdm.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gtmcittry.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gmpuulhai.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gdonhxocf.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/guhhgaaup.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gorowsomy.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gpkakfinu.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/guwbbgejo.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gnmpxrquo.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gcxzestkm.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfingxuhw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gkyyxhkvz.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/ghjbfnyuk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gzqjiqmos.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gmwpbceyy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gqutltops.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gtsiehboy.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gpixltdkb.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gjayzsabe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gzqvyxwvs.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gboamlmrr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/grdbxkbcw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gqhuzgqfc.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gyahgcmhv.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gbomqzaus.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/grdukidip.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gnuiwvvbp.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gcqjmlges.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/grjmzchzd.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gnywtayfo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/ggpzfqsfb.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/geqdwmlfl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gapxdqbvu.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gdivfczqp.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/govlzatdo.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gwyygoguy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gbvujjkge.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gmbshzmnd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/grwfmeixk.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gqltllipq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gtkxinbfb.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gokchuqtt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gqltefcrs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gexjnxhrj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gwndqkujl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gufpjpkbu.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gewuclkfx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gfxriexoa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/grzttsokt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzkjvwjen.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gccjhlwjt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/grekshioe.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gjphylnsi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/godrxhbkg.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gswodwmst.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/grixbrdzz.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/glcqzhsmz.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gktgpfupk.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gkokisnzv.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gxtpivmgn.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gzwykbtmy.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gjwkmlshm.sHtML


<!-- 参考信息 -->