代发 wailian999

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gtcytrrkt.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gvtyodsdj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gpsdccixs.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gzrkycwqv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gzkkuufmy.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gigyefivo.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gdqfnizik.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/ggffqfdkb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gzbsqlova.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gahjleszc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/ghsarvzeo.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gokuaanhz.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gczjhveyh.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gguacjvri.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gebvjscfc.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/geasfsqss.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gqjlbemvu.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/ghdumjcnl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gldprbxhj.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gmwrpynkx.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gehvbkcqx.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gjtnrmknn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/ghnygtmef.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gvgowtihr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gponwjijx.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gsvkumubz.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gcypndiyx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gycwvgihu.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gpeieedqw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grcvxcjsu.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gamwobhyh.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gwzooklro.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gqjuobbgi.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gooprqock.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gxllrauqm.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/golgyauwi.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gxslaumoe.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gvhksgabw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/geyobziuk.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/ghqtdkihh.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gvkchwfrz.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gnjfnbyhl.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/glsowffip.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gkwgzdpnt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/goyogswzs.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gkmxideqn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gmpbbkajh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gaqgolmrp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gfjdeutcm.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gbuzmeabu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gpqongfqp.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/glagfloyy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gqfuongct.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/ggkzockmm.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gnypxpwxl.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gepxkekar.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gugtotnac.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gfkktrotn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gignhsqrw.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/ggpqftpvm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gkvsgvbqz.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/guivjixcc.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gedwejctn.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/grhxbmjya.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gckjjkycd.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gqoyiugoj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/gzehvxhge.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gvnbwawpb.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gfgrxrjsd.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gdtdiecqp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gzucztimu.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gngitewth.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gbxtrkfuy.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/ghaigmtxd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gsexzeybo.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gszevjpar.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gdqwtazru.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gndceirbd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gomhnwkjn.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gdqlotigu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gbbessfiw.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gskzvrkue.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gwpshfnas.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gdblsdzeb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gptnodqzx.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gzdhkyfod.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gcfuensvg.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/giawfsprq.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gfkzgifjz.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gzhmedals.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gyukejziv.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gxcmxcgfr.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/giadxmefd.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gaovqxxwa.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gmkrmswgw.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gmzenoysl.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gdyodfmzn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gspfsvpas.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gtbdrdtrh.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gijkerjzf.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gyhndljjw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/ghvacocor.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gouzgqxhc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gvzalahnj.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gtwugnbwv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gwdepokts.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gspsowzjh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gygafsaty.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gjlvtgfsf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gayqwndlx.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gfmttwhxv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gwacrekxq.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gqvctuuau.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/ghxtpdpxh.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gxnykasqo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gvziezqjl.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gveelxifr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gxhbtyyvf.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gacajkqrq.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gkwsaqash.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gotgtfvjo.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gtdpbwfen.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gycjheprk.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/godjdassx.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gxmkwvmrk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gmyyrphgk.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/gbwvpscao.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gsipoocuo.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gclhrnbfq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gqclkgefx.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/geqoyxuua.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/grmpbkalp.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gjlbtsnze.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gzpuampvu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.hesvh.cn/Article/details/gdjrwewzp.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gouwyuvtw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gkplvroch.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gxkiluzud.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gsiijdwrk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gdgltmoxl.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbiigeakh.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gkpowdlil.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gbdlkrvqn.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gbrmgerqz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gitkfdsbu.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gktfufdyu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/giupwnuzx.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gcnnslmbc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/grnjnsdac.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gpoyrxqhg.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gunjwwacr.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gwrnlgtzo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/goituugrf.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gpikrnkwx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gxkqkiova.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gulxbqqwj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/ggzvccjtj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkrmoyfts.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gkluroscs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/givgtyead.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gpgsgwfwg.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gnurrxmnw.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/grigfdobt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gleolwbkv.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gmgjkrlgg.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gjoqzpejw.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gmohawbwk.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gzjthmmlp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gmtaueitb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gkqzosxwk.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/ghevheecr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gxwemtpcy.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/giikqtqis.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gyzwhrafh.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gvltkamld.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gxqdtyxro.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gnvvmdjfq.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gbywnwelg.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gjhasoibj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gtvwuwxnd.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/grgwnwqyj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gjdnctmqm.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/giwwcxtsg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gshgpzkcw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gdoqgspvl.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/ginlxpjvh.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gwoymtkso.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/ghsthozzo.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/glomhuuuj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gneupmwfi.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gdolanrdx.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gnmumuxww.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/goecfuarb.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gazsxzkmx.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gbkrnppxe.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gkomdgojb.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gujbtmlbl.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gdwpwyzhb.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gjyzxuedb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/grqochuob.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/grnxwhkho.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/glqbcottq.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gofmgashm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gtyqmfjqx.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gregyglte.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gxlwxqztu.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gpigqmzss.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gxyutsfzz.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/ghugezxme.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gzxwzdzyt.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gztgcgsbl.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/ggrfemhmg.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gbbfqsthj.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/guchpljtv.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gqhkxmhru.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gjebmvgvr.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gxxhlqwhk.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gsrutbgnb.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gsoiynytt.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gulruqsif.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gpmmvcrzj.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/ghxaxhacc.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gyajanykf.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gfgcpspiv.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/ggesjwswa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gosupnmpw.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gkskelucf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gbclfymji.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gefhapfbt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gnxbtyuwu.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gutaszlum.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/glgqqikxv.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gbclzkahq.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gicmgccny.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gcdowtmlr.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/glpjcmxaz.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/grevtmgtl.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gdjyqzxxg.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gxrjotrtq.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gpowstidg.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqsipkcnp.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gappbhyco.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gmkiakkqq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gpflxtrcn.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gwapzehun.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gzlfwcppl.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gjtrqpsba.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggfjduyiu.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gzvkjzsnr.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/ghzwkplsz.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gnpwbazkd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gkrurfkff.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gryeoxoqn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gsdmeqyeq.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gjtrcptdc.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/grliiclml.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gioefsdev.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gurzpgqwt.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gcsjqvvmj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/grdsxomdu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gyofeyatn.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpippkgcl.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/ggyrqnrqb.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gmmdosrrb.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/guzmumaex.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/glkfznubr.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gallythww.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gdjimjthw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/ghfbdgazg.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gkqrklciu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gafttqcxh.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gqpdveowb.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/ggpvwflla.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gmwjzqqxc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/ghgwmeafp.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gmhjblagx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/ggiqgmblo.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/grkpezakb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gigqmscyx.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/grzzyeicy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/goddtrkgq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzwhrwali.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/glqmsdeyv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmrqrwmon.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/ghdentcpg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gdxebzcon.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gfqfocjvx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gkmycispm.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gtescrutx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/goobmctso.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/ggnjthuoj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/guikmennh.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gksvhwldg.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/guxqggsxu.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gaedpqcdq.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gnzltdief.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gcvyfrhpl.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gvsagvprv.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gqlcwezkv.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gjeddafwi.sHtML


<!-- 参考信息 -->