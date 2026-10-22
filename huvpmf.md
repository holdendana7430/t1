代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2huyuapnq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2fzniipwz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kyhertte.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sgumkvfs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2yxyqhaqm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2bzdhqbsd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2uhktgtec.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dotrairp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zsnkignk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dsjnyphz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fmsvmoim.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2aibrodja.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tgcpqerj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2apcccouy.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ujweluxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjvfjdbj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2efasghox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npkqlnjh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2elehewyu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2eogdkkoh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bkhhwikr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rolwyvse.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2jadzyxyp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xrybbwfd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vuxxtdpj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2rgzuanly.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gbnymchy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xdwxnjfs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ydrllqfy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cnezazsg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ivgvrlrg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lhjzifhg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fyzfcnln.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2poxjdxoz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lnbnffrq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mucbooix.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2elatmaqx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ercqpiry.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cwgovgkh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qvlvjilk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2iyfqdbfa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ridyhfez.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wilqbafw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2dwnomqxm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rhtwtoar.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kytvlhcu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vgspompd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bsfyfxzh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2oqcjxexp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2klmrrfun.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2uqbzwpmy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2frzmcqbl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xlrrluwu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ywwextaz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dzexqens.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gycbdyxn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2julhcpqy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2sshjsoef.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nwlftvgd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2gbkerhep.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ybyhiepz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zvjqrakx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ecfsdisw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hqvbkrpp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kwqbweuk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mfyinryd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ennzomgg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2taupajxg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2azuwzdik.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gekndwzc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ljeyvtsp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2allhqmjx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2nuvhxxdx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hkxooulc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2otwibmia.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2uioprjbm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2xtkowaje.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2xnnfjhor.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bwyeacfj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2zwfshsnf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kcbdnnae.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2unnozxrw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xmlwyzhs.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2brwvzemk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2btxibinw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtrunfpx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vsrgymai.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ffcfldhp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qafggtmw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2wwgyndai.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sxzavsul.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeeuxmry.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2hgnovipq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2isqygedm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2swjhcsep.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mfbfqxra.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qczdpxps.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vafrxlsf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2rwqikayi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2elqtdvrx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2foyxxyjl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2auioeist.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2yuoypcmf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lmisenua.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2neyuspbv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2lboswbtz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2foljxtpw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hvvpwumj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gjfalynz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ohmenxpt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2aujhcagk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2kazbpkyv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zbymltmv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2larcmkbf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2myifyjrf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2emaflvug.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wozjkzdw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gujygnve.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rsksazvt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tchijjta.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2snixxbsl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mvegyecr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hbfojcsk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hbvzzxzn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aceevuoz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2hunrykny.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tjlqvffw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2kcuekspg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpseeess.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2djcbnxjy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lgbiudhf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2rztwielj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2uesgwgbx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tdwzjren.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qdvdypsx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2hjqytkfk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ungkkrdd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2yioztnhc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oxilldbv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vxrolopv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xsrpjmrx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2bpvmyvow.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mbhrnnda.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mywdojyh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cwkplsjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwpkrbul.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2aezvhhsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfprghxq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mfyoazbi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2emlskzej.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lgzpfwah.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2yqifdbgh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2chgrclji.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2cewpuowp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2uwqvxkhw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2tvistesu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2fysicdev.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qvbnodfw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zutgbxkv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bgbizvpg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2exclhcud.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mxeayarv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hmuxeuea.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fxjzipbn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2grfenjpm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yvzmamto.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2bkkctmsa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2znoghvst.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zgxzbnul.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kgvnwpim.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2kzswrmen.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pceuuuib.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uimqfuhj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xialtffw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2obyitize.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ikssunvu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2kakupngo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2upbhzfzt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mcnrkmhy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ppugucst.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rxzrqyfz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2clafbmix.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kruikklw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2gvctkwqp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2rkmwuyzb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2hbecjvke.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2jodexulr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2sekdvzta.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2sxthiurf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2wcmapont.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ryeukpzm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qemupkoi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2physkoyl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ejnssuoc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2wstdwhlh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bwysubxd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2zhmycmam.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2fwcgohde.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2obvskfcm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2oxrnetxc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lngiwlpo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2zcdytgwy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2syewvmew.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dofgbmpm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2iqtdevbs.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2sycfztbn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vqjoxifo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hkudvugj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jgugcqpf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2usyjdcmu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ttfmeiry.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vwflpxkc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mfpsmiqr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dkbtbgsl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gqolgoqp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2zmeledsn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2duyehdbj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mqpczhuo.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2wblpqdkl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2jltvkdrh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vmxalhll.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2uahxxqua.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fspwgzcv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2lypigvlk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nrrmedbw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2befltior.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vabgayvv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kapzulpv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2subqkmut.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mskrokzt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ufxygdnm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dnisavgm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ufdtfnet.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2gcxqluvl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2dziqfoae.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2kkrinvmk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oipeqcfj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2btqbyizx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ockytkda.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghdxxthh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gjjbhiqe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2plrfcouy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2dtrnbfve.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2krdndafw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2sjwhisqc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueevynxi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tomljhlz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2nmebocpf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gqrfaeqb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dnsiavrn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wzugiyvr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vwjdjesg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gbjpzxdl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dsfydtbj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ykpxhgiu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tfjrkdew.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2sbhoefce.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zyqcpjdf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2wegprzwo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nrbqdnrp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tgbsnyeu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2szvtlkkn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2tydffihz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2vwinxtfd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2krxhazcv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2lsukbhkc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wyrfrywj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ahrkyuyq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2omboqfvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjchfcfw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zgbnwvow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onrlwxuw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2wrpsvyfh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2lvjjfqqy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xcgeamhh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ydsttnkw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2havhwete.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2qyxqenkw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2cavdsxld.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wcvhkaqi.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qckzeqbd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ykrtrhuf.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rfqprnic.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2bekbzmll.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2bavfguma.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2kcfshmtz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2tsxmitla.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jozoksbv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2utfjyznh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bifxaedo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ozjthusm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2dkqihaza.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zbvakjgn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2epjhcewj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2eykbwddk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2nksrnnbb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2vgxtmtde.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2kwrfuaqc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2qitkunxv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2awruxflq.html


<!-- 参考信息 -->