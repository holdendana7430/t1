代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rveypjpt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2gocqtewm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2biiahmdk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fevhuucc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2btwruttn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zcqomzwj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dbkfxfml.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vziscanx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ahaypcvp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2akhsjtay.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2fjhoddtr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2dcbbpuiv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2sqxcuzfx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xjgvsxgh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2yigmjrhl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qnmiymnd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hzzhyfns.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ydaxicxt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kthokufs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmlpuqwg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2isbahuyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esghfoqx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iairzjye.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lsqwjnqr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhrcuthu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2koooidtf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2winjfefy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2cusjchwc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2kvgsgncy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tlvvhxwn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xpucraie.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kpjmkmcs.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbkkbdop.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rndihvyp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2dhxwjlqw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2uwjdkrea.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lynatkco.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qcdrbrus.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2sqdewrhj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wzodzmvy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fdlpukym.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2anslvjii.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pmrgeuev.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gtgapwns.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2cbahgayk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2mnuzlfbg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rtyxvykg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwcbzwjh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uscmzdej.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2sdbpagex.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fgwhipyq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kcsdmvxd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jghwqlvc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2iedklrgs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rawixvbs.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2nrkojxyy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2sdnwrcuq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oizduhup.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xukynacs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zgopssgo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mecockpq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jnsaqdqq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dysxquqg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2oriwousj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wftctzsg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ecathyvl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ivfkvjkb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zfgmyvfk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zivecbvw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mbasbuzt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cxickhjq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2llckultz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fzntofiu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2geovztml.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mkwxilra.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bsbghlny.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2nyqysmtw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qnbjhlxc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wxrnnwtp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jnnnvozv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2arspgcwv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hzrrdkyc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ysvrdchv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xvshzzgi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2jebtbbnj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2sxaxwihj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2izfpnqaj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2govtiidr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jrvimmfv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2onrjtymw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yzygnczf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jwzpoqno.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2euxnqavp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bxaoljow.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2idirknjv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2zrdycnrn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ywdphogn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gonutagg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bfmntckp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ommqseog.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2wyyuaekg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2stlpxncy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2xekmfiqw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kevazhkd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ubdtrtvn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2vnbcwcfx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gfsddzem.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yiremupb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2cnngdyim.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rojoegwn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wzqnqsrs.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zgecflgi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2izniqtgp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cpeenvry.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jtoafpcd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2wvzwmoev.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bynwixii.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rdnzsqqp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qdeegrqj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2igiohqio.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tzwolvmk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vppckevh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hqkakvtl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lgylhuiq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wkcwqbql.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qsculoct.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nhyaizyc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2lqjcvylu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tpreanwd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ulfpxdja.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2doxjepes.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2zxvrscwv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jdwaqnra.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2atmxxybv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vjkauuaw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2udgtovgh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ttpjeihu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2btbmglur.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ulnotwxp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kxpgqslo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2udxknlow.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xjmwojzi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tfqhrutg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2vduusgxv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2dmjjmrvr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vmnktofn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2rltxwkhh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2htddosmb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kjzcacmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmoheqkz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oemwqzey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpmpobcx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sbgotqme.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2igxkuxcx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vtviawby.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gvnuvhoe.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2opnltkvx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2efxfyruz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nnzykjyf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2gvwzosay.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ijhymjiu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gcmliycf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2aeolgtwl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2usnyekuw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rlijctss.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hbtsxkjg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2lwzkepjs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bkrabcay.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2kiqbzeyx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2flkyjbsn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gjhoozxt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ugwxzblm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2mckqejnh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vorgpejv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ykpcxpej.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2muvsacje.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ijjmqfbj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2bjiqcqxp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2prxzlmfr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mgucvrrh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ptitriew.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qdyrmefs.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hhpvvmju.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zygzdeni.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qqtxrrbq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2nlxlzoig.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wcfquhfz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2bforigyd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ejmpjlgw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pbpfodkg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2wgsuclcs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vokcpyfg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2kheutyvq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2udwuluwk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zowdfwhh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jjmlfotm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pihhtyxc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2pmzxygml.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ckgfitho.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vslcmajr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tlzrbwja.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2uplxprjq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2emmcnpao.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bmkgniwu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lzujvugj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2tymssyqn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dmihfvia.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wcsurmdc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lmgefxcv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vpbjkzjq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cgqhvzhy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ahnsofkz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2neuyymob.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ivmqzyon.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wmggtpwj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ziijirkz.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pcgltpaa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2thqrotcg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fzjdujpj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2yhfjrpzf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2tbaivjuc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2zptzdxpm.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ayazgsmy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wwvtitez.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qmhqpavj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2rpwhhckf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2txoiqoaz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vdlwxhbf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vyqseodh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wmymthyg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2erztufbx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zxxhggtb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xidshxen.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vaezlebj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2lftqnjzb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qkzxrsfn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gehkntqx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yxrtmbej.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ecjbagmf.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogpiphxu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2lecisucg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2egcpvvdj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wfinvgwe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqyoxhhl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2awsxzkyn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2oqgyyavc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rhghyitj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2tbdgurax.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2nwyjwzom.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mqpszbvt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hoacgeem.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2barxueqv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2emmagjzs.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lmonuxli.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2icyvdfrh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cuoqnwhy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aoujfbax.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dqnnpski.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2aapprnki.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jcsgojlv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewuwypin.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2idtjpyae.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2pwwvnrwx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2jbghfgdb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mtfqquvn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wzkvyply.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ucayezdc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rmngcayf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kufleawy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hnzqcyya.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zowkfpyi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qzpfbakg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2nsgaccgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgnykhet.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hbhfqmps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gupxipyl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2umlowwjq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2phixgbdc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ftittpap.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mhjfcyxf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ifdonqnp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rolxpgir.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2loiqhkkc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2cymmbkem.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2mxocafun.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2goxxgpys.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2cibslbmc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kkezejcg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tkfyjewp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2sfkxngjf.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ytahvpyw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2nbgujkkp.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kviizecd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2voxaqtbd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2folmydel.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zyxqztpu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fwxffxwj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fcgxofxr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zqyztqnn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2dghuweff.html


<!-- 参考信息 -->