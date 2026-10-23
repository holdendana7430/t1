代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jhhkizlv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3vkrystbt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xmofkbup.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ymwxtces.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xbqjhvro.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3obwkvvzo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ojegnqdh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3kurzrjyt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ipstnbnj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vqsjvavk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3zwmugfry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezxcgbvi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kpgutvla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndmtpzhw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gommmijq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3nmhtynku.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tzylisll.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3veadsqyf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3igtpkpaf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dyjcxsvo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wpxtbjxp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3hztzveoo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fyjvhqyn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3viennset.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jeahuntr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wykqadjg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3yraphkqg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ybfbjpum.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vowsmtwk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mbcdllom.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3boufqund.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xpwkwvgh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gvngkvyw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3khurmeos.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3djnqhkeh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qjtjfchv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qalfgcpb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cjhlfohy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zwwovpgp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixncrivp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cseidzvf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ybohgwcq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3uohhsxmb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nqmcjfbm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3kyscyfgu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3kjtvkwgb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3lnxhwpdf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fuatmobx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cptrippy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wqdkzads.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vhyhtnap.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3btvrtcyl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tfrjrrnv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jkrqlooo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tqctdbtd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3xbwojbto.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jzkjzygi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jakpcktj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3fiytulfk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tdkkqwyc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ywejzvfg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mcsiqwse.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3xuznewum.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3jgagwmhx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3kowmcrdp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cqieuebu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3yjmccxpo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3sqludvyu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3bsdtmalx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3pyubxfoo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yposlien.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3gwdzubuz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3btdrnomy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgfllejf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3wdtkyvqi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3phybpgcu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bwasrawt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hcpeewoq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jfpipzhy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qajiaxzg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3veevyelz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qayuipfv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zpntzrxm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ahzmcktv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3osxxlmka.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rrcifdwh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yzlwbrll.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbstdngg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3yzodnifn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aqftcgvz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ewwaacuz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hlqqnrda.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wmzmfjqa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3egxcjbgq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3orimjsnn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3anwqrodq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3qdiigplz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3iiixlkmk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wryluyvv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rsnxzmyi.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3najtnevj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wetaliec.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3hojryiay.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lihdkvij.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qqbmusro.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fwmkobsa.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3qjonfyoa.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3sbdkbdap.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3foobxaxc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3knndqbch.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3yptgbyjv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3smeyttfx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3pypfnexd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ciqolsnz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3blqdtkwu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wprmdrln.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3umiwmwbl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3lopdodnv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zxnlboqk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3rqmxvfrn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bzkwkppi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3thiihdfe.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ikfvepde.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vbpdqdds.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hllzrckn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3nubmunhh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3gtmsyqci.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3glfqonty.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3feuuagbb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ropsdfwj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3nxfjsqqh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3fxxxdhat.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixrlmlzq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hwggwnbm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3humihenj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qtrhuhaz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ujjchyxs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mzsfgepk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ksfyerzo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qqwhfdyb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3obeuauzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osqkchgx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gyznoxsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdwxtslv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xqyqmdtw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tbysfcif.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3yoqcetbj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3toutoigf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3etotgqjl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kbvobtlh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qdnaacbw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vqvynkxl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3reiahejk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yijyotje.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3iifkcdsu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3abfqayud.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3swmiyuqs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hdqlslmb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3qbvyvrfu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qljxruyp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3wofxlocx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3daspzoys.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hpvexbek.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3lcwpcotr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3osmbqmle.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ohzrkuuj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cemhlmwb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xcamuaru.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3wnkaluja.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdzvydej.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fkdmjzqr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bvvucsen.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bgudcuux.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dskyyoqp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mlycgsfd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lffdnyee.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zbrmkkmu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3sbvitqsb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jglulwjj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3prgictur.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3omhvfenw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpkzxtvx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wztfaekv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3rtafcxyf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3efncanau.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3qivpoeov.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3amgidgjq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3twasntpg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3sssfqrbj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3onnizmyu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yowwgtjk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cnujfsig.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3hhcnmiae.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jkiveohk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ubzduiwx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ozvmadyt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3amxlsuts.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dmincqdi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3eqpkzknf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3wnfkquii.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hgcnjbbh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3syoambar.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vghnwbka.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3qdbrqqip.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qvkiwnri.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rajbxhxz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3hrwaszbi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ukwjagdt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jaxectcx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xdpittas.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hsnneisg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3enyijaqb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xamakqdk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bberqdvv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3sctaowzk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qcrckqgq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mlbeulde.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3pfsnjowy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jspluthb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rgfupenm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dtvhwbzz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gkcifuml.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3coqxlmgj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3uswenrrw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vyukjmie.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nhqmeanu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3oazcwrbf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3dlipefrd.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3haluwqxi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3eyjosiyn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3elrclnbf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jbodwiru.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3cooqkmfa.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3wbzqefpp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qvaaxesp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3zmrtecdl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3lpiikonf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcnfwbfa.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tcoycwun.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ektywuwa.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3opbtpepb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fhadybnt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xkjzuzhl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3amzyanzr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3iomkmjpf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oupikyzz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ylugqldd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ddbptpdz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3enbgtsgy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pcviogxb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vgmaiinj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rcmopadp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqnaxakj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sqksneac.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bawmoayn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gxtnbakl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lxcofbhg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3clihtcud.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bdilhrmh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kuqtfzxm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qftcbnta.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dtyhuhxa.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3utfeobfj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qtxblfvg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kzdmkuhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhgfdtlz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bqttllfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbfltquu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xpghpjqx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3qhrdiniv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jxykhwrr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wnswigak.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jxbsuhbv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wubpdoux.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hvduheft.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ksuomvys.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3xjmsnptn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oqzgfbnv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3mtewlphi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3upomojcz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lalgbjcp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fnocljex.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dpbpjmeb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ntizwfzt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kkihowta.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xojyjoba.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fluzalrz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3zxanqika.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3npwnkvrs.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3amwbxqpk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3rjjesopm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nnubbtmd.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wdsadgbb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3fmtxlyde.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3shxgdqnk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3lksoqowb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rlirnkok.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3msxokfvk.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3arqefzpg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nzpqtiim.html


<!-- 参考信息 -->