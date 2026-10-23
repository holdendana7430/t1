代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pmgrrwdn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bqdqdoss.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3gfdyrzvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rytnrwcv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qwmwxwac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mteimlfu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rhgnfmhj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3tdgczajj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jigwvzcw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mwgywdae.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jvznljvf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ojmujqyl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3mwpgixls.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3oqjedvsk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jqbhvahe.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pugosepx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nujoknrd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zdwvbosd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3imgoswwj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dlncliad.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3sqkxkmua.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3mxvdhhcg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3vhegzpny.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3tsnfgynl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3bmlkfkei.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3loaapgkq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ffbmeraf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3adnhangn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yhvuywqr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ffynvakh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3trjuxizk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hcenbrlz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nijqnvgn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3pfvycfij.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rvfjahdp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3cicnglfc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hhfgjrsd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3dlntbyfe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3rvflqija.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cellzzgx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kuatpzpo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3aaazkrfa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3oljtnwae.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3acfssnzc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3fkjvrswg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kylvgtlm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mygxuaxg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ayleuxfa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3veakpznv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gqipmmpi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3qvkmzqqr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dvgveufs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3xivtxejr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3meidgtra.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3xnremcir.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3epajsnlu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ohxyiecm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gicrohby.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3exscrdbk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3bxlpaqmb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ubcwzynq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ywvxantr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qkrxhuue.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rseiwvlr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jwmymmow.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ekprarur.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3htjgqmou.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3xllptrog.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zbolytbq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zgztvxfd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zhphpjln.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ywtytxow.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3sbehbpaw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qekiiukj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3kqzlnpbg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3apkqllhc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3putyxupw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uaatsfnf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3trkscqvf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ajftvmwg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3eyzbioms.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xmlhnfvg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rgjpmrjn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ksmznyvb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3cnajajcg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vvryvjhm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jztjcbkd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mrdzsmoa.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rgduzllm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vrpczajr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3flpbosvh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bwruheod.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3egafshtp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ivswjciz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bqdusjpf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kmmpdbic.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3valdngva.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iimmanel.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3oimtlryh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhmhrebi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hyknbcqa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jorvwmnl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3akeiljft.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zmscevel.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3atpzlhrw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3myflsbca.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kvtitlfc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3dtrfkvqf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ktzfwrpr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vnmrjgvl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3bnmtwfly.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3xcpkrjfa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ckvfaerz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3vvgxqysp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rfhhtwxl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wupwxknx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qreqihqf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3pffrbzjf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vrzxtgzr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ztrnzgth.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fsqzfmxv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3psoyottr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3tgjwpprh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hzekipou.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3wlgtywor.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3yuqxlajb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3cxkernua.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3gqcfxfxj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3uiiiwiwz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3kiojzdmc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3exqitftk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3cwjqloaj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dtqibuuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqtdmudn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pregawbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwocebnk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fbjbcdxp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hvvspdxf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pkcxewfy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3aykzcyyx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3gqtjwslt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kccrlazs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fvcatdch.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lvqiyrbv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wlzctpqu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nfxdmmdh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3amevgoyv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jkakktnc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tzsfarpq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3evqchvyy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zbfywsjp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3btblobbw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3lzgsvaup.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ueuweney.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ugxnapdw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3suuamczo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uxidjwai.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3pjumdgeu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zqwwxfto.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mjhduqqr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qdpcjqpg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3uwksgufr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3uxitfiwh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cmisgojt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dojpjfjb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lidxtweq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xczbjbhy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ajjcvgem.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hogzfycl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qqbsyasa.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vwyqtofu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3yqmqmzju.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tfxspsmu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mgdsotae.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3opdnrbfk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3guwnljke.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qpccpkyd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3hdwwyfnf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jjccekaq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pkylzxlg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ttxyndzh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rvzespbw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3icuspwsf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cwttjjbk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3begiadnc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3cqrsjbcm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rcrqoeis.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3kdpdkxqx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3adjytjmg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3gzhuetdq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cvghdqtx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ysyonxef.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3qdszdkpk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bxmsuvhg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3huutwkxb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bmiadxfg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rigjxywb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hsjarsyn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3fxjzjpuc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ttedwebn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3sjsplveu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3lijfdfoj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dgmhqftj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mecemqzu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wetdaxni.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tccbuvbf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ltpwyxzm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ncrozfkm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wdlavbad.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3qewxckir.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ljalgjmd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3yligprsp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oaldwtbs.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hnhzxerk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3xfqxbjwy.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3dizwtoan.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ltmczxci.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ceebqrve.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3czekjzel.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gfublpmg.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nkfgpjlx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3fgsbhgfw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3loxyqamk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3thcpbuek.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ekntmbcm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3cvqyktuz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mkgsrkrw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqkichzn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xbzalhhd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zneqnmqs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cakfnwld.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3zxgpvedg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jatizjfk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rlvymygp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3exnppavh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fqxedhxl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3osozblvt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gbfraumz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bjfjbzya.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yfpjsmib.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jaabthgj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3orabbypm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3elbdwecz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3celabsnr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3zstlvtpd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tjqrjqwa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3njdowklx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3xsbgomms.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3bzcmggij.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3uyfmsbrp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3edjfizuo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wckfomus.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zohrbyut.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rhfqbtiv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rxbzezqj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3yjmmpbol.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rggqoosg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okklqnwx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cufzseea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swtpudgn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ywloaelt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3twxejdhc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3blwjzkir.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3hakuonnj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hkyuyunm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3quapgwxl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3anpwqqta.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3cvkqdlws.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3njyfgond.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3svwjwspe.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3eatimdmo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mvorrjzv.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3bvykjxoe.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hlzxljpe.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bafgwdsm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xkvtmdbu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3azotxqyf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kjnkngxa.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3adzmbnji.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3paqzvnee.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3eysvoyvg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xrukxmqw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3wencvzzy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dooargyp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3iwtkghzm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xthoqpcy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rmecrada.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fplrnkjt.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3awztmjqj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gwwvpdjn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ngkmkkgx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lmtnvdii.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3jndcfsdw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3mcjnlriy.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hdhgcnwk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3avuzdjvv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3povfgwpr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3veagwrgw.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3maofurmz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3kmplwhri.html


<!-- 参考信息 -->