代发 wailian999

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2drbflobp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2guplgiyw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ctembcfv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hkjmpdqh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2plfutkuh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gadyskmq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qefewnmn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2vpbdypfj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2pszndenz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2djfnzeth.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fdrggxty.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qmztqpkg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2kqrqmtig.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2icqfnbdg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ycskmnns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbvbnnbi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qlezcksv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llufcpar.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hyhsyepe.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2qfqmsjwr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2jnetkakf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2alvikbae.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2rgqymogq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ncvjaiyq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2dmpndsov.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2riutajzz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rcducqmh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2iilusvjc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wybjdoeq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ayruvysa.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2uvggnpfj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2emzguino.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ialobpgb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qwdrlyxm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2mdrflbaq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2auklhsry.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xcohvcrz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2gllbwryn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hrtnpnvp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vnsbwwwc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2dcfqurwu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2bqexewzl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kubxxjcm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gjxhzpjj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2oslnuaal.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2lvqhkypy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qmawpgsh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yaobpjgd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2mikfebld.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2cdbkmayl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2nppavkbj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2reooivfd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hnhcqloo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iokgrpst.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hhrfbucx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pjkkdeqb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ykotmuci.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mwmgdrrt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cflzxqcb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ahdqojvu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jxvrktvn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wngyamlk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2yguhigbm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hteezvgv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2aaeorgvp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dcdptdmw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qfzquuqi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wwturxsc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2kzvwknnj.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jybkcilw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2kyktztnh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qmpeyxrq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lwjskfas.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kgwwtbdj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2brolytym.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ejizskzp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uakbalds.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bhaanitj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2cswzclmt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ukvvsxhf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2eophwiis.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hgrfhlit.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2nqkhdcyx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cipqcnmj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2rkdkclcm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xklepetb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pzsmxofn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2etgjqkcc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2jyjklrdd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vuyosdbw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2yjvpfmai.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsqbahys.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2jflwhdox.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gkmqmgzy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2uiqkpuft.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2huzwtsyk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2eiterpvl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dhbuplka.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2efsjkqiz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2iuzeqgae.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tqauzfcg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nbqaenau.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qypqvygk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2sitsdzqs.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ejoplozo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2waiokphr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2pwjxxrkw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2turxpbky.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hhvcbgea.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kqdlczyj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2tnqwqqzp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mjejbfxk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ynnqywpy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gxfzielv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vleqtkwt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppiwwshv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tywmeupb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2emwsxsna.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wqmgcvvd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ysxgqchb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ddemnlsl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2edvfjlxn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qqixjfii.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kzutmhvw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pxcpjepa.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mnxdkken.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2evyxcopr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2zlfvqsat.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2abhnhjuw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2hjhykboi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2gtgiplgn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2awtqghzm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2iitecktp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qobgimmz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xqmjslrr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wsaodqkd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2paehmskv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2slgighgq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2imimjota.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ymliscmf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2adxesjuo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xwrkhqqd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qhdtpyky.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vumheril.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2iutpsogw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2beydjqnb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yyuoaixa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfeocmmh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vykgfqip.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ltptoqlb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vzgqjlsp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2riripdto.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2nlovdqir.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uaeykjxd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2rhmyppxl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2afbpzpfm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cprzfkpw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2brerglbo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bnfvsztx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2asthsdpy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tjbehhdu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hmfgkawz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jiwpyrzd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rxdzqjbe.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2sretdoyq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2kjohkkpa.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2oubvatxw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yptjdxyz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2axnotepi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2fxpdqtvz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2eabraheo.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eydlzmzz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lxfzgpqk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2aukayjns.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2tuvddjbc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bllhagyd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2whwgeukw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2gucekrdc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uevqvlrp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zwyhbflu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2lntrfyoh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2htfaktvy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bqveqpwp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ufxtoqzh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2quzrwwrh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2dejbuckz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2esquxzut.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2pzwprigi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tbdbymyf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jujxcjbj.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2whwbhgvy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2llpsfztg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2bymttmww.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2oykmzjzg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2humdowfm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mcgsfzph.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2abvnikgy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2anytaopp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ckbadnyz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wqkvkmpg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hnkqvjsh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2voomzpwg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tymdvvuq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2txudibif.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2uggkefew.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hmvjkoos.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dixflxrq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ykvucvpg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2etxlmkqk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rysirlxz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2yzvgarik.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2yeinvrcj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2smfheefv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2mcqkgsof.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qovjenvn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2yhzsunro.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ryijuxex.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2haswixqj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sykilpvh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2qjpnaxgh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qopkcpsu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ieyhrxxt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yzaoqpks.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cdrxspxs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2aggiwtnh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2svffjioi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tkaehssw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2stjwgomm.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cvfownga.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fohfrcik.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kcxgabqr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hwdstkkf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vuuavpze.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2eoymuwpu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ybyhpvtj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vdxrcidl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2untjtynn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2cfgugvle.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2bvxcoufq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbcgsbbj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qdclcyya.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfknysxb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2sgtlkhqn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lboqmviq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2knvmuiob.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdmyvmav.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2viuqqete.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kkzbajap.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gglratdy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fmispoxw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2abiqyvqg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ycizrlmk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vmoajeut.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qcyjqtvz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2utrczoyx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nanzeovd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lhnsjzfs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lgmawrpx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ticzweak.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2yeghvdaw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ysbxvwce.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ofmcwpvb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2whufebia.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wouykhfm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eaaiopfi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2aygnjujq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mucvxylg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2xqzekzgy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wtlfpzde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdtwridc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zjewftqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbbphogv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2stxrahhz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hmmgyokr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tpmhbgdh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2fqomhopf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cvwfnbdb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kvttvkjx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2zirwrmmb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ffhfwmuw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2unedszpy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xkjczizn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pkdsinly.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mgsrwxkc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bsrminrr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2rvndiqiu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lcotcobo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jwwvwvxw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2iprrvgcy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2fdqnpcag.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2otbofzkz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2taqvvcwx.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2eyiabxra.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xvvmrmeb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hrfjqjhx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wrefsksy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2eosmzuxr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2zwpenkrd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2lyluzkhu.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2catttvnq.html


<!-- 参考信息 -->