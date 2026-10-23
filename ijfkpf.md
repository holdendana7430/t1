代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3xvpzogby.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ikczxxay.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3oqlgknnz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kvhyyyob.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gnulysbr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3yzhplylr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3djqsacgq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hglsoall.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3emmcfhiv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vgfpffdm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hmyyvhwk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lhnjpuxc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3toiponug.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mxgtmdcg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3nwjjtlqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iiamwimm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3twmcultx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcxenhvs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yqvnjlco.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rvqczapq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3canzbtnn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bmiknipk.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3raidhwbq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mkqgqlxt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wbzegrks.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3znticnsm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3kypemsqx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dddmntqa.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wdrhvjtl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yedejzil.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wcgsajna.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3myiftpri.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3adilbydu.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3azamxrvn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3iejrgruf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ytejzzru.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lvpgwcxh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3touypqft.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rqbqkoly.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ygatzsuf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3swtenxca.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3csjgdmbt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xnyrckoe.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pvfoujxj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mtdyvvft.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ogjypaja.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ocdvswlp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ghwnvgli.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ymehkbpi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bppinakn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3iwisgxmk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jzpdldtd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fhkyjhsz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjeejtoq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3cieiyyqa.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ovxjcbjf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3sovfjxno.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ywldbjsw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3urnczzgb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3oqyxnhav.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3foqtvwvm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3dujznqnd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3vkpjzgce.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zmtfqyuc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jvsoibxx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kpdllvsg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ddenjjge.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3sxieryat.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3odabcypu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3cyvfnxvj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3oqdxrfyk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3irenxooq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ahmvxepv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3wtdrcfaw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wcrzimpt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3umjadmkl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pemshiej.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtkifusj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pwwqsnmo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3yrebnufe.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3brylmlkk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yajdukic.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xvdyjwsa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zuxoaywu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3mtaqdtwn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3wykrfykb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mcwpbfgt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ubkcsuhq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hypckmls.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3dacxfjnm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3jskmetzf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3durpgiie.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3febwduvv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3glqknrdh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xsdyfrgr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xinnhtoy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3dikcwopb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3tekfcyod.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vhohpslj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3blghxhyx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ultadaqr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3irxzkprt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3lkmvzoox.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bkigohwf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3tojlazbr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3oxnxxtot.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3wlortvyk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ozjovypo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ofzpvilh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3cmvtiehl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3esxouoee.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ysldnqup.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xgnmjket.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lrzcihjl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rkhavenp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zkpqhedu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hpucxxwd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpuiwssw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jfzhdzor.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3poqbuefn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3eykrglac.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dtpwuzji.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mjfbeeka.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xhsmoqhu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ltioylbr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wfsvvvxh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3zxjlbupa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3sutnduhz.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggnmbnkl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3dxrgvsva.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mdmbsvvi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3eddvivmz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3snaweaua.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tfotqrcb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nzmtfxne.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ilzmuppm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqiiebws.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3pqmqybdt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3chxhjoko.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qpeljjjt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uqviasnu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3rayfohtk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zdnxnoiu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ccjsghfs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3awgjfghz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yhrotiwp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kiogobew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yezwfkms.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ccmwzdgk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rrormgak.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3yrindxzu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hxqjuccl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3sjkjdhye.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3knkmplqh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3yfcmgqmk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3mxqjcowx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dqwsalig.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pcwfzojg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xtwkyfeq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tgddjiqk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ciuasvmq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wofjgrsh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3idcadnyf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jnkvqypw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cskonxvd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3upurlfrd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fxvuhgco.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kssqlbxs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zpltfipr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3dvhsjxgf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3blnpdlzv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejmprewu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bfqlkxlv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3paeuuxyo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ysuzezuu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gyumyblc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bimwtksj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3tyobfvyc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ubnuvbxk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ylodaojj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3tfqfapgi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3bcejwnpa.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tmhuzjtk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lnqckckd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3dheyypzr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xklrbajl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wkppjsvf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fmvplpfs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3phbllqba.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bdantxrc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gkqigxxw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fckuihnt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3fbojqbsx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ovbsuufg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3wfnaqwju.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cdavltar.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3tvrxabmv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3imnfhktt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3cioscdjf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3pmqlubtj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3icnuhcru.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3hsoaukez.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zuhxqqme.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rmigpddq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ncxsbwco.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qktosxgv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ygjfsnkf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3bqmoxtkf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jtytvxju.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nqcjwsjs.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3emjbbiye.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3lcfrewud.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3egcambys.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qrbkixqv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3jegnuvss.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3krtuskhm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3idvmjrem.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3pbtvojga.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gnftymmx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3mkxqanqh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3preswero.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jrfptiml.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3gublcdpg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ovpctaqf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zlvhelya.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3agwcltrv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dyludmsk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zohjgnwy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3navnnaxn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3auvhblpm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3pjlwxtuz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jenvzaxv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hyllwwru.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3yqvlrcdh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uigfzqbg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ninrghaz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ofximcnx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3eannjfek.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3izgxedfy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3bqxjkkvv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3kckqvthd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pximrknz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3elymyzyy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mwwbkuyx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3sdjqzllr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysircshj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rshxnlyk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3pumylzvk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3cdymxicc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3chgqnmlz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lxoxghhn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3kpffotvs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ohlborci.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3izghertp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ffqpcnio.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3psfzqyui.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zgvyttnb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pqskwodo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3bklypfzn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bgwbnvng.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ggjqevaz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tmdufsio.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zuidpvnc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3pjpfqdxy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3znxwtedd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lsgsomta.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lwtvnckj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3pepplbov.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3rcqnyaxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxehwcuq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3afnagycg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbvblfdo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3hvhpxrbc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3csuikzif.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vgoomofw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ireiafzu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ffbpzuik.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3fgalpepn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ggxgqrho.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rdvmhvaq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ererfpzl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ojcjduax.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wtspvyox.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rqisgzcs.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3nzwbrloe.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3herniwxk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3uorerfhp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3tlfnfwds.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3wybirzxs.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nhtiawgz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zolaalxx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wahuretn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3sjqrdgwp.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wossovde.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3iqaaoqlu.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wfwsfqae.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3uwvagxfs.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ioubdmte.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ngfldtct.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3odfcgnhc.html


<!-- 参考信息 -->