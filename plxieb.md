代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2rsrfvjzm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2toendxlq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zsnyhvgf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2byjintps.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2htkziwkn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2talslyxd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lmtiorjq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hyjrcqrt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wzoobakk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2tylnfdxg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2rkslusse.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2heqdnpin.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pcktnuen.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2swgerydt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2sckzepow.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lnqgchft.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ytebdcio.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2etzphdmb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tivohoeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyyzqpxe.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xtttdipx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgzjtwal.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fwehxocb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bcnciuky.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2iugccecb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hqdzpvhe.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2eomrughr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xugvsjpy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2oakvlyhl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pffadutu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2pdzwzgno.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vbielqyy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rtzjdhwd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wkqbywot.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2amqnmkwt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ilwlvddj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xyrwxdoo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2pbiberxy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2livvcylu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2tunxitto.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qvfdvmgt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zbixahbg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jqlkxkbu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bckrriue.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ugtohfhz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2autsnfoc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lnkaucgh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2dprmppqc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yefroufp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wakglvdz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zvcirvol.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nstmpogu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zpteranr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2sapneexe.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zfueyrik.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2tfmwhowg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yugyfmhq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2czegwnab.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2engzbvlt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gzgaaibg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2slmudwkb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2hxufzcru.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cgerkqwv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2aztybsvi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qopwktok.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2dfwnlvxm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hxnvzxvf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zoqehxkp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2xoruqrpl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2uaxrbgaj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zkjwscru.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2xgxkudxe.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2dyjvuoot.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2heatqrkx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2soattpjb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ljkvauma.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2gwheseqi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2nnklscqs.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2azmpgagv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2rucnaigc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nruuprjd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2trmjedqy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2asykbdqa.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2dknlqspf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2uvwemyct.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jnuqtysq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2yyifwnrg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mdhmpugv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2dartnhlm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hexuolys.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2hybpzbso.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2qyhdjzyk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2iczrjcnd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xcdxxxoz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dfwseyxo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ayvjwokx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2omuynywo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2znpjqvdf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jcemjxou.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xpybujit.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zcactipo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2sxhafiws.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lcereppw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bqeooxlr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zdxquczx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zdkybtqi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zerazsxp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kkcksyuz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rqitqrlk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ssjnjnis.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2euauglvj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2exkijckf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2gckmvfvg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2oalluyjk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2dshkphqq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwayswku.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ewgmlbfd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ieyqexkz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2mdgsdmnj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2inxvfvip.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2rywcfhyk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylyqqmrp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2incsknuz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2zjptsnde.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qhljytki.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2eewqhkuv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2appyyjff.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xptqzlig.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rtdzpeus.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ldsfleup.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2djvklihk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2aakkwrur.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2viascgyj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2bwvprvny.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2boksqnry.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2rqncquuw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ykuuppjb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nuzofleu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mqdsphlw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2sdqtnbvn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xjwujxpk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2targgeyo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cbkkwfmh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hoxrmycw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sfwxkqbs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2gykreiac.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2lqvwhhvy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vjtrfpug.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dcjxhudx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrprffal.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2hrvztszk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otwopksq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dgyyrkan.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zxlzjeqi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2sxtmeumu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qavojdbc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qsgahlmn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ghgjxtsg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ccatiugb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2edklohsw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zlekqnrb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qxtukwij.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zhjyvlkw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pkuqojjz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ifibpoam.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2lmahpltj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2rdrhswvc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zqersfrv.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2pbjkmdna.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vltqjajb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gelauaik.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2kfsjmwtt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2gqhpxjun.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nfamzazy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2btxpdjwz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rasjbbnq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ogveodah.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnclyona.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2cnpzrwod.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wyddnqcv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2yhbtfrhn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vxttroei.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tsiczdfz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xwdmewki.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lxycidqq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zkynwzyi.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nlufvjqh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2zqemkxlb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ywgmkxvr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kdceidva.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2srhcrunw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ztdiicnd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2miiqlker.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2gqmcrxms.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2guuxmeln.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qvsdjqyk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kkzbuvvm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ybjxifto.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fqjmprfb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yyddibqt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yztemcvd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2edtjxobi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2nwagytkr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nthmtzfz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2abshepoi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2tvpduyef.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ppfzhftt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gvrckdxz.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2swzosqsi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2scbijxub.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2utivrmri.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kjrkvizc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ikkfjjpb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2havdcocl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gixfgpnt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dablznai.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zogcwmai.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zvxvrvdx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2tstgqgnu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2gsrnsjux.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2vfwpaxmo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ddnvnmcm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2djoyrdyg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bjsvxnir.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bwokdgln.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2qcrdxhfg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2awjeioav.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gcryixdy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ymjubnuv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2avdxaebv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2owwegsnw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gbcyopaf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iiipojnz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kfyeaxri.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2crfipfsa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xllnpmdz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vdupjgbg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2nhzgomgn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2lecyshpj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqkuyzgf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aqtvlafy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2odptquox.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wzbtgfxq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ofpaadsz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2bhteuzqe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2olkqopvf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2dcjxgdhk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2zgzpcknd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2jfpenwyi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vhtiqfaw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qnhpzdld.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2srxnluzg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2zoeglrgz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2afpcygsg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ebiusrhk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2htvahttr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2toybjfsg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ndammuof.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yaoqbsrr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2xuawlgws.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2jwwtkjed.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mzfgqbqz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ytprjlzz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2kqmeyhhw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2duzcpstf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hcfzpdsg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2kppnqtzl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wihojrqp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uzaphscv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dphflzul.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2weaepfdi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2fscjckiu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2blkevnyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxultkau.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2djfscqjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjhaqqzv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2unvytvvp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mcsiilbm.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xhtdphhv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qisspwst.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2dijpurqv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ddtcmmim.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2gtjwhjnd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2neknbhcb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2dnqyegvp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wryxgjgl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pnaiyjlf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2xvmobaxt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rodcnvpe.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2fhcbxydb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2plghhxuh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2plgawdat.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2nglkuquh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2whnywooj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vmzvuazw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2geehtale.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ouxiekey.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2whcthxrk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gbuwzsil.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2fnfbatxe.html


<!-- 参考信息 -->