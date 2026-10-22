代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2auvimewn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2npmqnutr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gvwkxtmk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2trfcjzfy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qzcoyfrb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2mkbkhqmt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vkkhompr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zyhksiee.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2oseplsms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsmfqvkl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2scvvhpez.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2kjrowzmz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2eynfhqbj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xspxvfuc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2enhtrzpv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xailyrox.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2tgmdmzcq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2kidtxrne.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2diiavdpm.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jccplysc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2axwhfjqv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2icfxegvc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xunsfuks.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mnwimyxh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zuufgpnt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yjcekaze.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2otjpjrnh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2kycbmshj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2vdyinrif.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2fajbdrsn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xtrdddys.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vsevhewq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gshpmytd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2clhqlxcu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tezejjse.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kiokcgij.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ixvmuylb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2maggvzae.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nljnlrwl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2hjftsyxf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fqpvmqiy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2shwgqxqf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2tdghfjsn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2basnatqv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2oxstrgii.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jxsclgzz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ckpexzcg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ecssfynr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tzizzivf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jyuussjl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mhkayhrs.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2aejdllji.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gqxskhhe.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2gxcgjhyj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hozrxjrl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2aiafozrl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bdtpfgym.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vmksixik.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vfzfaqkb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2imppftge.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ppnaobqy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2sjoitmjw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nkgzkaej.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kdmgdwsh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hgpcvjpr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ifyeavmp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ytuliudw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qihsjevq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2yfwxhnwj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2iyoofgxn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zcvatiwh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rmsacdji.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ydfqsnbp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ozriprne.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hhiybcha.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2goqkoqsn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2usdxsxoa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drwzvmmh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2afdxjlfa.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ycnnbwqp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jdakteyw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dckbdums.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2njahojtu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2edrbjzug.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2fgkfxidz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jsywprjm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xtgnctoq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qoexdtwf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2iolijnmo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cqlfihez.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fkkgzpic.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cdiaxmeg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2yckrlosw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ocbpuxje.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gjswouek.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2jmfrbjyq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2maxuhahq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2znfvdylz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2cjddplid.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2haouahyc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2mxkzlvny.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qmmhekuz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xoccvclq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jaqrwdbs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hfypgnvh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rjzyanzr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xitygzlp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2oqmndlbg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2bpswuuvh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2skophxep.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kqwxaqth.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hgedujbz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yfqfwirk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2vsduivxd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2glpyykux.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ftgpxjjb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eyuwmgts.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bpijspje.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ideksyua.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2poeahtyy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2akloecmz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2cfmfeogt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2pxcqwasa.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2wgakfqxu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vykvowih.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hobwgxmv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2gxpdrgdz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2yxroexrn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2axnclckq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hfasedrd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2enqkbwpx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2tmktrghi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2korvbhzu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2vbmsglwv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2eseeyqns.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2lfxuyefv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2acxggcpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frtsshmk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ounpptrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clwbrkot.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wjykdqqb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2alapklgj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2yeohfylw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2zmlueakc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zwmlbpwv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nzeflzkp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hlrlstku.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ydxrklbw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cxzoiywc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uvnelzep.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wplqcagj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cxbzuevs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bqzzdtds.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xepxyutk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nzfyqnna.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dlbbjqup.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2moblcrxp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2limuprsc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wwougajp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hoagixlb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2smecmvhb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cvldhpqu.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cjguqhhz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gatwryfq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2uqtasxyd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2efjchfmk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2yajusqha.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ankjlmwk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hitlzoup.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pclzqigi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mwbrcumn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zudflswn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xdmsofnc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2phiscboy.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dteepdwv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2dpniwuqd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ptjilbjh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2tyehptao.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2essphind.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vsejipbo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xjhpokhj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2uuvekvoc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2xatvqvub.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dfbhmkkg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2tcvhxugh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2walodwqk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2snhsrewj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lckewwhx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vvjmdteb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2zcmjtvdl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2mydfivtw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2cmwqsfoc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jttnhegz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2zbrmzeyq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2setdqnmr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2tlbukvij.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ynqsplan.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2aprrwraz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yvggvomw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2rkuxatee.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uodwdhdk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mcivgaux.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ttxbpifi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ugucnful.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hleeyqzw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2rlimiroj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2averqwzb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ewcroege.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2kawjzllj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mnwahzzw.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2riuapmlz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wbieykbv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qbisqjzo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2qnisvslg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2xqggfhzn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dcjgrueu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hqgvdpoa.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2kqtzcixv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2lzvxiixg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wcxmsrwm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zqipwshn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pdsyxjsd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2spuzojdi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dwqfduir.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2scjztwxb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2aykvfwtl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2vojdjxbr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2veaqfisg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2gydgkllf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mahnzhdl.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mesdvlic.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zisuhodi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cesdzczz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ulkzsdvh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zinswvum.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2csdixmvu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hdiququu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uwdjujzy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikcbhcmu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2dkpmerqw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2itmlqzss.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2skzehqvk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2coayaamn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2bqbplhpt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wuwqneaq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cjcxdijj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2thimqild.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xrkgxlmg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ivululbo.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xakoigfq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nrgwddia.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nejphcvr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bizlxsnt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nednfzgl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ifwweqxy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2giwzgdnp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sfltiish.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2yahwogyx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2puzzgtah.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2nrnmejdz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2bcerxeci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qivmmhdu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lszgrmny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yylvbvma.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ufrdinwc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nhrmchso.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2lcridika.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2eyvmbior.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mwoquqxi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2khucmibl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2cprkhnbn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wtvwxenw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2jbnvjfro.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yryngwtj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ssrvflpa.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zqstfoxt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2owhnxjit.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2yasiupop.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2aezyntkf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2uqbaxppd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mpeutjtw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2mgdnmytv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2gvdblpub.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2gcvosgdy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ipgcsfsd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2rctookdq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2oasbdftv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tgfqnejm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2hpjwwmed.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2dgrrnesm.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2islaoemp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eivjrjal.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2kicrotty.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2zjdplcob.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2mpoydexf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2wxmfivns.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gkepxpwq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ojeaqfit.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2mwtrpgfz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2iolacosk.html


<!-- 参考信息 -->