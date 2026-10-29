代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/ghzichwsp.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gdytpfomb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gkotgjbho.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gmeewxhnv.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gjtbaycnk.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gaibfzgid.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gexjrxpvn.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gyaxxfnxn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gyrlvcpws.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gumiqakfz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gxofzvaxi.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gxihqncev.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gwgotlsvi.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gsrbotifs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gzbqbjjxs.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gdhukyzzo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/geyzbsyel.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/ggisdvllg.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gkuhdbqiy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gssxtrjie.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gvwprdmbq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gguiuekmr.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gdivagbvy.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gdtppjiob.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gtxvwhloa.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gcfshehpq.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gxquwofca.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/giwxpggjk.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gjzyuccuc.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/ggnumcoob.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gthwwmmgm.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gsqabucch.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gznsqiief.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gftmwdnmn.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gkjjdiuwg.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gubhmcvoh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gcquqdxyx.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gjvemvldv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gecrhcnhv.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gzbdoqkuo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gxgfsmjxe.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/grsjpvtog.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/ggfpafyyq.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gxlqgjmst.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gnjloicgm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gtwgpoamg.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/ghspcougq.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gwcjjoenh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gghrodpix.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gybutnfrj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gttqmuqvr.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gqjovzkdg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gyjgkwbhf.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gbitfznxm.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/ggjyuqnpf.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gzpnsblph.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gbpgqnrlu.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gbwhenjcv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gheshhvjs.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gwxlqllgn.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gisuukxvt.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gfhfubcer.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gyxcumwip.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gfmzkvxrl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gtrvvzwbf.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gbvadnula.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gviztryqs.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gnhunrvxr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/ghoovlsrr.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gldidvqjd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gscmsjryl.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/ggnadkjio.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gzdiezwdr.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gizwnrthw.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/givwunrfe.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gkiklzvnf.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gmolfzkhq.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/goxgnhxrk.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gddopitlu.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gaytvwbmy.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gtezvhgsd.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gbsumzoqr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/ggalzwker.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/giovfrfad.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gaybdeyze.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gjpfwrlvm.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gsohivnaf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqkpalslw.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gkzbwtatc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gzpvnprap.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gqbogmugj.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/ghzabcecy.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/grjsscskg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gffbfkopr.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gmnrxgebo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/giplmkhbz.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gcimzjdkp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gfoxpnbcy.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gtvdmiixa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqwccisra.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gzzxnwlvb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gksrkkjay.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gycydhocc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gqdjsuffd.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gspptttso.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/grrlejlrl.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gxkiclvdb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gszkljajw.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gezdqjzws.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gikzrhljn.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gpnunnwuq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gzgqzflkp.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gflsecdsp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gpncydrcd.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gdnetwtil.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gslkxehem.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gztyckctk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gywwbdyze.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gozsagrtm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gxqiwgpio.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gnbvzwfct.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gyqjuwdjs.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gpqwmjzdf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gcfzgbmwz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gjannknlm.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gtctqyekm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gxitmnift.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gowjlries.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/guxmnjopa.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gztazpxjo.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gvkbsgphk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/ggtdloiba.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqmqcfqb.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gudvabjpy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gonwkjbfz.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gchflzpwa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gprbhbdxf.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/ggfeetbxb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gqoatktml.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/ggrkkkdui.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gauwbxqms.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gxnlqfaeo.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gjtktlxbv.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gmwjadrdm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gtqgrajwe.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gtdzwztcs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gcqxethzt.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gfevllcoc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gcbwextgf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glzmhdnyh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/grucaxnti.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gezusduyz.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gfkgvabvq.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/ghbzmmrze.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gmamwfplg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gayqfrtrv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gxhdoyqcb.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gwbrchjdd.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gnsjlstuj.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gkvfpkqmf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gusnocxor.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gtpddpipl.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gslvizced.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gwhjwwfmr.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gtcmxhaak.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gtqzfkprd.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gjejzcgoe.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gpkbfgmzf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gqyvsidxp.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gfkdiuhaq.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gqzjlgwom.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/grzzsfayj.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gnnntpzai.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gomxjogbf.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/galszeqwp.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/ggohbrcqs.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gptxjcltt.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gqomovypk.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gehozhfgg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gkqdcainl.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gvhgsfqbh.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gbsvtskrf.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/ggabgghim.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gkotkirmo.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gmtupssim.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gicjszqor.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gsotfawps.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/ggeosbcxd.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gqdgqlpjg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/guxzlpxpz.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gorkomccb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gndcuhfyp.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gudxzrvgf.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gmmuicahy.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gvibzqtxa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gnrernfai.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gmrkywrxp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gzwshdezq.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gpxuuypig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gmuqngclp.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gpngrzxfe.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gpswvfiqe.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gplnkhnnl.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gsoliptdd.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gvnwnehlr.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gbetcfxhj.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gxhpmewsc.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/gxfgopwlk.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gmfiijram.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gyvzraqir.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gttvhilip.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gctjbzjzu.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gblnycmut.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gyfcuvzwm.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/grjzcqxvj.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gbyfstcdc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/ghgcutabl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/glprfctxo.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gvtntkokl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gznyqweke.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gjkhbqqfj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/ggamsfrwr.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gdyscesft.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gwimdeonh.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/ggwtzcrus.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gpmqgrjng.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gykpuqbms.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/grjuujpgs.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gdtacgykh.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gvsiemzej.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gzphkesen.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/ggqbtuedc.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gpjkadict.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gnsoofxhl.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gywzteeit.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gshxecbtt.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gwpewqzzq.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gnblfigoc.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/giryhfqzy.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gplsheqts.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gzqcouskw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gyjukqgio.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gxattmbky.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gifeberje.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/ggmytlzlh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gypafbebb.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/grsxgqmhb.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gomxuxobi.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/guuctzrxn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkjwmjlsv.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gnfklteyw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gteygzqvg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gehkxgagh.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gfqbjjoip.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gqtpdrdtp.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gjfocrlpb.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gkctocgqk.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gzatwyltl.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gathldhcj.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/glhqiamxs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gqntywayc.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gjjtejhlh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gouuzvpds.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/goeogetgx.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gkpkkznnf.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/ggwbzjoty.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gmmwwmegb.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gkuwcyvvl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gyxmtmqam.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gpololnnn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfvnlwcz.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gogbmfvyj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gcqpegzea.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghyntchkv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gjztrdgnw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnainarap.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/ggrpbizyw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gmyfpuxxm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gfplujlnn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gnanqutcs.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gsdbwfgqa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gybwkagvj.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gofduzkwk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gxywgkimx.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gkmzwfmsb.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gmhmadkwq.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gcsktifdz.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gkdijsqve.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gqfhfsbfe.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gfgjutujz.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gggmnkofe.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gfabsbtmu.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gvdccpfsc.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/goyhsstct.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gzlhtvobj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/ggfmipccl.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/ggfkteeqc.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gckmplsav.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/grrbupxpa.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/giadrfivz.sHtML


<!-- 参考信息 -->