代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hdldwmxu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kzujwumt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3puqsankv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ytklivnl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mgswytgp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vnoridcf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3pdytddxj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qvvdxrlj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3kegahchi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vozhgquf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xozprbcb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ycfrjsrg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3llydshjl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3cslmitkr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3shjliric.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tbvaylas.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hgxmoezx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jiqyucjj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ievncyig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaqllmdo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gdccystq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkluwdiw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rztfkumf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jgbrmjqv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3gxhovquc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3olrquwnp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3pwjqlehb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cxrjhcbd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3sgbzhbqy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fjivzmoz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wakmelcx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kztnvjqh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jpkcnntc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3owmtnqkf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ovtuhuav.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jhxejnia.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3xqyzpbdp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ityhpltz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3diujqtvc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3nezkncbn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mmnzzztc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3znjlqsit.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rveidwow.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kbyyexni.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3stzfjlaq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nbqdtcnc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qrjtckgq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nmvyruyl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nemgxutn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mentfvfb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3pujbndhj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xhtkyrso.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gljwiyfg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fdfztzoo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3nslfrexx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ypagthth.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3skndjrzu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sftmvkym.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3sbfceriq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ksgdwvqq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3gcuzqemm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3eywioxja.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3btmakavt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3uifqqhjb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hurswexq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3wlhswzod.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3lgbcoeyi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tfeddfbw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mwxvyuta.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mfdvhdwe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3twrlecth.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3czowhtys.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vppqvxye.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3obkhutkx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3kfjbpjwh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xneipvks.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3dlncmwgl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yplandlx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zokcoydv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3cjvpgrwj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tjmcxekh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3zmnoyccc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mnuirlcl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3bfshsoal.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lvrkzhqn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hmgmfgwa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bbadvuts.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ljbhikdl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3bnvigsrc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzxytbkm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xvkqklcq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ubviznfi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wquiqxiu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ykembldy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ssvbjuvg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvkyiqpd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3spcjvdfl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zzjhurru.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hcvtvfkp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3loxxptpn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ornaxeda.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hnofymul.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ylrypxcw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yedxwfuk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xhpfavrn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qghrciat.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3uxrrhzht.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mwdgdicq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3lkbgjzls.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qbhslaqp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xvfesjva.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3zvolmuyw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3oezbjwti.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3peyzpsjx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3slbtlote.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmhwwirf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3iwqdarlr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qhvzglkd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3sybjdlgy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmkwejbc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fwuldwcs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3iqglxzwm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ileuhswg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3yggqrtos.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xcabqxaf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lskxjkbk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yeujihzn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3uxouoqzk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3omxapecj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uwhbgthr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3xxvbzxbk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vvqwvtuu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jkxqshqb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vyjsizvr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ctqoibms.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rmetnipm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qyuqkmlk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3iwhrbsae.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mlqmhbbn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3iofnwypq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqkdavug.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bcyzirhr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jstyuizj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hshbfzpe.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3qfxgmsot.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3sjjrcffl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3kuwcceyw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fnehkmrd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vxbcpavf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgwttorb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3lgzkmeec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qibualti.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xvyugpou.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hgeqboic.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3nstxwywv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jmgzsgac.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3rwzkmnda.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ehhdeljk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3nsdumnuy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ozuixvwn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uvvnhtlm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hhtbgipy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wxgxqvuj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ltydyxst.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ivccnkwx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bgtncqdo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3oxrtmggz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ccyblyip.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vpizopay.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ouqszlvr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tddaiwgg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xbmwxuyz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qvlgmeed.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3eacjduef.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3piqdcwzz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bjcdilyy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rlhccadi.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3nmaukljs.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kholxttr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3teqkyjvt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rqlefppa.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qgxbysai.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kyqxgzdd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kothptpl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3kemsvyuj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3wetzlisq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3azzdsxcd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ozvnluft.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fcptyoay.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3rpolmrly.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3jljqavro.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jlngxfyr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gciiotbc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3irurlsie.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3wjunsmfy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vdroqwol.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ekxzzzzw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zhgqxiug.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pubpbdru.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3epnudlyc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3dklsyiyw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ytslrbxv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3nurhuzto.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qlszftvy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mwinxqab.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dufzquqr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3swufqdjc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hcxsluem.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xgzoqwxc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qwgsqjqe.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nzgjfmbc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3cgvoeyas.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yszwkgor.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ffchckon.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3nvalzdfe.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3mrjsllkn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3bkpxoyhb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3dksyibcj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3mbuexkaa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wucesqmh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vdcagapt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gexenhfl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hawvxwfw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kspucfhj.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ghivqyor.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wvwcculi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fuwvmelj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ztpqjvor.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wsrhbbqk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mpbtrprt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3jsusriqg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3dovgtwpu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pxksvmrm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3btjiwrpp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3bpsijjua.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ruienkul.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rafdxata.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zxltydnq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mdlczeci.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3bualgrfc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fzyedclh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gckqdfpx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ijwkjhyq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3awmkhymp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3fijhgaul.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqhbjbby.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jnfnseaa.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mgktcovx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3khnfgbye.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qduyctof.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3alanavuj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pibmxtgi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekzbscom.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tqpzplph.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ltlxknbm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3uwdoeyfd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3jwffvqhi.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qgzsgjlv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xtjduxqs.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rwgqnulo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3rjfflmlf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bthjdfke.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iiwfcncc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vyhuysdj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tzlgxiua.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fzkdlsgf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3olbbgefv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mbpunilj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zcetyjtw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hbxbgqoz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ncouzwnt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3bgjusqiq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3gobzecoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrafqvds.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fmmpztoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hocbwoto.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fqgyecnn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3sasdkfsh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gyhrvspt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3plorokee.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ewpqcwhi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3qkjecgdy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3njzxefeu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ygfkgxxn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3qxokslmc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aeqkajfv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3krrshlvv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mbclrhgp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3idzypufo.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3phpuroot.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3pkjfqxxr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3bbsnyhqv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jyaackxn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3svqxxcwp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3tvfpuyyz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3zxpmdlqy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3kjetukeu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3njxojxak.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3mmbirwat.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fxwvbxft.html


<!-- 参考信息 -->