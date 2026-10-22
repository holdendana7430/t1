代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2qjrrourl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2cjlsqzip.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2uodnikwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jaluveqa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jzipcons.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okjwbtec.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2okabvnlm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ilqpwtqk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpxmwgxj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2obsfhuuv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2syhvbexs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yntjvicj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pezqzjuv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2wetigtlk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2vmunznpx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yrqxcaje.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bnejagje.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ujmuchix.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2baitzxgp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2cumwvgtr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2eybbfmmt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hfsahdxl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mnfavruk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2paiacxcl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pvzdbciu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2opnmdzee.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fxrokbfw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pqlmhkdl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mlytqise.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hhtwddfr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qryyhndg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxnmmoyq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uclmszhr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xrbaaaae.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pjalztvw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rteypeph.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tnscxnsw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ptxqbiko.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2txgwlfxf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ugnlrkif.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wazyjgrl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vahgoskb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2mttmdnwo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rqbcemxh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wcbzbwdr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lyvhkxab.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ejmiopdo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ipgcppzz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2suxkbrxr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wcgydyjj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ifecjiou.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gbrjjhnj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zjeikytg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2gwbzqkel.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2chrjacnl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2oepbbwat.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2rgvlbdgo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mxxhjoob.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2jooswyqt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ipghwgdu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lpxbjkuc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ojbrgkiu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nwmpdxci.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2abicxfrg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lmywbpak.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kiqdljkh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2yeqfturo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mihrsdbm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gogjsvzm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ximquhvd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qxvohrej.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2djhtksxt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2rqbcnmgn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2avyialmv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvtrvlsl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2sztrkojz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lfswmwuw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hnbgsgom.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2wypwtrgc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvwwwrjs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ntfryqlr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hsxfbmfq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2sqkyazqt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xzddbrcs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qtuvcyke.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rxclvlsf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ychodjts.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2woobafnw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2xcpvvdhm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2amiduxux.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2bukknfsz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2opklvghm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2xojudobs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2wrsxmbzo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2amuazisu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xisnvdvd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uppbkjpa.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xdsxxfwf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nhhsqovc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxaslczn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2stzsfbhl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2bjvokiuv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2tqzjdbao.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpiebulz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fuqlndoa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdgqjsyn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgtvigrb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kowuftay.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pkhdmnsb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ologkzqo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bjkqxxev.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vcmnflsc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sodhqoor.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2cluextdd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ubrixeqb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hywqhmuv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkzrkrrx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ujmtdeor.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2vkpfgxhl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ladfpnok.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vqaxgzqs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qpsmqrwt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2skdkfhmh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xskkmmlu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkvtfbid.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2bulonuqg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hxqujmqy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2kemmcaun.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iadklkag.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2coutdofk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2gkkpvvva.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oyunizji.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tjsdbref.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgcwbiiy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mfufrlvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqiuvloj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qevnphxz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rblifyfp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vwxtvjhc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2gcozbjro.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2cqnadryb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fqvpqxmm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kuqzopar.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2dzerbuho.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ybbywbqf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cmosibnk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xysgvlcy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lgxjauau.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2eruqxtyq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2stecgjsa.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kqmfyfry.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2khffjajv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2hcwhduqg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hqpmheko.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jvywbdbd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2novwabmv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2xzrrnsnd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2tcexpyhj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nwmgekqn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyaieglo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yqemstid.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zwttnord.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cytqyecz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yvwvcbqh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2lmvndbhw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fiatxxjv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vftodine.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rljuteow.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2niuosfrr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wghrxacr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yvndjilm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2afjiyxqs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2cricapwn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2nzpntreq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2rvbbfoia.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ugzmnedt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ajoaetfm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vfnslkqd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mrsrzuid.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2cfhtawpm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dvelqubz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2llkrzhrz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nohcxzvr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pobxdans.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dkafyhil.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2kkkwsrex.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wxlssmps.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2uhrbewee.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2jajjypkp.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2lfvjwgwv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2goyyvkon.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2obkzrmht.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2afxynjfy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zsbycsho.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2aouujbhc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2nomwqunp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xhhxivpj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qccojdro.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wqixtukb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vebnfaqr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2etlnfzwk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ldlbtyqv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2zqbjenws.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gwuraelv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2mfcwajyb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ysofacgv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2drlffsrq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2szwfhvdm.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2umdjgsao.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2deeurzym.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2selqawsq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fynzpefw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zzwqgufg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2uaouqfcu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2qhhbxhrd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2vstcvrvn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vptzsoso.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bcxtfpip.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2xkbtiuzs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wwkrerre.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2revjkbwu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ldovlvcn.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2klpeotfq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2eefpdbhi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2klljtzfx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfjvsrtd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qkrhpbvj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2kehsybar.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2cfdqhjag.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zsfbwqvi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zifvjcek.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2hzcxjtpc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2asqngwym.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fgucyjdl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dglcchdv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2izjiwfqn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktautbnx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gzboipnq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ytdkgchx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dhtbqvqa.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2tsywesus.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lwwowvxo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2enhlluzr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2asnycewj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwqzkwkl.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gpjtmnwj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2gvrjkeor.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pyawfumu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2iepiajcf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nqlezbto.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2koyvcplv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rrmssunj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2usrpgubr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gibfkwjy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dnsxoflv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2dysdmuuk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2zvlzzltx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2surnjais.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hqwdqpog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxlyoquh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ieteucxy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2aqmrucdh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jtkjpcwe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eirwgiga.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rlikitzn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ylpkhblk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vpylxvxf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oghmjhwc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2jcqqzuji.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pkusvoof.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2thikcnyy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2fraimoaz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lrafdyvh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ytkifeyx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2vwyiwekx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jtodtrds.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2xtjtwwkh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2oxsrrckv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2xfaajilp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2jvtfdcjo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2euqlmsxs.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ruwdryje.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ogcdhkgn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ugahrmxv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2epabcjsn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2aasznzob.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2rdtaihtz.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pajlmbok.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ctmymugd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2gaojpxro.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2xufpgqfj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ytyvhrka.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2lsrghcuh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2dzlaqyhn.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lnlondcf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dzrwdppb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2czefltcc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2obkjirvj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fhkwmagp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2gjgjwyws.html


<!-- 参考信息 -->