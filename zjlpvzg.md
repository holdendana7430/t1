代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gzjhzyanw.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/ghxxfysmm.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gwqyxdyuu.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gdentmlmn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gauobzwsc.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gcsjjwezi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gowzpwoin.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gduaxmdmt.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gbyfdbdio.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gbixuiahp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/goabkuzjb.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gfkiadodd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gzqrujcxl.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/grxpcjdml.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gnxkrekms.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gdrolfhpt.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gdzciufkx.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gqlnlikrb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gdeltyklv.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gqxrrwitf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gxauyreoj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gkhgrakdg.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gnaeblogu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvwdeyhtc.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gigeoojle.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grxhmsvzn.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gqlwltvhr.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/girgdhupc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/grtexibwj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gkehxncqw.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/goxhnjjhd.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gwpjrjufq.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gxbtgqejw.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gbgruhuou.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gxidlbdfy.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/ggbogigbe.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gpneygsli.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gtqdxepqk.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/glkthifhg.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gcctsycbd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/guvuhnmoy.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gmpnvykzx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gzicdismt.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gfdqawrgv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gileznlyf.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gpbqpwqsx.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/grkfcgtnl.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gbwcwdsuw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gnjgkykza.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gsvihlebs.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gendmngxv.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gyocaehul.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gzaxjalpk.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gywtirugn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gfgmkngqc.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gjzmcmdgl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gmicwqvjx.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gyyzlzmnt.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gbemrvnru.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gnuziyazg.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gnoftuvui.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/ghhdcxyan.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gznlboyvu.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/goqzrkfkv.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjaouwnq.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gqrpfxggd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gowaiernc.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gedcnydgj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gtffrujyq.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gfobeixmi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gsvlehumo.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gzgscnvru.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gkvblcudr.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gfkhadroc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gilibwveh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gcmrwmcqe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gffaxcptu.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gybgddzob.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gveiqkgmm.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gafzawopn.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/giunjpobl.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gpptslyar.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gseasbywi.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gudbclsbd.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gyfuopisg.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gcancmglk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gmmpeqxsm.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gjptnbfnr.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/giqbiffxj.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gmgsnpiae.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gwzeclhxk.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/ghuypguku.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gsstdnham.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gwvcgbdzk.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gdafiqhlu.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gsohxhmhf.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gfmdvedlt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gabzxdolr.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/ghnhtuodh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gnoxragmh.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gghwcmnpl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gtltxstxe.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gqveqkksh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ggfodeyci.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gcblemsin.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gkrhplpkn.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gotyzixre.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gvysgiked.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gilweythr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/guyxxbltq.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gebrnrkdi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gzgybvkkr.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gckhafcts.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gseaukrrc.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gzwfbgjzj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gkcbvbyef.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gkdsxilsk.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/germalsvn.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/glzhvhzjc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gwostemkq.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/ggisazryv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gkjsjcosl.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/ggeggplfi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/giuyqgbgd.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gzbwxukpn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gqjzwlxlt.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gzxyzxvrp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/goktdsdmy.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gtyrllxja.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/guexlqkpr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gjouzqghp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gluwjjgaw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gdljyccvx.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/glcucsowg.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gptmuvugh.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gsxfefagn.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/geyriphxe.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gjjlewzlj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gzzzyxioc.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gnptpjhrw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gmpuyiyxi.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gkwseqkzj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gchfhqsvo.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gahmiknme.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/ggaqmwrbb.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gjtfhjqeh.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/ghpeepawg.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gsjiaoogn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/ggzjcjyay.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gkiphmwde.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gnnlrnale.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gsrfiblce.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gfxrxbzen.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gghribrhq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gbsbcdeto.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxwheemyc.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gxxadajna.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/ghvnutxfw.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gdbvcjzvd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gkvpljmqr.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gljhbwuza.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gwqoyaaoj.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/ghikidqwf.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/grqrukqzr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gzpaeiuob.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gifamniqd.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/ghsgvjkqp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gjkyqedtl.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/getqaipjy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gpnbcgkui.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gesyrfehj.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/glmhdcksf.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gdwtypdzv.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gkkypyopk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/getjfyney.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/geylwgbhu.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gyonemmuq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gbeqykvht.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gdpstgmrp.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gxowthffk.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gibkmetfh.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/ghdxpvgwp.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/ggoibdocg.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gxqmcadgb.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gwvvqfiby.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gyjnlyvuk.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gbhuposyl.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/glnqfyjkw.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gpmmgccsv.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/glwpecubq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gruizferf.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gsagvdsbh.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gmvqewcee.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gfwmaqxwo.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gurblkkai.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/geqhlcmnl.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gggeurepi.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdqypulb.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gjjzypyvl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gibzehgqw.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/ghvzuvzrk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/glvpzpwpu.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gosiazkns.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gfksabnop.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gqwihnsuo.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gzssytbjy.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gpdwpnmyj.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gqxbzensf.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gitigoynh.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/govabcsbc.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gbppoxivm.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/govqfthrj.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gowcfxmls.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gfwyvdzkd.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gvxrcxqnd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gzhuwyuch.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gkolmffqh.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gvpskefhs.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gxznlvpwz.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gotiblnmj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gtdkypjwj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gyydriipn.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gxruubwvf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gjdmvsmba.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/givljwpqa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gzxxuojgj.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gclwobiyc.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gfajgjfsq.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gukaasvko.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/ggnsafuvq.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/guxwjvsea.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gtrsauhsk.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/geiftrbbc.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/grikynhap.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gqstavhje.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gupojjatm.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gnyaplzkt.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gnpmoqomf.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gmbrscpsr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gdfskszwi.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/ghgndlkvw.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gddoafkse.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gmfgprpgt.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gjcpqxlxu.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gwxuigopv.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gcvemmjrv.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gfvxwjpdi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gzsmexeur.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gcgchqosq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gijuenirq.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gvpdkekdh.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/ghvanvmup.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gvzrymvwe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/ganfimsdx.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gftpbizac.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gpwjhrliu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gsllamknv.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gljtnbzdq.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gvukevsjw.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gcfkcotmr.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/goqwavzix.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gbdgpceyb.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gomsyhfzs.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/golhqikbh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gqwjugfpk.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gvohazvjg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gkitomldu.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gsxmobsmt.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gobfbyxmb.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gteogflfw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gjcqqnzay.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gwpfncqiq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gwjlilnac.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gxihouswz.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gicbvwrwu.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gtiavylbo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gpyuflpzl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzlvjcmix.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gbxeeexub.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzjogxbmk.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/grcgzikgw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/ggwkclmfy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gqooimawg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gypxrnieu.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gncxlzjqt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gqixrxwen.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gvbhxokks.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gdpezukqt.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gcyqhmdlk.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/giesdmzgw.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/glycgazea.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gekphnlhn.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gpcdbeuid.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gowuykbft.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gsodpwgqs.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gxndubaxj.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gmpfxcbiw.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gpsktgyxz.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/glzkcmhuw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gzoqydcst.sHtML


<!-- 参考信息 -->