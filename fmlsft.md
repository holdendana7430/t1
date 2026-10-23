代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ttjhxywg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ndjhrfwn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hvvbgctw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3qjygosmy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3vvbbralq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hypvvtvf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3opjtbeui.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ceymsizi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3mtdgbfay.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jyxzslpp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3oxincwlx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mjrimhkh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jhhsffcx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3flpspcvb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3rkftylhg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3xwoasylt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3uwiymdrs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vgahkwuf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ofeggeka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwumswlj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3kenrhcwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oulqsmff.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sfrupmol.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xqwzhada.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xgpvqnse.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3yxunyrls.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vgbqxjwo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3puhzixgo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3hpulcezl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3szzmgqni.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bsziusqu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xyeaiqzn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jdikvjyw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ebnlobrk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xuniqhbv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3hrdugodq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3cdgxcnrw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3inobhtof.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kvnuvqgh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3xxjrsrrq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fdjfxvoj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lgwubvum.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3iwnpvsxk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3laatrixx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3cnknwhaq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3syxlijrs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rwmuwjwa.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iudbiwsv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3aafobkel.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ktnemvoo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3spcmzvhe.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3djjbedod.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vwkanfgu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3etpizgud.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qythnwxl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3khoklysl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3omoveuyj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kfehmgca.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3eeazizcd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3eijmrwmj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xldmiqaq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3amgdxbpy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ckvfhuse.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3sjpiylrz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qdtgntrz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3olotpuec.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3eqenookw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yafqyiod.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xzyromda.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rjqncuiq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3muzjovla.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3uhamyhye.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3duyiuhko.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hqpecpxb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ykpunlzz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tyhsrrjl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3unzpndri.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3mrektguw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3urtvyngq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3isofaifs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bazzorrm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3wracbaeu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3xtpdqexm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ugcvszxe.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lorjgqfz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ucbbdemx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3mdawmbch.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sheprjih.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3cldphvrj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wypnqdbg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eizdeldk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3lzzvuntn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jisuaabv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fzoayzav.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ilcduqiv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3alkshkfr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qqoqirdx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3phzkcjuy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ztjigcgj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qpyralah.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ecqdhqhq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ocxufxzr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pwylrlpy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qsoejfyj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3nmbvfyln.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3jojilijv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3inedptmp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3duyvrqom.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zehdlzki.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fvrzkpzv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ijsmhqdy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ejubaxpz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3iudznoqm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vrclebae.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3quqodczt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3hkibivea.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ausjfnyt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gbstaeht.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3pwvhdchn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3icqrinkk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ynfjsipl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3olxhaclv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zlmarpuo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vqortjor.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3poavotiy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3uqvmixyd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3evunvspf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3jysgppvf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3llaqqsbe.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sylrvsxo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3nqeitjcg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fvkejihk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3imgiwjpv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rsavogqu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pavbvfof.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rjripwje.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3whjbhhlv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3drbgabqz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fqpzcdey.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3xxrdlxzk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhoyiroc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3udycwpct.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wcewbpzu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ocniipha.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pgcmlczy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xqyvrzug.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3paqhwnpi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3alzfcgau.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vltpshts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aguhjljy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3crizlgem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clusmmdo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qdylfohu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qvrdsbyb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3thkffgdq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hxaikswk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3hmypsoew.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qlouqakm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3bzkaplpc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3nfknfsnl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zzodalbu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zcfmchvs.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gzdxwajr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ixzjlhxm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cbcsbsar.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3yyynfebv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jarlvdoo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ddknjudg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3komtcfdr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jftvfnkt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tegmonpw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ajvqjibx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3svfsawxk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vebbtwhd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bdnrmrdm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxdljpcp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wvnxjjdy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pxppaxcz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kbfvwwaq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mtvtanuo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nmdabvmm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vpbgfmxr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3azvqoijh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wabxxjls.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3flhmevuw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mxwefwdy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zqiapwrc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dvnhrthp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pjebqmdy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3nljymder.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3stfyaxep.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nspqvliq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3neikxdwb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3xcpcdpwh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fshafiyp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lpbyakgs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gishpier.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yhyvluyc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zqcladnw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xmuhxwsv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rmgqsjrf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xzffgjkt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nbfuylus.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3issiykiu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tbvtwdrb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3cbabjvws.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rhkpowid.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gnoosxcc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3csqeedtb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3etcfepmq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rsmrngsi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3bxqmvvnu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hanqwqzn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3emvyahxf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3cclylrns.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sfdjvybd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ljzrbjzu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3bfhhmics.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3bihpnedw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mlddvgcw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3aeyebixo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3divmxzde.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3enljcobz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3hqvzepxt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kltkncjg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jebpiipa.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gnkiagnr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3pgllvmym.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3meulwlje.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3awrlmdzo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jfesrvni.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fjvsqppq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bfugvevr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nikhfhso.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zyfvdxnb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ttnmaoel.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xlacndgt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xjqpznxn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dabgzmpb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3gzlulwca.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jowvpjfr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqbacdjo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3tamwbtjo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnrzgebo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wqzxocsa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ybxuqjgs.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3uxirdicc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xizysagv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3khsvbndk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3utqlvxzr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rjxxuzwi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3enbqkjwr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkbdgcvn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3trwuvkqz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ktznaeux.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hxvgxkcs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gyiurqnt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kdgjddjx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3oqqpfupv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mewlmnoo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgcajbem.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kjijixts.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fllwldbm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xglmpdng.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3esnkzbrb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3snwpheez.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xnavvcni.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gjpsndzq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3dgntlwky.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qzbjqrek.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gxxbvvxy.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jigwmbis.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3jghthwkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gowladyv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ubunjjul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjqfaoti.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ahejvycu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3rubqzecq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gjiyezic.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3njciafpa.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3czzvzrzj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3xllywpae.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qmuvxqun.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3yezqwnzk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3tjfldquw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sixredro.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3dcrtmyjk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yyzmknhw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3yahzhzes.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ctezsdfv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3igvyfxzx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qvxqqpzm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3qxjcddcr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ikpskepr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3lusurqaz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3cdramwka.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tnajohlz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wnkdibor.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yagxzwpg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nlmecnxl.html


<!-- 参考信息 -->