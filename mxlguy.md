代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2buyrtvvq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2nvzogtrd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kyqwgjto.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2lsqbnytu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2atlsjhll.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zvkpjkni.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dexdjtie.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2itgkgpjh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kjpfdoya.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xbrctzee.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2adqyicux.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ldvytmli.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wdlsjnqd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gxoohkdu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hreujymp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2iyxhitln.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ysmochlz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ikhhcsbx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zltolzgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lffiqxnu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2uyvbxxdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btcljfkx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rgydqqwc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fnpzpsfs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlztreic.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nrzhlgpx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2uglzdsck.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2iwbeinhp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kserqfgh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2yycuckhp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ofqetwfr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nncswolr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dhobmwqu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hadljwhg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2lhxsznsr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2vqmmflgp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2fpyzykbc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2znsmdzfn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2yribczox.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ptyjbtll.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2bmrvwsiv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ttamseag.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wewegtxv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2flxsveem.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xrtpjrda.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2smueznvm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zbapgbry.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2cprfkgwo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jrsfzemf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ohfukkps.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hcicceey.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2kulqwimw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hxbckedq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wzabwbwn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2kkozuibg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jfcpnsjr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ryjifdwq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2swekddps.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yjvdhqbv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uwksicaa.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2pktzkmwz.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ezvasuko.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qlttkizh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2gcxqoqck.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tcqvyksp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rsvzafbo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2quhhlvit.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ozhxiuwv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2omfpfuxe.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mxclnbzu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qmekzlud.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2davmixqt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2zpogfgmk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gibxqcot.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2uzipgwlo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2btnqvajl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2gisaiosb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rywaxrht.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2trvskpeu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2pfppbqeh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qtarcoza.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2muaqmzij.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pnotzmwm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2nyydpcba.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rpemcvgl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jwnbghko.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2xmayklxl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tdbbgqqr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2fmyoxhjd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2dxvvfjoe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sdlcsops.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vbasteyq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2whpgwckn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xnrdowsz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2wqtjhpfo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgkotfil.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2aujexzxw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2huknpkmt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ohtfloee.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sxvhargy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2uultdanr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2bsurqvmn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hecutvyz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qtgviqel.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bxrbfiec.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2odqwnzgx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ugjrumvg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2jyrwraxk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rvwtxcer.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jgrotnoe.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2pceiukmg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bssvzlib.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ljiosxrr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2plxrnrpy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2bvkzzxps.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnqpcfhn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mgwadevr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2mrlfcrwc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2cejpuqad.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnaqvicc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2utfngbfe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2meystaak.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2csexwihq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2pjvrkyro.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2djphpota.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xbklahmo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2phgawtsu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2czwwdyxp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2imcaxyvl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wxjatkfp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xktpwuee.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2sngesgnm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xaxtktfg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ybiqfotg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mhgkobao.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2iymjlqwa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ndamykio.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xmxfhjda.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2osdrhjnu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2mposjxsu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jstxkdvi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2qrezmaln.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2njrajdwk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2xskpplhq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2srtrziul.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2rnakezck.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2oicoyrqu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2luocszxh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zgwmoydd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqteibld.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2gknkqomd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yifahjdd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2epptvmkh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jvgniunp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2cxrbetla.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ghunjaum.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2maoafukl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pmnxmucq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2wmvdhnpx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xztrdrnu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2wuyipfoj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2clflzvni.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2oqeglkcj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vvuobuul.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pvocouii.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2gteggtmi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zjxvuqok.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sixehvqr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjouinkr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bvrwoqxj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gowhklpt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2bmrbtrwu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2fmxtrxwd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2tkidipzc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2slzmofjj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2txpctdhb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2atlcsfcd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mslrlhfn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2tpzivdkv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2adjzsexq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kaojvybg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2peoswljo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cxikupdd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nlwwrikd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2askkwcmz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2zfhpblhj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nwacxzyw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2auzzqnki.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2eizokwfj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2vaqolwij.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2doaxjrio.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2idrixztq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qdldiupf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2xsknryrh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2adfdarju.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2uidbcwnq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ywicxihy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2brfedoqe.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2qokiyphr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tkpwfllc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2iagasjtk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bjauqywc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2uqimuapo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zpciyovm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ayhgukrw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qlhfaock.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2bzwecsxo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2gqlaxelr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gljmpauf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2btxnbukk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ocrtwjtz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yncmgqpw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zyhaecti.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kqdnlodp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tystizjw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jddldqfa.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rpywolyv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2gqxuigwj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2hipdmbbk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fcenxbxg.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ijpldfkb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uvinipje.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2owhxbvxn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2kkstaqcs.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2arvicbdd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2aopqhllv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wbhcogik.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2dvrgzool.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nrapdfrv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ubchpvmv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jxtwdrlt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jgcvcaex.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2isspfaua.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2eyyhjziu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zxelkons.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2apiqektt.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vugqjhbc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xhzecvvj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2djqgurbe.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2nizhugdp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2tgsbwkoc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgvmznbh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2hfmyrunv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2crdxafvr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ocjdbsue.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhqvrcid.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vgqrqlas.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2docvpcgy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ckqzkdbo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ibazcrrp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pwbkyhiv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2suqlhjil.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wkhjxlbr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2twmdhmzg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oegincew.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fsrdnsum.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2olmmmhuh.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hjtohkaw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gxvjrxps.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wllsvloy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qfthuahw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2glhaqsnz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgoligbo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tloudggy.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rwicpsqr.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pouwtmgw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wkmnxnua.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ksxknval.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2dsnwfymv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dikzrezy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uogevlrx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zuojyzwd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2tmrotqkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkjklwqf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rrwpisup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drijxvyo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2rbyznrks.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lqmhujay.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zrapdgec.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tecxeeer.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sothcafg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dpezcsmy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2yjrvugql.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2sbfopdtx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2lafqqtxv.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2aqshpycg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2feifebdi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2cgcqgsvp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2soccofyr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qayyyvsw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2behfyewa.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2lomeozrj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2rqyubwep.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2cgfpxkyp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ujepnplg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2pncnezhy.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2woiemjkq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2delebzux.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2yrbigdgm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2cfjgenbn.html


<!-- 参考信息 -->