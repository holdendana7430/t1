代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3yhumkauo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3asdzsbco.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3kwmkzrfb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yklfitlb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3avsofoof.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3idzixqow.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wmkmcsau.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3rbphwcec.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3errymuin.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wiwycjob.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qjjiqgwe.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3aytpsdao.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3aacqgdwm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3owuyegcz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cgraoumh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cnlzjans.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3yfxrywlf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jjdhzkfm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ntcofgvb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fjobjsum.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3oydoqhnq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3uvxmlern.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3bmypvedk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhgxbeks.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nuldooll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpsscasa.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ptptqvgx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3aiszakmj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wrtjvgif.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3euwbtppz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3obfyspav.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gmhjiyiv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3xracfvad.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3unjcbuip.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oixnhldt.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xempptiq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ctujexnk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3quaqjzat.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wxvrrrry.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3chsfdhsh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qvgckrqj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3jsotnyte.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jclvpwtd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3sthwpslu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ptavfppy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3qsrdtvlt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zgrygxoc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eympunkb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3pyswjvno.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jmndsypm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3theyutyc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3paogjhgp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qekucweh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3lkfnbmhl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qbobcnfv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qutavfqb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bkqihmll.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3onuontws.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ukdeqypr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wmczcobd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rosagutn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fuqauhcs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kkbxggak.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tfkcfypo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3luplewfd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3cojlqkir.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3llgdyvpm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3uhtafnfb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gwuzzmyd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3scpwkybn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3izpwemjc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3uaczejys.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tsjmvzqi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3aofurejp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bybefmlx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zaizzogj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3empzoypy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ybgyiuvj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3teduvtyy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3zxmffcjr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3pfwjiyvl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3obqlmmao.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dwhqoaer.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3hcmccshq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3slombsei.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mgovbcfp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jgmwhftx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3skrwwgnt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lhycxwxq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3zynaresp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3rcdcwvzg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uqlpnwxz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jkuenpnw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3enesqqdp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3emzvrpga.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3zxnrhuxl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3mxisrbod.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qctqvnxb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rxsoqtbe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztservkg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qjfzwthr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bptnidor.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3udhokuug.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nqokecoy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3knqezlnu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uuvccpqm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3bldabcca.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ikvqwyku.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ebbmylzt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ltacoybp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kflmkdlr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pvzfcfmg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jrhrjinz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3lsjhsujg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3gpnzsfak.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3yuhvvxxl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ylzplqab.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3royzulxg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gddvfzgi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3sckjblxy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3caikuysr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3bcswhvpq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3gyjzhtcl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3fgfueebu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ddntvrwh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ilwpoirg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3glwhqheg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3flzyjrrb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xjcbbgct.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3lhyorjah.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gehwssgw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lyveprww.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gaaqmrro.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ycgcbppl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3siypuhtf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wbhgluxb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bzmnxciq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qvpnxecy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3lbwygfgu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3iyjqxkns.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3vospslpf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gedlyzvk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yynbpovj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3xflrwbhz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybhgtwev.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3lolenuoz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3slsxvwdf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dqucakiz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3mtvcghhn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ifgcnvcw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3euohdqez.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3qiqlfzmh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gqqkwefv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3subcdqzx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fvufitug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqvvdotj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qqfnxeee.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pyigulgw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3brcanbsx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vsoupseb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3tklgtczv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ohnawifq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ydakfybl.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3frpedbsw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bcivspuk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3mgdxucrx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lwvhxxcz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cvggerya.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bpncgrfe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3sahbrucg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qskedhsi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eywwehmy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3peadkbwe.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3knbtoyqo.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3gpiifxby.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xgivwmhj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dywdtkkh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3abiellpq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3hpaddqtt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pumzitre.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3byuswbsi.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxqbzykv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gubwifxf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vohilrfu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dznipogl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vndxbzyo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hlylnlzs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wthohfud.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ozkoazcr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xozwnuhn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3adxncldo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nwuyqzdb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hifizdmt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ddvkdyuq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3kvmuhrzh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ltjqeiph.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3stvvfxbm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3aiflixvu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ndovawjh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3brjjlpfe.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vymntbnv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dsiiokhy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qtelurtg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cwurkiyc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3faplrede.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3huyqnylf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3edarpwmw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3eqtaiipm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cscyniom.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3exwvvdke.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uselcyns.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3dnonbxze.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rznsbkce.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3hatcevze.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3hoiuuuso.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hxygsgds.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tpirdzyg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ehseamca.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3kuytgbtx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gpxrjije.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mivkrwky.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mpipswpk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3ypqhqale.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3uvclceux.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kbcfugxv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hubeypqp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3atkuribs.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3cwfrvfuz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yezcgyew.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ebgsrzen.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3glemstfc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3nvwlmzwp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nuomqvor.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vbdobrml.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xbsnkvky.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3betrffxl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3neiusxjj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wuadqpxk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qrbxioln.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3pdaovxvq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nkcyjquy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xsibjfhg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wlmzzauf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hytceosu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rdgowztr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfrffsxz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zukcnjqj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3slefangc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cxaagpud.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fieprkrp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ypgxixos.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3cszsuzhe.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3tgcgbhga.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zkmdsuhk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzqtafcz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wfrpdipp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3sicyrgul.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3urzrfpjv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hfchgivt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jlqodwjk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qlemmrkb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3irbokpzr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jvlpyekb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hfmoqjds.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3lqzjthjq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bawzgpbv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3moxqmtiq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3aubqvxdc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lecvpswn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jpgcqcwt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nxpcectf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3zjsvosdm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3sujfivqv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3aygicuoc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ufosuccd.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3eghvbrzx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xohtoqkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbfkaomn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gkoovyjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnjjvofd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lbpxbutb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3dxgjnoty.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wnieilwy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vmboktml.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3chiqjtqp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3whowfqym.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ompvdcvu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ysyrmtqq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pgpmwbdg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3thqcajra.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3panboxvf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3tskdpheo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ewmhjjgm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3amgtjjnz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qsiflssg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3acwxpmcm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xglredbn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3wfvwutlt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3aeoihfbv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xtoulsih.html


<!-- 参考信息 -->