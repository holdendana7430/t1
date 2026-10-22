代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2yiegilku.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jxgptfsp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hgjdsmgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqwkdafh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ytwljeii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckffndif.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kmnuiooh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hdwdqoks.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mnourciw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2yqsfmbau.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2owupystv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xncnmhgq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2dbxuiood.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2hlwcfzwg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2jftiorcc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hwupgned.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jpiqeehk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2whjtombd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2loagpovp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2unfvcnoa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qkwzssar.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mxvcxquz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2sqtbdeam.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2asshwdpr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xnurnvwy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2vlywnezm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2uezqgirm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wiobdvqc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2fdmafmmz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xssetmne.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qqmhpqgy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vlnqpqdn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ovsifmcb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2utoveoma.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rmmxyixg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2dbaqalhi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2lvlywtsg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ccrfbkjt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xkrvpycs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nvlivlcz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2wdfxxwph.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iurxpkyd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ornowvls.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2thnwsgwe.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2cjuetoin.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2yuoznmha.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bejrklpt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tlmijtzd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2uqnvckti.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mqampdpc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2amkjzlks.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yjnbrcin.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vcvhhktr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kfficwow.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nkpgfcbn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2aldqjmwx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hxlbfjnj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2mwttxgum.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ndpoevrk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2gfbnkbor.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2mlixypwb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2niauuqqw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wfkrlhld.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2otccbago.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2chcbkyhx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2eckxuzrh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2yusbnkrs.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rrmthjvx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qcdhivso.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2degknryr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qttcrmex.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lnfmbvzx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qsxrnhki.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfghskuh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dkwzomsn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ndfaynfn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jwxcpnfr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2eshdvpgy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qoeipplc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfyiiose.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2jxparlha.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dfhzntxj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bsbriuof.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kwusezrq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qebgxrtl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vthafusa.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2msonbnfp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vfofckcr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wcjzkhrs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mrvwhady.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wsvltkaa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2lonwlyel.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqcgtvda.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vdgpvksn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2jlhaudpq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2kleintoe.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2torsxewk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2alnkfxfz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2bpxiuyxl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ddbblgmu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wsehpnya.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ffnxnbtp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2jwjgbrio.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeipyayp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rpnpchcl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2iisuwtkm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2agqfgeni.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wjfupraz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dlrxprgo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2elqllbpx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pqzehqlj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2rktrilzw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2koqqwntf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pjwwkjpu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rjeooiau.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2lafwipyj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2yiynvkjn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wgvzphlf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2irtudiyg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2zofzkkec.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zbyxwxmn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2weotjbpu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lthymnca.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wnrxysci.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygklylpu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2uoinmogx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sotmfozn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2etrilzmo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tzgbcxzn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2lreqneua.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2stiyffit.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2gyanmxqa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dltjrhdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otvlqizs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wdzbzjtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwrpaoyd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vyjognft.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xxprqpcf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mxlgtogy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cgwnsoct.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2uqqoynoo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vklxubgr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2crggjfqq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2kghuttdc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cktakynq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2dqqtuweb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dqhwqnad.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xbeflwpd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xwxhwvdj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kjbwpvul.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gszlykyh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sgiawazz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2qbgctsgn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2beeschfm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2pxxbzzrz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2osujyeee.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ekxihbpn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mybyhrfr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2dkawczws.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2twnatqnz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2wsbglvqs.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2reyuvqcw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2dxcqsuka.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vdunspwp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2slmhheok.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2whqsffrc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yqmblcpl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2paxkeaom.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fokqwowc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gtdpvxdc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ecxiogew.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2whgfbkea.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ehvhghks.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rwkogxkr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jddwbcxn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2dgtpkqgo.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qtqkkobg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dtknlaan.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ngazbrpc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dxreqibz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nasdmnoz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ludssfnh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rmwnfhej.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ozqspmtr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2iwtjihqx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2dsyycbks.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qfytoird.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2igrodqqj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2yuvvkias.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wgcehbvj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dtlyixsb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kbkwyrdx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fxfforsc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2uumwnfjo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yffbzouu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fanfxzin.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wfahqknu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2osticfkr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ievmgmag.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2wyppehjh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2cerfwdvp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2hxtcjwag.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ukbuezrg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2seksebsi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2fseenbqy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qferarkl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pccdnpoz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2tywlmokw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wzuwhjhs.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zkhstjvk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vdxpbgft.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2uihzppnm.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cgcoqhti.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2hhvfwkqh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2afqfgyig.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2yeborqrq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2axasjibg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2adofkmbr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wtfkwtud.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pwimxocv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wuewxckp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xxzscxqa.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vgmayhcd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2bhgeyoxp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wcicaswf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebdpcffv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bkijnyvu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lildbxsr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2wgzeyluu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2omhwtsws.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2pisydlul.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2emrizkej.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2upwvmbch.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2caticjup.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ywivwjzs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ggrvgtgk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2urbraucb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hpjimsce.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hxzkqigm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ycnhagux.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zhvillyr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nysgzxve.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ibxcpwdg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ldqfjhwc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2hjsmhfyp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2denonxsg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehowtirg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2bfpbtjrc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hyufwxap.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jrqanvei.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xjylerpe.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2dqzeytfa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kqqhpeuq.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dswlkmec.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2oburhmpk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2wkolgtoi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tgtypkgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjzjbsxn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uohjimod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twpawspc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rnwydlga.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2yyzpehrt.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ymfjyopk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ewjvyjpd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2tznhunbo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2kxcadabi.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2pvdqsizj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2uwqjngek.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2mreetubg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bhkgvfag.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xtqlhoff.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zlphrixy.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ebriqxoy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2zdpiwptz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qqjexubf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hyqfdnnl.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2sogojomm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2seojqrzw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hybiurom.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lsgitzab.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2chwrdyxz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2assheeqg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ydttlqdx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fiklvtlv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2unxbishh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2phfouyek.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2qsccqrnl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dgimqoqy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2klcpmqcm.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2unaqpmkc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2teiljdmg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kbtrsgyx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2zhzarkqe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mzczyrgv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2idxeqsci.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2puvaneoz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2pljbpazi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2tsyzffkj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2uknoxick.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ocjcxtcq.html


<!-- 参考信息 -->