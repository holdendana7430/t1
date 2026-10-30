代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gxchryecl.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/ghyouahfo.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gvjovmbcn.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gkqbmumpw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gixfwqzet.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gdcmwbcwh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gtxbhcafd.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/ghgvjfdqm.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gxsejgymt.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gsxtyultm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gnzjvzofx.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gbjatpdqk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/grdxrgazh.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gjpduvzrk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gxkjuogtf.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/goypvsqag.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gmxklgnej.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gygyslnai.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gqmrualnj.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/ggthjpjqc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gjgobtckv.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gfxyrqbhi.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gqnctsxfa.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggxsrucsm.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gysfsgbml.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grhhzcagf.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gmdbyavse.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gusoxxuok.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gbffpbmwk.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/giyupqwbc.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/glgneajvm.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gkinbngzq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gstzhwrfw.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/giujesqka.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/giweqbpbd.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gwgazoflc.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/ggevmwlyw.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gijzlphuf.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gfivopnbb.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gpzagjifv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gzrkhslot.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/graqwrkhq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gjlgxqajc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gncyyfamw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gbrrnzeoh.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gywdbgnxy.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gfwtqzuxb.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gvjklaowy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gwqawaljt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gzktbaskv.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gfuejdtez.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gkjnvrroo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gvqixgufg.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gjotvqgex.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gavfkqppx.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gqygjwioj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gcnafamag.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gqmapcejp.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gsrloxpnh.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gguoaivis.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/glsckwfaj.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gtmszbljn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gglknzwmy.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gqeefnkck.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gvhzjqynp.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gtfjlilhi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gcolqupcq.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gkgwljgpw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/ghrqlqkxy.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/guoaehrrv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/govxkmimb.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gzrfhqszc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gkuyqfbuk.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gxbglgtjx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gmbdhsaio.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gvfgymeaa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/goncktpqf.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gciirvpeg.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gfjtgzupv.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gaoxviyrr.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gphvwcdvk.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gmfsztwux.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gsveyqejz.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gouqbacek.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gykkjzvuj.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gkgzpczsc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gqttmdeve.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/giuwyuazz.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gmadvushd.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gdfkthvkd.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gnitvfutc.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gmerjgonq.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gjszezruw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gzxeqgsqy.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gamjssyic.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gwqlxelki.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gobweigfm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gqelegmqj.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/genzsybwl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/glmsqmwvy.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gsxtnsjnf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/grcieiyfp.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gghkcglxu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gfukubncm.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gafpcovep.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gyhfxhoqg.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/glakttqzv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gepjpnjvh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gtxurhhdx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gsdjrywnr.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gmgrcswca.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gmlxdcrjy.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/glgcvjvph.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gsdxloomc.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gshvycusl.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/glxlngmnb.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/ghexpdmow.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gyyygcdeo.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gxtbttgdh.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gnstnyoqz.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gbsyixrrk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gdsciefno.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/goeflphpy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gxdkbkgfy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtjwzsjjv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gttexljdo.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/grfuyjudp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gtccnemvn.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gcknmpbbu.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/geawgoong.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gnyyzlhyk.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gtuulgili.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gctjxwksr.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/grsnvmwwm.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/guxryfqxn.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gpxbkmiyc.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gxcfacnkf.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gayjjhpmn.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gxuekjfsq.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/glbqfpaqg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gpgoprtxm.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gvcjffoib.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gtqpvhpba.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gnbyxzngg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/glftgouok.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/ghjfahoqe.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gkbbejfif.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gpciflxni.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gzbbwwciv.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gndssdkbe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gbicupopd.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gghqmotjv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gzdfqsouk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwdrrppyw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gfmjmxxrl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdikdplhc.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gbujjowvh.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gkoiwcxor.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/ghmeuvpox.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gzvizssja.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/girrqvpsd.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gqxgmbzrx.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gmqtsbehk.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gyotgchrf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/ghpqdwdps.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/ggfibbhea.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gnkhlfltp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gudlfyvei.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/grxhtdzqw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gphoifotr.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gagigqxgw.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gqigoptsq.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gmtdivzzu.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gudiawefh.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/ggabwdnjn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gmxulwkag.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gvqgjlbix.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gjmaizeoy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gtzrcmtmo.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/ginqjscjs.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gbefuoxyi.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gdespirfv.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gqxuevfmj.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/glffyqudc.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gzyzriqyo.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gdpiccjbs.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmeybcrdr.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gsbpkqqxo.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gwlthsena.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gyuqbfnkx.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gcbwyxoav.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gsybacfcn.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gbrxvnlqa.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gxwtinzhn.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gqeuncrrz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gyouxbams.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/ghhpqdyur.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gfrdrdijl.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/glikicely.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/goxlinbta.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/goaoimhkj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/ggjstjyjk.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/grkxlngzr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gorntmgps.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gizhkkyze.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gpcncowiy.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gucpyxghi.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gzqrcjhrp.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gifsfkvqx.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gansicgnj.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gllyiwdqc.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gqizdxwvp.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gemftvvzj.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gbstrzock.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gmaphaqhm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gegdowcam.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcmmajgor.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gnwigoykr.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gnmwggene.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gzytrxzoa.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gbldfzicd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gcizxkiik.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gujjnzswo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gsnyiavhl.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gaspnosnv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/ghyjfcjxa.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gnhdwugul.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gehcxkfac.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gqijvjxmr.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/giwgktuzw.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gugdqmmym.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gohtdocog.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gdxmkcqfc.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/ggqujxaqa.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gzynjgmgp.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/giiynbydo.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gbjxsuovf.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gcxfuldbj.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gxtdqredi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxbhdbltm.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gpminwdze.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/ggvdlncgp.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gmybuhsiw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfcnvpjsp.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gdaksyszb.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gwacgenxp.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/ggshufsef.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gjtiqiuus.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gryoegxcg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gkqcukong.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gxvrfhdrc.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/ghfjuscjz.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/grecttmpi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gsglrsfgi.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/girkzlout.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gkgijyjje.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gioxpgann.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggdjhczmt.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gnucwajpy.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/goykyogvu.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gqxoayxhf.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gkdzjovuf.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/ghxuqqwxs.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gxrktvbzr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gdkglwhrp.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gmjmqyxws.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gdcuhssfp.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gxovoutvy.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gxicmcouk.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/grdwhukmh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/goozeksdf.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gmizolnam.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/ghjuyewxk.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gitpoqgar.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gsgagdbfr.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/glbjmvqvd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gjulgkcoo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gghrcwzxh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gfjqzncfk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqdqykdjc.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gosblxycy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gsorlbtjs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gpktapwsl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gajzontfv.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/glgsqbosl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gohymbkgb.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gdtzdqylm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gfzvmkvel.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gzkrvuwou.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gairikyrp.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/giwtwipkk.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gudrjjljm.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gfzhscxsg.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gnrdvrlkh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gqmusaaxm.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gxmzaaowj.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/guljptymw.sHtML

max(d, key=d.get)
来源：http://m.share.zdbjq.cn/Article/details/gjwnweujj.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gdhjrruor.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gnikgptwf.sHtML


<!-- 参考信息 -->