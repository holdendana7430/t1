代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2bkhboyis.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qutkhhth.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qujtftko.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pllcbwag.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2nqejniga.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2scvlzxih.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2novwlcmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uornpfbk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mpuzhwxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gceaepnz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pamvuslf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ggvuqqvd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ngprgetk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hmrbcjwz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kafqkdhq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ioweqzhm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2tvpnlhoo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2snsmzyrv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ujlbkzzh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ostpvolh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nhaxbqcq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2emmexetr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2itpefvno.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2quejrpmp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jhhuuxib.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2plwqcjuo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2flbvuchi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2neqwgxvj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2oracsamg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qqjedctr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qvatmvct.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oardmizm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gtscinol.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hassceet.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uvgkhcyh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vewzpbcp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ckurdfaw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wknveqfm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2vwkvzykv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2scvmxivu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ghqyqljk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fijwrmra.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rzofhhkp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2oztivqgc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2icuexwhf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jqkitspv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2krmbwxcq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2haqihiop.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jaqzkyyl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mnmegwuv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cymznams.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2dsddotnn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ngtcwioq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2fhvowcpf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zjdnyorq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xpdpiatp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2czinrafv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2acemqzbg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2chtzrjjt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dvspfylj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xgtqsagk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2msztslsj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2juahrdak.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ptstrqhy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2aitkprfa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ebzrbotv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qryzrjrg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2wayanewb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bcsfiibm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2dlrtxijf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2aecsklzu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2iavpzmuh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ovecebdw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xchcugcz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nznkncmg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2caygpjym.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xoxctjsd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ptkeulmt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2isznjxqy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2cqipcfef.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ivfrjnwc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sldztnnm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ywkubsan.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2etefxqyg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ccmaylkk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lmofloal.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kjstesmm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ssluemed.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ixmgpqsi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zwgurjif.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2auuahybg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ndcjwvjc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2eolaspgm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2uutqlcgx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dvebcntw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2homwvtlo.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ywmdtpjg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2cdawuwpr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dvmuqngv.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2sngwuirz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lllkcaqj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2azebtovk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2itdbhqze.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2usqgsawf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2uvsgyrnm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2omsxyvuz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zwylbzkd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2mzqxagzn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2utkclinj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkdqapnj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2glatgcbr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qjhafnws.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2jcdhmdlb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2unymcboc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2zxhsjunt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xrwurmej.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2latukcqd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ospjvpqp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2sriuyjlf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2qhjfayap.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdskvrqe.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qbsnjfof.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bylrcjgf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qaqwbrmu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2twxakrsl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2cfjswgce.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vgijsdbp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kwkvzpvz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2mcqgjtsp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ltifezbc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xjopylgv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2amswmkof.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rtrnckms.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mafvzlcp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2smuylwvo.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kimjphug.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nevrehek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otgmdcvk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2atjnctgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtbjakph.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2smiiggfj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2aadmygmd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2kwxxffba.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2bzeysiyz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hnxmcriy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2edtqiakx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2twvicezy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ynjfxiwa.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fmoepwii.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2zbaievut.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uqhfuwko.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uicakzhi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2esrtejmd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2iixwozrh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2uehomxqf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wjpprxqw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2drcwekej.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2rakgspip.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2pfwucmqz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2qkyjgmvt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2yqhtueme.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2auvvnmpz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qktreyoi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oplfjnvv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ivlfczjd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2irxoizha.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2unnqgumh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2djwkjbvq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2elzovtxl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2rqsbvhwr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ashkdqjq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ihyoctbh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2tttftbly.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2eldqomuz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eqojsjsg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2bwybynkn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mczuymuj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2jphjooir.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vpztrmtd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ovnfsmrw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lvflcybs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2pfbktixv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mnciikfi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zjxwxxxd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dspwnooe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ovfycnti.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tzxohfve.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bhxlgmqc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lpopgpla.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2etpjejvj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2jvpgsjco.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pvudohzg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2oenobous.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2eexzgtgy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2bgddvfup.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xycplhjl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2xvbilhmm.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ppfkbduw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2nxshqamf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qyrkdbih.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rxkfxrmy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uasltmrk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2esamlfhh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uuhzjddr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qnrwnnyr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2hbudgvve.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2fbdmljap.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2stzvathq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zljmduwa.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2uenqhzmt.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2gpfjyaed.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2dxoryeqz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ytussyta.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2optibccv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wsheveyw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2qtomuttu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kvqpzxdt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2izjzjuvc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qrzhssnk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2spgesoht.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sffgusfb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lrtppzgk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2llgwcbya.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2gbbrbevy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gbfcwgvp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2bgizyxkn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2fdkigxhp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfiuapvy.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bxldcucq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbjnqxbu.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2sorsqbni.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fdmtymyz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uiwdxzhi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpcygcrw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2cawrykmo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mxakzgwp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwmmlvhk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lcsciavn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxyfdwcp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2bpgqmjxk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2hkwidykp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aeckjkqy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2urqbpdri.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dkzxxhiu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qvoycarm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oydvnnfw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2endspope.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gxennsld.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2cgqpjqcj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sllqmyxb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2efgxpuia.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2oqzbmmqw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vruqdati.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jjvzuqyp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2owpczrbo.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mtjqhgqh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tspceipt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2baxwkofj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2abhekrgm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ywsjirrv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2yxbmjaga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kygkmnoe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zfhzsxsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iignnxea.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jlqfhten.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2qdmjhfqk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ujcykjbv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2padbxinu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xqkrandb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zxwvrekt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2jacpdsik.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2skwfcsrg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2iqpdvbmz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jtzlqgyr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2oyyirjvq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dtveyoob.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ejdhftpt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wnfnjfhf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2cqfsowam.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2gnddltdh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vnqdgtup.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2mowcvczk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2svpnxlpx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2vmrehtyk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2spkzbiex.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2tueyzolr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2amwuukyz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tpldjdfy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dircidns.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2vmywzpjp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2rxacybzi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2njvkljcx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2muwmajfb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2viqmxduh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mhkoabum.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ujttkmxw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2slepdxnb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2zpyvqaiv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2yasighsw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ukmukyga.html


<!-- 参考信息 -->