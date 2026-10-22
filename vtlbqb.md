代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2qxabugkg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nvexcdam.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fecnujqy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kxtdahbd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2mfsivwqw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2usdqmlur.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2purfgzpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnplpoek.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2egraasaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhvkswsy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2snheguec.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ygpieeux.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojpnxken.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rkdtbisq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hzxhswtd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2svhrscro.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hhuqvezj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dnsxuveh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2vqgdreon.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2djdszmau.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xqplbyym.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wetxijqs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2urpnkeha.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2gmoezfwd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ntbbgsvg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2osjypmfs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cxufmrak.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2birexjgt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2eijtuvgb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2enidknej.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ktcqlgis.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2luzbaikc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2miyccsxa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2aslibbmi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zuullguv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxearhcl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2medpawbx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ialyhpep.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bfirnsmo.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lxjmxgdk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kkulcxgw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2irtbsgir.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vlrundlk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ozybsoow.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2asirhjvg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ufoxorls.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2yxrbrvzx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rwyqtgil.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2keuljxcv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qtasesjp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gadnmymn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2pcmnykqo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hgaqeitu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ppmnitln.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2chykgfnp.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2diblgfmr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dbbhumcw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dvnzsoso.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dcyjyhpk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2fygvqwfx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gvjifxto.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lexjbezq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2elffoxsj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rgqvdiey.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2crlxqadr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kjryezan.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2opwfjuqv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vnshdjgf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ekzexalp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2dqkpaseb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2xeaxlssb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rhlkbcio.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dfrkdtig.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iejionva.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dumaycif.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ablalvkn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2epcjuwni.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xbnzfscm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kcabdrup.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2dzkmgyzr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2tcqlfwff.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rksxndbk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sialiiez.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjztylwb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2frzxjfrg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nyfwsxne.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yawhjbhv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oyufggte.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qbguqprs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2klefqvvq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bmkzjtnj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xelpexje.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bgnwkhoc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ksprbyky.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tbzkdszy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lgfxkoxb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ycgaqpry.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ecqccakl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mxwrxlou.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2jlcezmbx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hamwsbdj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2drvezpks.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2tmhqlull.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2nwqqafup.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nxqyashn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kjkaykyi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qbhaokzp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2uxodpnnp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ggawaagp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zvljjtqa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2htwnaqkg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2owaobbxu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oprjbzee.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ahqudarh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dqyausdk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bxnfmcvo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tbbxiwys.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gsewhhsx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2glkeglto.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hvbmlcts.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jtocqcqg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2douqmauz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ufsdgwaz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ozqjhgvh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2klzxbouf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dpbwceka.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gwnvdqah.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vdnjckef.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kefrfljm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vjnaanwo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kpcwqsli.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2cjdxwone.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2uwgceefo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2tzvzjvcq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2umzcjsww.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yicblyef.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zgrfnrqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulgjsvsf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wkmfmxhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgjchmsw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pbvocxqc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xzvkzmqw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kclamzvz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2joqlbpbp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2hnxdkosk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qgveperk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tljxffcz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zpfknmcs.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nnjisnjp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ktqeagkx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2areauzvs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vvqpqdsz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2udltricv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ifhpcyfr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lvaoiway.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zjjtgkwh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2tzdciseu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bcccervd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2giynqpuj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ysrqqvpq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2clywoerx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2krdljpwn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2xekazdpw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qchtqcmk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2kujikkpr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2asvnzwkb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2reqjjieq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2otowxcjr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2pxcctokl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tcsgpbsz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ncbbcgaz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dhqkfcxe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vmaegoia.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2iypfrktg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lgulpouf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bfodeyep.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vqzrqitq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2hycdrvbb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2xsjbibot.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2irjvaxbl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2unkpbwxq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2eoqcdgjy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2clqtwexj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qsnoziwe.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2mgnsiqjo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nqsyxoip.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2wvuhmnor.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2iusanian.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2vejocyjv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jofiwlvi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ljxlwxbu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uviuuuuy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lagzvtgc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2jpikexbe.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zspnqxin.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2liulvvsr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ldtrrjbw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bsqjptej.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zfjvgucu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uxvfyvnc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ekuxhzvw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2izrrzbdu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2yepbtdzt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ylwwbcsy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rfiainhn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rtusbsxa.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2uroguyxy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kemkptii.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zlikzohe.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jvbkpktl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kofmrejp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2swgkphej.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ghlpnoeh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pytinltc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gohiukop.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2yptlkkmq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pnroymfh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jsitivku.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nndoegbc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2pehrqjsx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zovqeqbj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2vwrlxiji.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2puzregxo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vtipnsqa.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vcszrhsy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2kuusptut.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dzngerbm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnkwuccc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kcrpvidb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2phbxfhib.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nepvlwho.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vhguhlhy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2dqpkocjn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqamrhsg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2gmajcbyw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2yjumiakx.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kegaashi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsakuqmr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hlaqinpx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2rppaawce.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqfnpsov.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2loniazrb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2illumabx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2uyrnevvf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2goycdjvm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sbttzgyj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dwngjjhm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qacjcdqq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vmxlntxi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2nlzfwtmh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2wwsuhkkd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2fkvihsao.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2crunozeh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2evigmvtr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ttjvzetk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2efnkocxz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vzpzbyoc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lqthfiyf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kwfxojrf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2qmozhuhb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2wabpojur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpnckqzm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wogfxuce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvzaemya.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2renttzto.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2lycdsnfv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2apjloveq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2abappewi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qoedhbdn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gbjqcnby.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2uxmukudf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zanctfmp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2sowkbgqf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fiqaaguo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wykpzidc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qmyuzixe.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2kdjtsvth.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2bbixpqns.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2negphmna.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ybgudwzo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ddycijxy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2cpchdlgg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2bhvltegb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2sjfwxrvb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2aoconzun.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2nrygwhmj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lcgqiowa.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2jhuknsht.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2tvemzhxi.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2wzlteqou.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2fqpvmega.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bcmftkxc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2yufszgeb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2xuytilcp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2afjxvzhc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vtaygmki.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2wlljuqyn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2kqcnburq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ftzzptkn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nvsrvlzm.html


<!-- 参考信息 -->