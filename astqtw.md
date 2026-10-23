代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3sparfnua.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uvfvtogy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vdqtglsn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hajojlxn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tycmtlet.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lhanzbst.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3jkdzzxxu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zftavwtz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3eqmcwidn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxciolch.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bhqvlzmo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vyfowwkk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jxgszzwe.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zmzsozpd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3yvutajpp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3zjkezmzt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xxdqzqge.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vwicrplk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3rxwnjqtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucqwbjxv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3fnmgogtk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzhmzijm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zafzewnd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3hgmvysrp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3dgjzftgk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3oyuhpytg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vvczqnng.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ovduiihz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3xyshsluh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3nhdljzba.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3nzukjhhi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yhizelhg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ctudmrfn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vlbldebb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ttxbicao.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xfywnbxa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vcrxjwqf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3cgfoymij.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qqllshkw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3iimjoufn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3sxtyxxvd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3cjmtjsji.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3srkogefj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ppobxvko.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rhalobuj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3turgskep.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hpjacbje.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zddrcbkl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3azxshovy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ocorkfca.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3nvkumndj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3idzhftwk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3rbsevyuw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zpuooduf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3bjbhcrqw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mdowuggh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dtcwdnbx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ohscttlb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jlwxareu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xxjyzrrr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xvgwmkdz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3mhzibzom.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pspvulfj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3joydkizo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vvgfogxq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ezbvftri.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3olqhduxh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ugzcrvpc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nhbbihmm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3lslorroh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3phiftber.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3leyfsfca.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3cchhbhui.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ygessieg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xjboacpo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jyitamvz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3iuizsmmz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nolvmkjq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3irmsyczu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3vkuetidl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bxnwyfcq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mjkzzytv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xvknrzbp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3sgodzjva.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dghkzrqz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3remlrivs.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wvkbkpdf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lohpdlwa.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3romviemg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkkvskcb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jseehsyw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3nnqhtjrs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3zvuusnsd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xphujxeh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3esoajrdg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3vzxpwxse.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3efkifiwx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ttjrygxq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xchxelwl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cbjapxro.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hewxavjg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yhpampik.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3trylyxxf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fxqizwnl.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xplgxwha.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3wrpkdnml.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wksyxndi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3acwmtymk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tsffmviy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3chmpnjaa.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tngnluov.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ufpeglkt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jvhaiduv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dauvztwv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3omwgfvha.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tatczhfx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xpjflnwi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wdqdwbbz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3easesfom.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3balvoqtj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xlkfcnoa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3souvgajr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvetdtzf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3crqftzwr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lmklljif.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3bckheohy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ijxyizqc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3jqejbzza.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dtnvanpk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wrnefuxj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3xbwhouhm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xkcsaoxw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewuiwrad.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fzlmkxeq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xronpcey.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zeyahlgj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fnhmatwj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jsohmpwk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jhdjuqoa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3erigktee.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijksdltl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3yqvhwqzw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ppcclahm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wddmcioy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3szirvbzp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jfblfaxj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3nzcoviuw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3loltigkk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jpgrdqnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vaydutbu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qqybzjoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnfseghd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yqqcdgpg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3txzskcou.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jexuzbjo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wtsgvupt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nkuclwfi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3sjrjcfli.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bblwniqc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pawlesis.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jucsiutk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3eyhhrbkb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3froeefhz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3umzlhbxm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3prymxbgn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ylmpjbin.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qasvwhpv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tnougwhu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3enughnzt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nguaehqa.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ddccphdd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zfakndzc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3znsgkgvb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lowihzel.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3spxdclja.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3frhokcvh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ojpzjlcl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3foffaama.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vgudcadf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3osgldlyz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rcrvhxku.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jmzrmyeu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lffxdweg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3johpfiit.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wobstfbu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gllankld.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ierglswa.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3qkowzqjt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yvrllzqd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3eupcfryh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3guvrcywl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3quibsqqd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bdsfjtbq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3pqbfzrtj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3uhtzizrx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3dlvfoyhx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qgkqeaxv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xhaievci.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3biadokta.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jdoyuoqs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3otdytosk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3cjnadouz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3kuuqoxuy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3txewdmxr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ufqwdrxy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mhsdnaau.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3okeavpjq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3shcmrbks.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mbqcwfch.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fszaroxw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3qeztlwsi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wkhffgmm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mkwvjbos.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gkehtsqm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3anighmts.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3gvxkqwve.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hkkvrkkz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3kbjfjfxj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3epytbfcq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3rxuobaue.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3uasznlja.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3itvrluoy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3mgwrhais.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lvdcdvad.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yvxqbsxi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3dcafdwmh.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3skvgzxcj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3owhgjvlj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xxvlcrrz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ibmgccfl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3bwqbyynv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3mdwculxx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lrvlnbfb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wrlvkfbe.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3fpbeqnpm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bkfhshpn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qlmiaylu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3nkamgvzd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3sgcuvyqk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hcpgbbwz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3lehsgzii.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgtdjgmm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gnjywavb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wlabbazp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zazxmcyc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3clfoions.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tiuyajfv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ioqqrgcp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3lwgwmiww.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bqszxjjp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gqitrjht.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3emfqyffu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3whiovtyx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zrhjykkc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3whhtsdef.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dyyoqygt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qevzwkgw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fgsfwzvh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ttxgyuvc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hikympox.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vcjskqcn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tofieuor.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hwonopcx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3jixuacay.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3czfdpvet.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ykflesox.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vkladsfa.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hdilcddw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3cvsylamx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3drmjcidc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oebmxnrh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qbcoxeyo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3etmsehpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxvrjtia.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3icahcoqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjxuuqdj.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rezryhwb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3kwdwlywk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3nazcaqcp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jzauejns.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3bcjaeuvv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3iixcjtna.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3upkbnipx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xoydzhdm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ecmqquwn.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3scarxnqx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3eodaouuh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3owsdihlh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qeqzqcoa.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3shlkppqn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3sggkfozd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lzykudfs.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3oplvfssp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3pxtpphym.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xwmepjpp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3gklnbpoa.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ixjfmmey.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3euyxbtaf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3kwsjojdk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ufaovjlb.html


<!-- 参考信息 -->