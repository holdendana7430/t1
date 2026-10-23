代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3iwpjgnat.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3thbxqoth.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ukfzepim.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3lmawmxze.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3zlzpvand.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3bvahnldq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kaqfmeye.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lujflvdx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rqodyprx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vhssszbd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3znmmwrre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eagvnyql.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wzmgpzka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frsvuurf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mzwzmeii.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3drvygfgk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcjkjoge.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3oezpuebj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3mgcapwhs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3makarkmg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lmixcebt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3udrquiql.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fvvjpowy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xgjhhejk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ouwnvils.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jmtzfdhg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kazrggcq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jfzhhhmu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ugoilmrs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3egoasyfe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3elkeejwr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3tgsflykd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qhavvqbf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cdwdlmls.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3vknvywpd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aogkltdp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3kbrfiaok.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3msbuzmjv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qlpsxbnu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3unwhkwsi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3whtbndmb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3nqniawre.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3kggjokjb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3agnocmxe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ybuvuryu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pigzmedr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3yizrxfox.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3iuljpfff.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cvmkvflc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ehltcsbk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xcgzkijx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dbmfuubr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3boebmoik.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3uerjlzgk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3odzknhkr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3oltavxuv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dxuyfilf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lgefbfmm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3swhnqsdd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bvazcemk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mzgtqshe.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qhahdomr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3myqpfbpi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3oqjntgmu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3aefadkrg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dtaqfizx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pdlhaayu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tfelgzzj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3nencygyo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ohctpihd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xwfnqlty.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vyglgfyc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cwxatbuz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3rpswsagm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hdipkolt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tuqkbfuw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ktiawlbp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hbznoqyg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yrbggsbm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lcakoqdp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3aglsmcln.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fwvdqqvc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3yqzacuwb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ftinmxii.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3cokjdcji.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bgfvnzbw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ovgepplf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3yuznrwpq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ngeesrcc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kmnpimde.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qpzyzbja.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3grmxjqpv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3xwdykywt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3szguvbqt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jjsvepiu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zppeghut.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ezkzdiwe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mzmvtwdi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3zmfkgvuy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3brlhmure.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3niugzwgx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3izcuavrc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3psoafrcz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3liokrjzn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3pnozcgqg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bwalgewy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3qsebtxru.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ktxpohvw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mhqzawsr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rcjdgwbd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3neknbyhy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovxtgmny.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lflfesgm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3omkbbghi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yddwyjzh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bdabdvoh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rqinujqv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjxauocp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mlcoilrs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3biojpnli.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3efewfubm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fuenoqbu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3qvtwhkbe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qqgmqpjg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwvjxyqv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3courlcxu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xbpggxgy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ypzwjdyg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sfyemxzf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qxxmawcc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3lahilovg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3yjhdeair.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ibdnabgq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3canepqmi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wfzioipn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wxaqurnn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uofpzvmx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3thtonrpa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tpugvnbo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3dkdyhpkv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cuhwluyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upcwuboi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ulqbjwwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssexssda.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xcyqlaiw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3whjaatpc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ecafdnix.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3lgjsbala.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ivdxyiqx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pxpnmnpr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ryhslipt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rczsxxsh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ommpmyjp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3wasancab.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3onvwtiqj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ftpahlgd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rfnjofcq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3uykrqjxm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3aqeylvde.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fcaqqckh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3tgqznari.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3taezolpr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rrrjlhgg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3sibrwaky.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3kntnxykb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dcwfnjop.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3puagdhcl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3udkpwhcc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3usxqwukz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqiwgvdd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xszvrvba.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhcrywq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3srelweww.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3swgillpp.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xlvorrhs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wgucoyoc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ixbfrgdr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3aelleiij.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rpautprq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3hpcgeqhq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3utypwosc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3eehmuico.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3gigevtig.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pgtaoaun.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bozrengp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ljdmtery.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3wsjspijg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jmqrmmwi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jehwxvsh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bqkghpna.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3yohckaps.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ulzyvidq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wrffmlgj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3btsrfbdo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3sqxacvgv.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3txuxczgo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3mskyevzu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3frhgwozj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3psxkjdpv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3lhwhpoop.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gkpwrmya.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xkkcgglg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3gkqovvwf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3vplwvosp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tfjkmuty.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3awhbaklv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3htyogjog.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ewlkagcn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3srqswtlp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wxnnguun.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xcwhcejm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3piqwrtuk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dcskmndh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zckdfuce.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwhuegww.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mugjwfog.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fmbgiyzr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3avepqncf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3eyegszdx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3aligugpy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3chmxbsri.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fkbvmndx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3crvsnlya.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ejhhlxgh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ejgzsvqr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3fdfvneux.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mvnshktp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uhuzciim.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jqdvusby.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3emcddglz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3pzmuuttj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3avrcmdue.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3imubbcjo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bscboctp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3eusnpjjt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gdbatizf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bmtwdfjc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3afdluotg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3yigwjhot.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3txmqpcel.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lhzfuyyu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eayqeauu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wpyiyurl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ejgjvqwh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcwelfuq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kbbasmkc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kpbhyarz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3qmlxxtvw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dnyhfbtb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jtevmbsi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xfsdgclf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kgyqgjei.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qiuudsdb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3snvwyato.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3urvkimta.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ilgkzlkn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uexyxhju.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vwzrfckw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yotgkixn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3kapakflx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3uuutvcyp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3orwxersc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wgtdpuug.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3lqtilirc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3uxmgrhgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehqnmkfx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ghjcflbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqtpusby.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kpjpmolc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gysbkluy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3koeguhot.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ekgciows.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3arfdevvy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hmdzesty.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3idzzgeov.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3sjxznryw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3hfqmptxw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qrmihpwt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ngbndxta.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3fkxxymvy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3shqyxggb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3tuelvruu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3eqwqljsr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rjoowiwh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3illbghjh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3glhdrrfj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3efyhdifs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3oluamwop.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bfiigkuv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqkfrrny.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3khmnptyx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3upnylvqe.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3iezradop.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3drwzjchy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3aobuprpw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mgjxhdcw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rdmqbtjr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ukgpjmxf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3negbgyxt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ckfbyhss.html


<!-- 参考信息 -->