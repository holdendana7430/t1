代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2afoyyhoc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvexyoou.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nrfxaxxs.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kbwmjhlu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2dfqjfevj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vbmfhyxe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qcixludj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2kpecofpi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2cikgytji.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2nyahmyah.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hsoapoyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruzsxxaa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2domxsvzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxvxluih.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2itjcxhlv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vhcdlmeb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xwgptjgr.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ozttbcux.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2uxdfsgvc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2oemvjoga.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2bmcisbhw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2coqspszb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hlffimgx.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kkklbsvv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ddpwimfn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ehzvaldj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2eeskmwmb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jnsrntcq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2eanzzqmb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yevmfamw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xcijppdi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2frjkuxdo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zvshpnur.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2wpxfkggb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dyhjrtny.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2abltwsps.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gomwjwhc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2psvzshva.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gnjhpzuq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2qidlaxtr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mhnaolrw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xvuejybn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ldyzpwyl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aekeodfq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2iqdylgxn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2cjqitckw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2zqjigith.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bbogrrvl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2tvfaadka.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lvfkuuuj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zjxzqgfh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qmxsabuk.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2yrzoscop.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2uddmmppk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hjrjobbb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2imvrdewr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pppnmqqm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nbthigbp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hacidiuf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2sqyrgdvb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ejamojoz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hmygaiqk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2tqqryirv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dcjfwvem.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2tlnfyuuo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bbrlooga.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2eimcguoi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zrmffpbi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vkwilbal.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2pdokutxx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mqntfezl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2dttzqzyt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xilcbwep.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bhpqzpnz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2kxlhndti.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2iktnulrm.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2eiusfoja.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eupztlmr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2groptaoq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hhsdhhha.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2fezriosi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2eodjravv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jrndhujc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2nnfsedwt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vpfzsrzr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ekfszrmq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2iitkxotr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ujbmtpbw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2fufnreru.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rotoxwua.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zwdnncaq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qcqedzcw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2afunprci.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jdbotkqz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vexlpwxj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tqiodhhh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bdjfptba.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cbewjsoy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2kctwpbji.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jzozjzjh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yezwdtcg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ryilrurm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2lbbvdbvq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2busvutqn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2gnbfcnfc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2icozdsps.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2iavhxlzt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwvisnpt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2fafyihkr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2aatxglyw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ruzsympg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jupbutsk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ibdwigur.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxpuunis.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ezlfsyll.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2irhhatfe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vdtmnqgd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vxhfksna.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2kplrcajf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2iraauxrg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2npotddhw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2owkhzkmj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nbtylkis.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vvqtamye.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2roaaztpw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ypmexmmf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tftbkesa.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wxtzpkxz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2bcvxuakt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2agmereae.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2qiduzkgx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xknbtkgz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xahwnhxs.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2mtpgkmqr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2trocbhvb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qqgvrjkz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rjchzdjt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qhpdemhc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2dkbjlasq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qqfmokab.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pxlpwflx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhnlbzjd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2cfhaxghz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lebgazdh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ocrivnau.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ahxmuqsy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mygnrkhe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gmzyiohr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2nbzlcwvj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cvftmimr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vrmaiqxx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ktpliodg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2upcbnysn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lqjagrml.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sldvpexb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2omcotqcy.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vvtjfdbr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2cfmadpqh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ffljpher.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2isrycvyj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2drdsljlf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xyotaxlm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2lvtclrxa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jadipnaa.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2imzrzkub.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2yacuglfb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ohcmnkdm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mepzfxas.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ydoytzin.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2oppdsggv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fvmeqdfx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fkgjpzsd.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2keopmuzk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2icmrkfki.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bbqcvija.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zjrknqre.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2szhanjsf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2puzprflu.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ggrqmoho.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jswosoav.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qocrfths.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2gezdfzam.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2hyppczod.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qxehoadk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2txhxxpkd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2vsaslqpr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ffxpxztp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qhyyraux.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2trknwmep.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rnqxddqt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yvnulhio.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2guueuxig.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2zvtocvkx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lcvditiz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pbtpihbu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ylmwatfs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rrpsjibh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kmgwuiuy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lbcwxwwl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wymrmilx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2xfxoozos.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fpxdtztf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vteguqau.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2vdtekrxv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ogmxqedq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fistffmn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zixcxfee.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ojkqufpd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2lztkllaj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2bxyeaiso.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2mykoahnz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ypbmotko.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hinpfzcq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uukwrwrf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2nlammojv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2lgjfmcxj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lwhbjxli.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fxyqbisq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ubdqclrx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gdqwqmhb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vncsmgay.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2dcohdkrk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nfuxwgjd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2hcssgach.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qqoedeji.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bqqdskvb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2xvfoqjve.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2lucvpigo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tuwqrefe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2sqnhbcdc.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2bepuvvhe.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rppfkdqs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jttjcvis.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2twntmoot.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2pdqxtlfi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xavlsguv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pkulgdph.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qgrnplfc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2frtvakbz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2jnndtbgq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2gvnpzyva.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wniqzfvr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nvyapqkc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vvktjefd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2iezhexhv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tfisxdmu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bpiqurpm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2disowwjc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pgugtqtm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oekqwwce.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2isxtvcjy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tcjcsmos.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ghdwyfgx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gnulzgsw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2wpkbbokf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2fqjpecla.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dhcrvkxb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jftlcvfw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2owuquyqr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hhhbicyn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bedukhcv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uwraksar.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qvjentpg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ovbntigu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2roswicyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmbkiesm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mvkjqsyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahrgcjsf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2rzkznpvh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2uudoqfol.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2qblgomgi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2dwyyeqxt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2swvopxla.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2pcntnpqa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2bohywihj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rcvtcvpm.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2yufgvtii.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ygzdgnbp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lcgjmlrx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2objokbus.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2xxfpskot.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2fjqlyeda.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2jwvrntgv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2yjcbmajr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kqkpsixv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2sldbtjke.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tarugzrh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2rrbrnqmk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2adsqyzdm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2bhvwvgyb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ayuhnktc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bpybmkft.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2hokombmc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2oqwkpdmo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zajivzli.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2lamvwyst.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2omaslhba.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ortnmfxw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qpoefwwu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2uqpcqjtm.html


<!-- 参考信息 -->