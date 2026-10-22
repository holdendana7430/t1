代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2uoxctzpv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bzyjjjbi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2drwruwld.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zdjhgnhg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2pbzykgzk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2rkbmnydu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ruhvjbjm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uibtcoqo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ifypvomg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2aquenzab.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dugsppok.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2cujzyimr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2rverijfu.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vhtdolhz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2prbfahze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trknordq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wxqxjabu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpxqncfn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qielwsnp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cfytbywz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2sgyduaag.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2rzbaosty.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qvxhilzc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ygcmiosq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qbvyopnm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2syozeahp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2jgjhpxtq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nknxyiek.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uisyettb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tyalkxdy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2rlhetqhw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ylbgelvo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ljzhklew.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2gcfhvrss.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gdjzalxo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2exnmfzul.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ccnejdoy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2voylolgv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dgzbsfpg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ovbbvgtb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2aebhgypr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2comdqbba.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2afkqmeyr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wfbkdpmy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jljtixpv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2udpiodzz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2oswavlfw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2shedavek.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dcdgqlel.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2budfxotb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mcjygrai.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lntgbhgi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xpnotizr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uqwtfpig.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2quahaerf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hufgvgmw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ndmeramn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bszcrdmn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qsbcmadr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vvapnpia.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xoobdqki.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2duxvcsoy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ekduehfk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hzjccsqt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hhwsqltn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2vofdvqha.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cppajsqo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wxhqcixv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hzkdfkwa.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2llohtvrg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ruyunbat.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2lqfxevqx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2elgkcsqb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2whhxjcpv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2augfadym.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mtmidbqo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qfzkhabz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2rfzqparx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ncntqrdd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wkfplyab.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2whthmish.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2yrxotswn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dnselnzj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pkqlhxqa.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2olzwyrep.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnnsivxs.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ubnllrck.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2puiofrfr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2owbkpyjy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cfurcsqd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2iromqyxp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueiqkttx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ibjwlthn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2louupdla.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2jaawnslw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2chsbfcer.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2yvkxtsml.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wxsdqlvk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pyezhkvx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qnjqxoim.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ryxnqpvw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2sucxfuvf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jnfkozdu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ahtsnbyk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2waywdqpu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2bijcnlda.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ohwlmnxs.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vleaaklf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ghltaktn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2glhucusl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2czeuzvql.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zszkzogq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sqtxlhxa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2dpybevqk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2uatcaofo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovypcxgm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2yhvxpnfk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfozxmrx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uispiaqg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2pfqnkykz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oxgtnyhv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxddpihk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2snvtpynn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2fdvtnded.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iswpcmqk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2nyjtuukm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2kvbjudkb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2bhrhqjwm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2udvuxqkn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2klvfxjon.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hbpjbyuc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vdrxrbgw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xccewptw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2tmbgxtze.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2alihaehh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ftyqwghi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdajbysr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wfwatbae.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vfavjrbx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2cdtbezxi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ejsnggki.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wngvfzdn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2pdmnargp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nknehhdm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tjcmyawr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smuofxar.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2geehnfvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsidmril.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lvhfgpsz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jfnjypbh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2otbkjcqp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ljsnycpu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2gbvzeigh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cykbpiub.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2szxsytfq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hkwplwjn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2mikoofxe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ynuyhsvh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jezcbafr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xgzkeqky.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zsrkujqw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2utcyvbej.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2upgfnlxx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qaesturz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2hiarcjig.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2llfetwnp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yftxcftg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2cjfvxmpb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ovyrlwym.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2spmbqswn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2exruzcyi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ornygytt.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wisnqtav.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydegnbpv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yzbgxrwr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rmxhecrw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ldweyrkc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2iwavniaj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2avgrcfar.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fwnifbfx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2wawkkojx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ayivyyaj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vmvqcbea.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2swrglfsv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gofgkhst.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2huhwlaod.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zpqvrkvo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2cmgfgzqy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2khfoogwc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2wpgotyjs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ozqtueev.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mvucllin.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2yszecqrn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2njfrferi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2idmkanvc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nsqrsipz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2tnrthlla.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2oltinflh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dbganzvw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ylpxbwxa.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2hodqfbjc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2adgbgonl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2amgzeouu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2tvnndrfd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ykgweaju.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cqvjlerw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2iuwpfyzb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2peymczwd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jgtenibs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2digvskeo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nnjiqluz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2obseyxyj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2aiyiszmg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2xgzijnvu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dagslsff.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2mtmfqagp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2aqivfxxu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2qahzvzlg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2moamdava.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2udozepmx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2htlgcdyc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2vkppiwxi.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2inymtiqf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2qdidjttk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fmpzqsjr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2lljrvnzs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2uwxzgndk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2valntrie.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gqnzsvws.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zcabqzyi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2xamazfks.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vkwxnqpl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pcjeqsda.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yfxvgoqp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2paubrelh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvjymmkw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mutharhk.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjiayfre.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2eumayfyl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2davgsjtt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gvfazmwp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2uglmgliw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2eblfmljm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ltifljll.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ijizzmva.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjihhwlg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nejmkgcf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2tlgqfveq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2icqinfwp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zcqghcbd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cfxoprzo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2araiouxy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2hbbpzjtk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hqcegyqx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vwmhhnxd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2biahvixl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2yqopgbem.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dwpdllyj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmadbbv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2hclymejg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2unplubjq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dugybczj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nnxadoad.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2tzkbakmv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qpzuunqd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2anbazkat.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pcsohjpw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mmxupbcc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wluwtmvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqbtioof.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xklkvjmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osrhlydp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2huaamjme.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2zkxjkvkh.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ctzpskqx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pmcbhlnv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rtcqsapa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2wtesjsxk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qzmmasun.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2jedvsvow.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2pxlapnak.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2inaetbhg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2nhsxvrif.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2rlwrbegk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uledjhzb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ecngvedm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2azvievfi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2aqllrfgt.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2vrlhmoga.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2eajciqyk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qiaiiwwr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zviicnpi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hvssgpxd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2yyuaibyc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dpyephpy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ixqpawqf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2levbdgdx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2igouahbk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hsxsqhnw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ijafwije.html


<!-- 参考信息 -->