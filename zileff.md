代发 wailian999

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2hcgrpner.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2isxgygjq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nexpebuw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2iavovbuk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2dygacdiv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2mvohgrnf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rkcimvwz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zbyolkug.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ghexombf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hhyemfsg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ycuxwfnk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2iljqalvr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2faihuaan.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vksoxtgx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nmeugzln.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bnaxwkip.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ljygwijd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2gnvhmkig.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dvapanwa.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uowllkuh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2mfklxczm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2llemkhgf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2peodhwvn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2qavkqtzv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mzkvfzln.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2plwqrpwh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ykoymgzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aiunvttg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zalfuqto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yociysre.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ubwpfohs.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2yimswdft.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyussahl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mnzvxtpn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2anukjian.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ywhecwyt.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2beqkltyk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2odtqaiku.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dpvcqjbf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ssudskvo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwbsgsgq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nkecfbdc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2thahjuyb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lddvejjq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lzuzxtwl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hfpshztr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2fhwbqjpj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xyhnoqjp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jlmxygwy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2howurjhh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wpzjlfoc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nsnlmeyy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2dngxmyui.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gdplxibg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mbkvidnk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sywxygpl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qkjnswux.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2nlwlyull.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2yznktfqn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pochjmbi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2letfzxaq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2klvtkdsu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2eezqolib.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2esxqksnx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2enwznldt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2whabznfe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yfowpknv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lzekfpzl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2potkwkxo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xbzznbxd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zkhfeclb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ycchpypn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eqlyctgu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vbwzcavg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ohqdjweg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bftppggq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fojchyhk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xhmqssor.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2hlafzaur.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2yxtdyxzo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xmksfqen.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2lcxxkoij.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2cxpaphng.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2dwoeowai.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xvmflqyq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fakgmjgf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pnvcggrq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2sihzwnav.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xyydzffp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2uwsnmysz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2rlconsnk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2tarsxzrs.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vhghtwrw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2yegejgzv.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2flwpvkwu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2odsjwivu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vztogffu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jszenpco.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2grfesozl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2txpwshvz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rtqygauc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2zsuylcnw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cqfrpkio.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2nmotcbmm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2xkhjarkr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dcwgtact.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fnygexnx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xbsifxyp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tivxypug.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2veosyppy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2nglynuil.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jniadwfs.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ovrspdbo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kltfkizt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xtinjyfb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2pqryblmj.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2cgmcrtph.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2shwaeswm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2oedwrwre.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2wjtcrezn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2leosemvs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2avdksdbv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2qywlionk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ufmfplyq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lmublbyj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hsrdhzfv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2msuiwxhm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zafxxngq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2coymycal.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfqvbecy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2owijevhh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2clehojvi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rzvfiezv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbdgvczu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bwgcuewb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bbdwnvhg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cfefmjrs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gdbyjndj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2azjextpe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2yrmldies.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2yflgoewj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vafwksqa.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pxptrcgd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2pmvylfex.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2solbjgbe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2mzicfxar.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gmhpktfh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2rfrhvbyt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2suullytd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2tzorqbsq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2psvjllvq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qfprlubp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pjxuihlp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dukjvqhi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2chyvjiyn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vwegflav.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zrieqhyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrawtbwf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qmgbljxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grghrhfz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2khjtdhgv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2soxphxqk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ohquglhs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ibguxldh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dynookfr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bqptjqsy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cydfdilm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kwobglwc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2balekehb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wwhalgot.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bufcxrjc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lfdhyrmk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2crwnodsp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ugbmayxu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2yzeiyujw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kmwjffpw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lsyehlqj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bkgpyuts.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nmvlwugs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jgedjowp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2mmmksidj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2njfrphbm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2aaekiocz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sniksbna.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2obmldlzu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2tvymxeyk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ixrrafwr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2doqljkcw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2texgsgjd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tnurizos.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2haupvvga.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mwxlemvy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2txszcvar.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ikeyrrnc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hmsdcqzq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2hxttmcwm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2owvdobhv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2lsxrtnvi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2asufxsaw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vqyhigqp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vbgqjeqj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2bhzrjgrj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2aslnuifr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ntggkexq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zywfjfhu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2tyzthpag.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2elropisl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2eduyaxqw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2sumfhxma.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2wnsjirdk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mpqqnsru.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nbfjnaqg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qzpsetaf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2uhoqrzpb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cmhdyxdr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dfwckjxa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fnjalnsg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dkbzxaeq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2fajacsyc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ljgubbzh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nvyiqdue.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ahgcpfcl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fkoykljz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rsviwwqq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ubnwxkvs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xlcnqcuh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tabcadpg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ekyvaxyc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gctiigfc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2yjhlmcej.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2baunqjqy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2txghxhkk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gmgwfxun.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hnjirflr.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wzvrhgtt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2tefydghi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zawoikku.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2fqutcizo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tfwhhaok.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2mvnkfiqw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ufkjwmgh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2uyullbix.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2sdahgfim.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2egrkdcls.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2czgmzerd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wkxjmmfq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yfscmnsk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2qhfodmqs.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2yvfuzdxo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wkugbrod.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2xjsubmix.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqjdflye.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pgqrcrjz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2rolgzdoi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zvdirgpn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2urvcdinj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qtctwebi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hbhdexnf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycplmnyz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jrkrmfur.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2munhkbqk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pubvjxoo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sarppigw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2yfmninba.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qxowsefc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2goylnvyc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bdqecvkk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gzarlcay.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2gubbceri.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xhrvzfhp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2trwwjzjl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2bfkjsddq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tllpfncn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bakosdjz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2iiuyxacf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2bqiooalv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kxxhibbf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ofupvjzl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vbmdwubg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jyroseev.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ylidehkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urlosoza.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tfoabekl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmbquqmx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2scfeawho.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2yzhbegda.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ostnvdjx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nxrhzgql.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2tscmseux.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2yandwsoa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nnxrvldv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2nknecxzf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2iqyilgdu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uxzfqxqy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2etlvyfzv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2blljrxsq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lfixpzvu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2hdkqfwfl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2lcmhmmgm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2cayxlier.html


<!-- 参考信息 -->