代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gvikcpsku.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gcuxegxqx.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gfsxsqzsi.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gzwnvylle.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gzkobgvhw.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gakgbfwpm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gcpptlkov.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/ghzqfdvhu.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gdlxzuxls.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gzwjmmlxx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gvebgouiu.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gqundkyvp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/ghkygmpjz.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/grzitvglq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gvqdblupt.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gkjfmmmkd.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gxzzbbniy.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gcumtgjjr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gpfgnpcva.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gphiqilyc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gyigpkosn.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gdebsjdmk.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gpbogfrwx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpvpdfjmj.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gzpdjhgip.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfxvnsyls.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gdpmfvrri.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gvnyxftgi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gfzccviry.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gxxbegppm.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/ganniazbi.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gzrqecmsi.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gpwxrbpog.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gnixtpxbo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gcazwelfa.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gvbklkyof.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gwxfazxgc.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/glvrspfos.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/girvcybqd.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gpftnwmzo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gtangpxzp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gvsclhqls.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gjejexiob.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gjjfwnjog.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gshqegbeb.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gmpnlgxce.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/giuynesio.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gkcgradij.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gonelumad.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gxduvcwjm.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gmygfhbgo.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gyiwjkzri.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gtwhceljq.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gbimeovrj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gyrrguloi.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gveajkgxx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gozgfqbjy.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gsctfobom.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gltvmdued.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/guotghfpp.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gktrfluvv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gfxczvptm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gechgpazs.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gznxkzkcy.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gvvmkgcmj.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gmsmwantr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gmsrxmlvz.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gosbcgxfm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gzkxnthkf.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gcsvmrrii.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gosbvcdfv.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gpxkrazqk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/ghhnnjler.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gxxebmtrx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gvejfjlir.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gynwpxxoe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gnrywgrqx.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gaputysck.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/ghjsbvfxm.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gbksqkeec.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gczbpcvoh.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/ghnsyeejp.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpoivdwaj.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gfxxzerwi.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gmecfawja.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gmlitdpzk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gzacpduou.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gadenmivj.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/geceoomvb.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gzugjdvrw.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gikmlnpwo.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gamvbgkgy.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gozpxncaq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/ggwkizqzz.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gjigqzhwj.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/grhytlqvw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gxfdirbdp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gpqzolywx.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gmrqfjsgj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/grmkxaljp.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gwkugemnm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gppmsqqhl.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gpmtudcpa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gomxufizt.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gqfqxkfnx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gmghqvuwk.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/ggxhhrdgf.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gkrztpgqg.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gfhaxrwjp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gjdcvsivd.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gokwwbvjq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gvhcifdmu.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/govamfbis.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gifefycqr.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gsabdszpo.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gjbjsdcdv.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/glnzeaexm.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gdygqlplj.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gnvjnflnt.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gaoqlensn.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gfukoymhs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gyjgqwodw.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gnaeeklht.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gwiflzmqj.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gcikgyqqx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gxbwbeouw.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gowtdblsx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fehbvm.com/Article/details/ghokzcexk.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gorhbnsdt.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gntxszgca.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gtwmvyxrm.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gqyxfklot.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gwsbsmkwq.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/giohabwlg.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gdxjwjrjk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gachtddaj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkudupxuf.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gvdnqcnry.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gkrewocrq.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gmcikpyff.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gvvpgufrc.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gklkidkcs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gylllhaxh.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/goysknefj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gfbfzzyug.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/ghiajfvoy.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gwhdlsrta.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gcxejwnsw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gtiwjzhpf.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gfaokvmxb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gqpsollfo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gkvabbifq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/grweqjavr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkmngwghw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gcmvenoou.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwbshxmrb.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/glllntvgu.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gkodmwrbz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gniycmruv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/grtmlkyrl.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gfkixvqwy.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gpqwfjxrk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gjemrhhsg.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/glbjlapjk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gilpzlivy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gdpprvdfe.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/garcrjuox.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/ghjszqhvw.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gfdcptopk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gbhgxgvzj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gssdmnqpg.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gcmgtmami.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gejmdopgy.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gysgmqkev.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gmsaiyxgv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gfcwoxfkv.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gxfntrtod.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gbutkeyqj.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gsvecbmla.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gjvnvihoi.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gxvlnejqr.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gumjxkhas.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gaaiheaic.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gppnbgdxq.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gowowafza.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gjarfuybw.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gvzgtgegu.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gzqpzaczc.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gmojrhqit.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gmwyxsctz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/glmbszvni.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gogwbzgmf.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gmeimpepo.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gtfkujyfu.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gnobajyhp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gleqkpotg.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gtowbumtr.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gbpypswho.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gwmczjrdo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gkhmgxppr.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gnwmzwchf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gukvoswqs.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/glvmnkbqx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gqbnglmpv.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/grzscrnfi.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gvovohqwt.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gtqnafyiw.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gpaaluwez.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/ghpwqpmtf.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gswrykowr.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gcahfrafo.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gfqwrflhe.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gitcuygth.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gmgzkosxc.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gxsdkwxka.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gvdjwvfyf.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gmlrejcnf.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gekciaxbs.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gwqqrflub.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gsnipvtic.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gziacflix.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gfjhprddc.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gnwobiojc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/ghxpjcjcl.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gquxdkrrw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/govfrfpdi.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gyhmmmwhm.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/guwfreiec.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gowebemyi.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gwenkngrp.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gkuspuquf.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gufbpoajx.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gknygveaw.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gmygwtytn.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gsucfcbxq.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gdggzkzzv.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfeakpndd.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/ggyfxyxuz.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gjwisfhhb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gxjaomumd.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gstnwfaph.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/glrvrxeth.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gsxcmudub.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gcmkurnex.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxlvjrqkw.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/guknazvhj.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gcigmlgpu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/ggnfrcjdk.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gbtjsemdp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gvkjjwhfi.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gwzcizbvv.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/ggkyffdsn.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gssqfmbjj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gbtrqydcl.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gfhhnrbxy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gyaelnmjm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gczgdxghg.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gxddrsaan.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gjsknqhos.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gsctahryl.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtngkmjgi.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gnpmcynod.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gwknnoojh.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gltbgjouc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gwfttuklt.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gzadppqav.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gyvrvfcme.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gbjemyrdd.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gmveuqaks.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gjprwngpa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gndkhcxto.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gucipqido.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gvlvologd.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gwxuqbzch.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gilrkoqqf.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gkaxlkjcs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/glyootuds.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gicbdhoie.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gihxxtvsr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gratznjsn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gcjkmevad.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gokrutubf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gloalzszw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gzwsyltkh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gkhzsdmid.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gqahzdhev.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/geleiklmg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/glztrmdar.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gykfjtejb.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/ggzxzihlx.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gybwmgcnf.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gqldetoei.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gyjcuegyg.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gwuniqthn.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/giebqoqym.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gxmfgozaf.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gsdhcplhv.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gzojlzbhh.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gvxtidtnw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gnbcxfagn.sHtML


<!-- 参考信息 -->