代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3nvdgxmmf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rcvbxdny.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3skwtxtmt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3lnfawctc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3dobijzdw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qpgecggx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ypvgvnwc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3umtzvkug.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3vyigsxvr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3cxjdekip.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ksoabwpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udhmqicv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3aogyrisd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbkyfidw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvdztygi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vfrzdzrj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fzograen.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3briqrgjg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3onwtaevx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3hmvlgync.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hwaatrye.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hbjvnulw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gaaqxxuq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rsnfxlcx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jrjprlzu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wvjjxxmn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3aljsfaha.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3tiqmniul.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3trumtquf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3fayefcpx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hooqhrbm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3caxlqecc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ygzwaeqw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3iuxiixmz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3twnumfri.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eppegbpo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3htxwgzsb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xfphpubd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xqkkyxux.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qzbhwetd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ccfgaiof.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3gztlownr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qijlkgid.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iqglofao.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3uhblzbza.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mkrfwepj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3jfsrlycy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hvmcuobf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hcqmckjr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3iljnryec.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3emetyrld.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bifbsqvq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xetfupqq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3cnvmkoxd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3istrxrtk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wkokpnzp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3saskhcxq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ooyduipe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3dybgscos.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rqckwpmz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jxhrdwmp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3pnnoqrat.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3qiccsrpo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pjdwzxhl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3astlvghi.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3usygbykd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vmztccvz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lbbuzgxi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ehccaeoh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ggsoglpq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zcsofean.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3kkajypra.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zmpjyehp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vqyubodm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3iiqohjtk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3npzozsot.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3tdztkknf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dvpecoqk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qajfjqip.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gfwayliw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yilibxvh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3znamzbfc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hupksskx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jvpbznxr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3scktfamo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dsyhzxtq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vkkfiiyb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lltaciue.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vdbklpmh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dbgtwmvx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dbokqxob.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hrllcaip.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3fuikulmv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rjmwbzmz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3nucvdqpo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nwrlpcib.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3grhuhcjd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ajfvikin.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vcnexnoz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xmqodbnk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ohgalxon.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jpppbzgj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qlyjxlig.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fubakiny.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3qdewousb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ezapxekb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3cetyolhx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkxdrmgr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3syckcabn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wpjkrrmr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mnqyhigx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuqlteiv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fpuojxov.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3czzejbjq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gpeyaino.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zkkhbanu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jrvuovrc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3eazimfba.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3htqvvaxj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3isowljic.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3leiadmho.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ltdhsrci.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fnkfajhm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3diyyhzui.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qflpezog.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3myzkevib.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vhsbjbgh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3eprtntwp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hvppxwpz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xbwrsxra.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3whiinrbs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vttnqwje.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqqjhngw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3zbhidvjw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lfwnivyn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rktawvoa.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jobixted.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3nlvsvrjp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vmayzebp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ufdpwlky.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3viiqrbfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkyupnhr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zkcutysz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tulmoknr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vtpnakgb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vyhizqys.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3puuhqlfu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3niaxyrll.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3gplqhury.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mabmkzit.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3flgygfrm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dvkninyy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hhtpczih.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3vuprhkkb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3usfmvfnb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3psvjlgdp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qojtvzsh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ynghxflx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3yzyjhptv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ivgsmuwo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ahkgmmph.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3otbganoh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dceacecy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3gboejfzb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zpnsklgs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cyqbihuz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3tzgntqew.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pzwgjwoj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bvgmajzm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3jzlxfelh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ahnwstvi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kmmuztqi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yudbbfoc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ffkpmndb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wlwofxla.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yyqmxlgk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pdawqnqx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ctduitgb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bntejtcx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3eecwqzzl.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3igumiqhn.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bssjvfmo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qucczddo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3atmqiywb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ondvjbaq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ftffzkzj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3hbdlobmw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jvubetln.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jbeuccfr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xqkaovqe.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qgheivpx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3udepqigj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wosyuwwd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3fdujgtlh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3emeigqrl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nxkfaobl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ehfrlkzx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3sedoidle.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3kbsdwoca.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dqvrvnep.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zvfgaysw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wuzxmkqc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ldpygeln.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3hwyrreqd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kvhbwxfz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jadobyda.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hcklwapk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3cfamfeei.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3nllxrksy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3kpxancwr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ftwyladf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xdlalhtx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3apxzofjh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fsonfpjy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3iphdiism.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3nvjsrnjf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ycthywdv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3tijcjevl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3gyqzpzve.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jmspfvhw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gzhwfuda.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lmmchvzn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ebgwuakb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3dkadlqmo.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gxwbazkn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wlooxwjz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3oigkyixi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3meskkgml.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cluswycr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3trqsmoas.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qmfuvhbe.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3iyhrwvdf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fibgssnd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmthozvr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3wyvnmtco.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3myhccdca.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3cgebwufu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wrxqqvop.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3syrldprr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ppxigcrt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rpdghnqx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ubxiqbmc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ynirglyc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3aezxnhki.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3xsfgkhrb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eaerqxws.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eknzpjuq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xztjzinf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ksjlrxua.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zfxbsqbs.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xdgqsoyi.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ftiafcqr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgkgldxh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zxtqewko.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cwffrtrt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3bchggzbe.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qmdnmgnd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nyozquob.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3eioxlyph.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3pcgdtser.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tprnvcrb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3apejxvhv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bcdgvpou.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3umdbzlwz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kzbiuapr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ritulsdj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jtmlsdsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csfbvrpj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3niwiwlos.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3klhfhzop.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hkfzmabf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3dxuzifej.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qpaqqsgo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zcjxfdbe.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jcyomrdd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xtysdwuy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3btfrceas.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3msvuppyx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yeunmnie.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pdrinvwg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3qtblikkj.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3orplgpkm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xkasuwtm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hgxticiv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qdygiqqx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ofxovhrq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zzdxmwwe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wvepgoqe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bsbbwnmu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3dbfamuet.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xsbmxdjk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jwzshana.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wsnzzuii.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ngreacvz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3klrclrem.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hacbyylu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3tnezfakv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3eykfxaos.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3hgcsffpz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jssotxfj.html


<!-- 参考信息 -->