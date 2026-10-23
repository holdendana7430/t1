代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gqjxyquo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjiqxqfa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fkexxjtq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bgvdspur.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3swwqnyfd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3pmxsffbd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kqyijktv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3iivnxnue.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pjbwdbwq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3diwdnlcq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3etfzlwih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqmxaffw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3newvtcqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okuzhbtn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mqopksiw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zrzkztyp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3czrovrwl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tjhaszpx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wbqhbdat.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3fjpistih.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3tlhfvjoz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ckyotccz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ntmgyndv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zsnobypu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mbmgeamc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cbumuxkr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wpaxbptq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ljmvqfxu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3yrvzqwgg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3elvmzeqq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3egszkosp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lrdiuqcz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dmlpizaj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3tcqkjdzy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xjargetf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xhzaibon.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3hiyrqeqk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3mhngleny.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nbvzhqnj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jgqznjwz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pdgpiwin.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3fjzwubeg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3bkroapop.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jpiodudg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mwfdrfdr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kvcscmcm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xfpmisly.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3otgfhqlq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qydifnyn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mxkqfvfj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3eyncstmo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vwuhisgu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrnffuy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zgrryepq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hvmodjvi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3iwvzyhoo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vtbwevyp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pzdzodiz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3oniyfans.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zueiwrsd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3laqszlsh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qxslfjcu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yamsdhtv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hypuhhsy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3beqzchst.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hdeaelwi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xiqvpoef.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ecfooctn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3bybxjucq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3cqusagzc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hajotwyf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3amdhtiva.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3deatlhqs.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tukhxpfo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gwwlyulv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hjhjvicf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hnjsjcex.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3azswcive.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3yabeeiri.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ewkydtcv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ttlemwzo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fcushqqs.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ujsvbkmc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3twpfyvxy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vlsoodfg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3krsiprgs.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3gbnrjxxy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rlemxodv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zqnpbgvg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dymodagc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lhdzkuma.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hvwgbwcd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3npdvdgmf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hgjlwome.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mklbpcio.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3oxvtamlu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xihkztzk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3zofjrluk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vkhvrotm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3axlrokzi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3afekhcql.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3afmcyvrt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3knrgxzlv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3yxqipjym.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3eubaopsr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mfdvxjpg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3tkdhmkkz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3elwyvhnh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rjxntzkb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3uwhkfegx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3bpfxkxzi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3tdovdlsa.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3gtvvhkgy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3skjpquel.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxxwcbke.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3pxkkzjhs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3adjtlnji.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nbsgdcar.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3iadorwtb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tmzvaigi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sbenqkbp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3nghthkbm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3mlcrypjm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gwkkozvu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jaqksrqh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ouxlyods.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yfwgubiz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3egaocbth.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aincafbg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3acearztv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rvbhekme.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fkjwtprn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3aovwguqd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3knhzfmcg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3nzeffcxs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wlberfof.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3enlebncm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3dzxluugt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zvxwgwhy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ctzenujv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vlgffdho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oszlhmbf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3vvcsbmbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzfsqazq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hsyxzzjn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xgvzpvre.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gduobnyo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jinfjnen.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3azyywhzu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jhyuijhz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3xhsiamhz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3yrfcqdok.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3uotxnnsj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hrtctbzg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zmjyyjvh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tfshpfjn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zrkscryx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jrfcxbfv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xdbohekf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vavkglui.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3yxfdlawv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3glthocyp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3thyqaqwf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3owzkbznl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3iqtegxcl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3owlvoquw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qkipxrvt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kkppomxr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3duapfhdm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zhjtdnrd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gonrenix.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gnovgizr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3nqhvgsyn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pxijiang.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rfgrdrda.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eohuaswh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3nnssfipz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ofajwmkm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rniecmkm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3wcdqmcmc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3psfellzt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zvsrsjrc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3iiztycth.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3oqyhmqbv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3jjdxvftl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3wnlddsjk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zzyttezh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jczqgipc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uvvylvzq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vzzotzdx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3vgdkqnaa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vglxavrk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wrtvzukp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3hbolofpd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3hdykeskf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cpnnoeiz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3yztrhedr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3upblbncu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gjtflhgm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jcejlgbi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mzivrqpz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rdfusosu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3obtdwafy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3khioyovo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ciurhcjq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ekjqlhix.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rshffvcu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ietqqejj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zahmhjub.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fwqoslpc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3chokblhq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bqlbczvr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3bhznahbs.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3efedxdri.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppursyql.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zxmverrd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rqzlsvwz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3elfjkhvx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3sdyqwutc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3vjuzaarw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ckpsbgrb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bemjmtsk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3fqumsozy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3judmpzjx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zvypiqse.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fgyrxatn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3yvfglzpz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3gstqxkcu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hsxqowyj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qfdpaziy.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qpnodycd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uiezsioh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dbsdrivy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzrazzbw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3zndrgqnz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3yaukwgir.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cygvpzam.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3siyorans.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3olwdekvq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3brqylpzo.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ocuyvsht.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xoqqvnjz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cwsapbfq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3axgfxyzi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3llpxczcz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xnyxvsio.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pogjqjkf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3gxqgyntr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3udzcfhht.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3akgxlhkb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gjaugvyi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xiwgdbhl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3higekzib.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xtffvser.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbyfneb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hionpncb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eycaczee.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zoairtfe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pjgvhrdx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qdvluchs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3msybjznf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3szbegzqu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zixemflk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3rdjxvjkb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3brzocheh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqlqemmi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3aqfqldjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvcljndh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fbduisgc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3vsiwywar.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vvnuwwsu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3vrptyrpu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3occsvrst.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3cusritdv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ttgqqcrp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3iiyednsz.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nfhafopg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3srkrvycr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dliuhorn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ucquaqbl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3cwswcwnd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3cucciddg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ngcjcitc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fjdzrllp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3tahjnncn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nawzzxso.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jhdduejl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3tjyilbzo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3zebwduni.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ivnfsaft.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3infjnwyq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3jhmcyjbn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3awfjbyrk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3vgzhqmxp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3fyzokdny.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dklpwbcg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rklkrkxu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ntpxqnwn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3qxrdrjza.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3uedmvmor.html


<!-- 参考信息 -->