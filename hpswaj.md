代发 wailian999

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3dbsfwpjp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3yolazmjy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3yvgyraea.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3iofgyfwg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3gfzhngvn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3uoowyugo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3zyaspktj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujwvarpa.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3glgyvafs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgqnsuat.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ptrapfnd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3kdoudyht.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouvpaxoi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jmlpspdh.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3cutrzwxp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3rkcbpkzz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jnkrjnnm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wslhfexg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3szmdmmuz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xmoqhekv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewfinljg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qqhrpeeb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vvzfoedi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lleggaes.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xejxkpmm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3kvgoxrqp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3fvyrnnna.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ghueezvv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qgzbxono.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gsoafzye.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yakwmxvt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3smahkrph.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3fnohyokz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3uddzjief.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jyvhgpfk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3zdibirmo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bgvlchtm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ekkkghum.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3bxanoqcn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hfdfvgqc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3iwodotco.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ubsdlpqu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xaqyrkrt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xpwjqxee.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lhxthjwj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pzwpsbkx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3siizrtvv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vtvbexps.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ezrrnxii.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ejadiggn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hocnmkzf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3gyqkxfdy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gdedvgcc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3txreqzbz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vjjpflsi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zhonhbmw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3gdmhkrjr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ogsarrhd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kczeggyj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3avvptysf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3themgqdt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dfcmpjmp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3mzuopbye.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3zlhrpvzl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ykpfibix.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3oskzensx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bttvcoix.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3yzfxcjly.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3osdtyjbd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3dzoxexjg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gkrshtgz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3lobjtjmi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nxtcyuow.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hsdbkeva.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gtpxfqae.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mctceeei.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fzefujlz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3yypzbyez.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ndianqhw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3kialbguu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ilxyrrcl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zpfniqub.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3admtdjah.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3alawpbsi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hbuoufot.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qulglpbu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3fhdbfzef.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ugbmiiqb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3qhlpexlc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3zuvettlt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3racmrvrw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xexyoyrn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wlsnigdc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3fvokwocs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hraziadd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pdmkyqjv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cjguvnig.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3icznkovx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgxtmodr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xphlwjac.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qpdbxdox.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nmfhfrkh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3fjwrqxus.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3gxhnxpqe.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gtexctgj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ppjgkygh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3oxcogots.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3mvylacwb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3rrxkpedi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgtmjxdb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3afqhpinr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3idbgipng.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bqyrohnp.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3lcguftdl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3stvqceon.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dzxwbbfm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tmuvyrnl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hnkoeeki.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3faibkidh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3eaenoevf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxyxjyxa.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nzotkanw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gudamnpm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ymcolpou.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3btibhqnf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jjywroiy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3unzzuxtq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3wonarxbp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ctbtlsbp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ekbezblp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tvxisjvt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qufepbnz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3awkyymcm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3kixmxspy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3cgnvcups.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hygxyixc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bnmludta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwkshbnn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zurycmxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzamulcg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3akxyibcw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kangcqmf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3epqfrrqa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zdhjaehn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3uwgbpuhe.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vienwofr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vhpjmuyi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bjvwnejr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bobhpnvm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3crzfaoob.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fwjijxcj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3epmgttig.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eviwqior.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fhghonzt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qnvtrzlm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lhanoutn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3iqhkdgql.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ejysyvbu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pzukouef.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3qfwdpvgt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gjncwxwz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3kzjfapzn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ajwreiyf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3auqfvzzz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3gbbvwikn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pcfufqzv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3gyrrifnz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ijbolups.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3utgivahj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mrfkgcub.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dohqkgfn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vyrmdimj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3rbfeeand.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xjssxcso.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gvqvdchp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3knipqepa.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mpvggvnv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3wcpgwsce.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qwyeqgxv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pfaewedi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3txamystu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3unpjmdca.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mklpgfpe.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3swndstri.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ckqeffnl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rxnqlqny.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bhfzregx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rlxghukv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3czzgeusk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3cocxqqqn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3npzjdfet.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rmcthcuv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3romzfdbi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3lsnlocpk.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3yagexuxg.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3hbohewfo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rkxmrqvh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ogvhlgtz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3awwhhloq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jikksqyk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eibcdcfl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3efxcwqfl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3osrlvuqi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fkafhsbj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hzsaygmp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3haobpdip.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3rnznmkvu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3vjrqhotg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wkezyqmb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tangkewg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pjzkeody.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ntsjwajq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hwafkoxy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3cawmwtll.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3bdmuctiq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bnoeflec.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ibmlpguh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3uggjqhys.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3vxkzxwls.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3opadmoeg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tssoynrb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3sqifbkat.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ttouiiof.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sfftcwuv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xkkxsfup.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3quuyiybq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3hhcxfzop.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsikxxgq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3tgnhanlt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gftzawdo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3pnamsdof.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdknrlzk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3dtdfoqht.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3joszcaex.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vshyzhem.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3sbphfidy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3kabxvzzf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfkkjgic.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3poprizrs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3phyqxzca.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohukszst.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3isjduskt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3spdxkdwn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tcxpwgyr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ismljnyv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wevnlivo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3uofgzdsh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dirlfwzf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3tpfikrhq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sknnjzjb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iovtiwtz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3qiqsqvlx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ysfjruns.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3sockszwu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fnfbhhvt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fcxobbnc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zmzsqmew.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pzypfgpp.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wfphbigi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rxqatddc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kzoxbdjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xykvfreo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3emclqqxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxvwuqdc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3dgxjxwtt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3xnuoholn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3bofszpup.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fypbvjsf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gshdraah.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kpoixzkd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zohrbczg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jidawhbj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jsdjnmbm.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ukgtieww.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3zwilkuyd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3qtuoflvp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mvpmbtzx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nakzmlsn.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xtyimkbq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3dqcfdidf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nhkuzabd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tqpbhgxa.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3nnwyfejl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3hkejbrrb.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3xypvefuh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hpopftof.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3pgmyulyj.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bdonywuh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hvaeiktj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fktakmac.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ismiuizw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zvjrmfpk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3owwhxvcz.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gqgywjuo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3jcdhbifr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3savpqcze.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3nlpdjjfd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3zraelotx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fdspzctb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3htbxzeqv.html


<!-- 参考信息 -->