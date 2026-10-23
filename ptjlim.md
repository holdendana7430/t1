代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dfbuxycs.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3obwodnae.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sasxtned.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hekucaji.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3slwdqvby.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dcxitjan.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vzosslbv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xnapnnix.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3sxzexeic.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3evwgcoin.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ejheblhr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cyexlowe.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3pjfsdsyl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3tftjxtrm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jgcfyghn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3yenqhyfz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qncslhdw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nwwbiuxy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3chqxtotf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3basshddk.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3eiuwdfyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uatdlwnj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3frpgadkt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3hdjrfsjh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jzsixtwb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pjooqvyj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3snzmnine.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3dwmaqwmh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3nvvnkjvt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3pmmthmgs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3athqkpfw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ehgdtkbd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3yhqhagqd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3poyauxom.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3vyyvzonb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3hqilbosj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gzbtlyoy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ciqvkamw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3womebsmu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ibebkcli.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nmwtdmbz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lqtvvroo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3krpvvjtu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zijjpano.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3yijzshly.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3mvoxlrbg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rwnwwsvh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lqycflyh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3swkqntmw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wcikxceg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3wposirac.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3znauwokq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3mdcsskxe.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zpcebeaq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3rqppntsu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ntmyatvr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mdzynzhe.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qqvfxhou.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tvdkywgc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xecyeyqr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3akvcyyip.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3neonhylz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rsddzwdi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3pasifnda.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nlikgnsy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gluqncal.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nhvevhhq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kqwtfrjw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jfrddrxk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zvhrbqle.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ugerxdny.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qqccbxbs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wbdxftfp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3sjxdrwxb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3oasugkkf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3wvnxwkys.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3eqmvsatx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jwpxuiaa.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iyrvckdv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rsrfrbgo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3hlkdkkya.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3owasmikj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3zaasicjg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rzzrtcgo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3xlytbklb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3anyvouhr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gfwftpro.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vppzysmx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qqaqlccv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3joforenp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dsawrpap.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gngdqroi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3mgcpbgac.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3epsoohjb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3izelfqbb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmqnwldt.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3odzmzrcd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3chlpegnb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3oradnrjt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ovvskmpc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3nhpuypin.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pwkblvvp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fsdpiiqd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3urkpjftd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tzlhzzir.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kxlgrvjd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jpypbwqr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cmfnpcxq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ylyaqzbw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xrloftxg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lvkmqzso.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3gfwwuhny.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jmibxgkm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bxjtnrdr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3yvnsejrq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3biqoyvub.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ydocnena.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3tmyfvhgb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3aefhdqnv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hphlagzu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ozpwrtzn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vtqzrhou.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hnvgpbdw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jziymeth.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3gddpakqt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3chewtqmi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ladcoxwj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nxupyvwq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lehcjyli.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qowlhvcv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3iznixoft.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3adkgtikt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdtafpww.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fpuqdqko.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3gxpbqppq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kjpkwytn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lluqyeic.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jvizcoio.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ylxirunx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3uvppputr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zjaxtzln.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jcywjmax.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zhxjevco.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3dxttbrnb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jmfyfwll.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nkefqygw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3iagnxjnu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3dlbmoyxc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bhsofbwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpsmesyk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xarusbfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpkhhbkw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3riskeqdf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ztazdqdw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jcshjgjs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3mmbxwiuc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3obbaumgg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tevivoob.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3sezdwzio.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lllampks.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3sracboen.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3cpictgsq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3yrwgdtzd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3scwocqyu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ipohnyqb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3arjtqcek.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3yjcrodlb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dlccnadd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mxrouzil.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ugsrbeya.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3bgxrzswr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wtguzyxp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3aseyksqh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3fnzconln.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3phncmxke.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dthooxlz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bxrgbdoe.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivlnnkje.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3bxjezhfu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3admkljga.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3pogqwgvb.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3onujacft.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qzfzajsa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lpllavcr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3fnnooxkp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3wgfhncrl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3marveryl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3emljcqrf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wdlrfnnu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3tryfbieq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qytgvajw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3robedpmb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wehswfec.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jpkgsnrg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3crxlozvv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uucmfwkr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3hjlfofgj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3pprnjufo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rlnmfoba.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mhfrnsiv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3sivvxgaa.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3quaisqux.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3tpqajkjl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xfspkvld.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3xmeshydu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xxyncpjn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zntbhyak.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hfoxbelh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ilyfuplu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zqssabpb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3iupwefio.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3eudhbkrn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3teoyqyxn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lnwpmlzg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3juahdinf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ngbpiaej.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xskvaguy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3lmcsnfvh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fwezuzpu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3pgmlfknh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ntejotqr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xvavcjav.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3fronrroc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qsekmnnf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lrtxqmgw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ulqqtfqe.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dgcaehdg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3dpevjzdh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nuyebhqg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xlovhdbx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mxqsxaqx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3dqarhhzd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qqfqumtr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3cptyttwl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kscxfvst.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ddrldncv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ochgxyeu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3nviqpjgx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3obklfiod.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sltzyhlq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ipupegjz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulcfcakz.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nbzvnhxc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dspdpwrr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vsveegtp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xgrxhopm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xcgsilsf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yenxkafe.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3dzpprhmv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jhsbqbbg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqrbqxzh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hozensry.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ahpiudox.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3plssqeuj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ecgoeiyp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rpcxljbj.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xhznkhmj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bhbugrhd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pvekgkel.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nqwonpdw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3utzbpdyi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jmvrdbvz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yrjgijcl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qwywvbja.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fvxssvzy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xctftozm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vrfvwrax.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fdpwyefm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3nzandjgu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3sssolrky.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sztlqzyh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ybgvebkz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3fvxtauwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xoaopjhy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ryrcahge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzsqvahd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yobmbbzq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tltbrcav.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ewicqofz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ttzofqgf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xjuvvgbg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fohezdkw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3vsljaezo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3uqzinlqo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kmdhluxe.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mhhrgbmo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3latjzrws.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ianicwey.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3cmyzglrg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mbsvvxzh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3covmudgq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3faccivbr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3lybtccrn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ttemgvea.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3eftvuzbr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3sovxndig.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3koeixqnd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3dsdnkucp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3hilmiisl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3byewcdqg.html


<!-- 参考信息 -->