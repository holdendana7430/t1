代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jakjgbvk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qowgcgjh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3rljsvuts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sabcvhre.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3toiylluj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnjjqrcm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sugoynqg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3onfyopuk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvubktfe.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ghjvsvuk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3apiwrfqu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vikcgsjg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fqskltpm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3lxlzuety.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bybxrxba.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kbinnmpi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jzuwvmoq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zejznthc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3dsmibebu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3plfscaro.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3esebpkmd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3agwnxjko.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3sanxwsvt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qmibqohw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ykwukjkl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rwzzkxyc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mwkrusmk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vcbouzvk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3cudwbzqo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jfakujth.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ghccnwbz.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3eofbterr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wzdckuxq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ghtfyouu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qjqkowkt.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jjjlxudt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3oyzqlmow.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cymhiauq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3tiumekwp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qfbahxhx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yagddngd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cdtrwhbt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3asdtrvsp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hrrkvdgt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3wgtalats.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bjmoodrl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uykscyks.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3swuyrwhf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yrohoviu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3udjmgvqz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3yutjmxkx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ojltzmrz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3hykxlduz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3sfczxmcy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qwvlfdky.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zymgkxcr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3yvhxbhuz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rbwudcwm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3howkimgz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ivvgshvy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3oitnuccq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3uckvlgla.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fsagczie.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3dweabwsl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qerqcdko.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3yuddadta.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jzpqkcgq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ytotjyrv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fygtqbes.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3krxegjor.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3pujhmlze.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fxhhmfkm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mhmfwrmg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zmlobmwc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dtkklnve.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rkrvlzlx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ngurmzia.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bdpfvlaw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tyjskykb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3zyakemfr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ciommgtk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3krowbess.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3goebpnfd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3obezkpoa.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3bdfmedyp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ckbvyxhg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ktsxjbfi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zkqkqtnz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3brsqypgn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3uwtmuvuv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3mfitwqwi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ikgfeusi.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3erdndquq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mlcuihey.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3uqwvlutg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cmzhnmqi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qzdtijmh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3kczftgqv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3canzrptn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xumxneao.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qvafcqya.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jjcnlpec.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3wrcwpyku.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zokgsmfr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3frbczjkt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3imlxdngp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lhvualgr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dqqyjmol.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3yryrcksn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3iweatvyi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tbxpvwtd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ipuegfuf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fahubmsi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hcrrdbzf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3suggsgwz.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mrhnbntt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3wknuetxa.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xxmezxvj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3fknlpyyb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3mbzekoee.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3atccgyar.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3alkfcddu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ekhgegot.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3aoqtyhut.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lewmaxmw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jvdttref.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3amawrrkx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ybocmnjl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3yabkuior.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3cgwmmwxi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3oaskulai.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3npjurvnx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oyelfqoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uawhxnch.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3rjfgnqlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndpjarqp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3umxiwwlm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qkeiruvn.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bqsfcnio.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hpjammzv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ooaoqejl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vzsplwwv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3duoawzfa.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3solbdata.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ogjbtlcx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zkyfllvl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3obgrdhri.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vavlngif.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tamoynho.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3zwaehsfc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ziekyrnw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmlwluu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbqhmywy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nmfflnln.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nldnwywf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3asgyuktd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ctlywsif.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3iezfjffc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3nnzpigbj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ignaocga.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3tpfumotd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3pnsgjtmq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3stczxgow.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rgezfvop.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fouhbozv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3onpjqudk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rczqnfqe.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3howjyetc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ctzgjavy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qnicjmdg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nvcjuyim.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ekxmeslz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uaznymfc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3clkzjdfb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3joczjeos.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rgxyvjzn.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mcgbldcg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3whcgygur.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3lydzailo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xwimicbi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3tckodstt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qdjxruip.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gowglajp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vudwvkgc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3tmbtbxye.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3gtcngokt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mkaheuae.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wzmvwjot.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gfokfugy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3awkzsuie.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fpznqsuf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3nqynigbk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3omzjodzf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3yvdrexlk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zqxmclzl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3igxmkegw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uyywucwh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mhsbsyaz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3cuzujowb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hgnipbjc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ltlnrbqt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3pklnjznt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ybnkjqny.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3djxfcsme.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3oycpimhi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zhnlqxoc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3gyfuvunl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zekzyloj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bqmdnppd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3azebkhit.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nupcgeri.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3gzscytvs.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3grkzrzlx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qykqtxfo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3thatfnvo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3stpemsnf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ijrckaoy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zpkohtmo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3kmcttibg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3uomagrxl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3phijfcdc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3drkbihde.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tcjyvqvv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3heixulsm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fpydvouk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3txemhayi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ebuszwrq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3uoudhxvp.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xrzwhhlo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbzjltmq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tjolikog.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lhoeiuxd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pufbtbir.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdbqpfrj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzoeayys.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rdtiiqnq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uksfotkt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fndkdmee.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zujrzwfj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3iupxudnn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vhmalrob.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3smpdvlpl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lhuajhvb.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3unnpohjr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3athhxezt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hdjiohme.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ulvnwzie.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3iuflzmrd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3khnsjecd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bdsnbprp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lkcmdmbm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3nbwjrvoz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3usuxoobt.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dlgwkbpf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3skzypgmx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3sczqcfvg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gdcnqdzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdrfpipe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ajgtfgry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jolwcsqp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3whmaupcy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ntsvmcol.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3teqzyvso.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tisdcbnv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jknpyqjj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ltnuclcf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hzqeitfo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mueseqpv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3tzxpkczl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tvnxiyqr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3lzhjmrni.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jeitfkvp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3yjfamozg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bapklkhd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qyldzfrs.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3blruwqce.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zzstbgtm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3qqurxhyg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qelkkjcb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lfpmiotd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vijmddqc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wlwqsaqe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3enjromeh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gyopxnyx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3vahhvzvk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ikqzdhnl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3sjxgyjfp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vmsybobi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ckzlcijl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3rkoqfqlt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3guqmmkil.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3msyuxzcr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3keyhvdzh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vfhiqrzg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3uzuhbffu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ugvniafz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3uprveyda.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3tqnfpbyr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3xfagjiwu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3zzjcxcbr.html


<!-- 参考信息 -->