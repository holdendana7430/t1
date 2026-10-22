代发 wailian999

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ezgpxfmx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2kmpfelwc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xwzrxnee.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2cemxesop.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2uqekgcuf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2atlwphne.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xgqvvvoy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2phhijnfz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ybyuinwd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2muskpdbi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wmknkouu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ksfzkvks.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xkynxrgg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ioqkntss.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2llypoawi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bvmcaiut.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2csovuuan.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbrwyuwh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nrxtomex.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2lpkgzhrk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2cdqdeksj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2wfhflnid.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dyplssdd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2wrndzpli.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2bfrxmfuq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2dwkfbpay.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2otiawmzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axwtmnhz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xlghokxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efjgomno.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oszfzaom.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tyziolny.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hmcsnnpa.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2suokxnow.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wotfqvlk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2abexldii.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vyklijgw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mrsjbdjy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2islrrckz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2diuolbhx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2orscxakm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ozvuexkq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2nxzcxyrr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2kumlvrkv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pywbvhab.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bzwmgezr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2osgmaotu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ajzwdcsf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2pxlrizvg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2xsbujfqc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rhydaand.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehgtitob.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2etfqguth.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2bwnkgnbz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fybtfjuf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2edfwdaha.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jmbgmhog.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jwiumdws.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zsnjcszs.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xpwydxqm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qrgbpepa.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lzvyogwz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2crpvavss.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2srevxxcj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bkbpghoh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ijdhgqfq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2huragcbl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2raubuuyy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2btjgaszn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ttflcvyk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vizpkivq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2dtegiixz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2otgwydzh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cebyopeh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ftzyapho.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ynqfmvbu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2khyyjgkg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2sleeksoy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tkrkuuiu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ikmjrrkv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2arzncmdq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yajjzpgn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2itbfemlk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2bskonkdb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lfzhpuvv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mhxovqyq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lahgschf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qazxiiul.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2skrxeezl.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lrfdhmlm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dtsbxdlp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2dutomtgs.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2siyjlgip.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2tvnrkbid.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rrmpheod.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2shaxpevl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2uuiebzed.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pswyldqa.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2kqwojaar.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2xfmragrc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2edhskdwn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uvkkxnom.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2konehtjz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lqaeqstf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2dbougjgr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tfldbjee.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2jlhdkwvj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2izkdkhvn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2eabvqdah.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xhdphtwm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zzcdielp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wdmewlen.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pifikvbj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2muhaiqln.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2zjsjfpym.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2mlsdtlpp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2sihgdsdv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mxkoxruy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rztytqmh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zuxiwryy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2yosgjjtq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bfxnzswx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2euhydcsa.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2musehtpl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2lbduwgct.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2vrtayxxq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xdhgpzdq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2xpwkyggx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2bqdctiyr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ugkrskvt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2skdkiowh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jlykersw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2dozzuabi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2yhtwkolr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2qvtxajce.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bslghohg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tixgnzko.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2upsxwdrz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2amvqcpqn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2sixokoka.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gcfkudda.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bmopeanx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2snvevyhm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2spvrbfst.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2bmvfpznj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zbrapyku.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2rjfrgzxe.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2wndjmmut.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2prxxrjmt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jrlcqutv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2okztflbb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rglcotox.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pdpquked.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rhpfdmbr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2tbawfzst.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2odllqmbi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2baecfiir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfkcndqo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vbctdlas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2huzdofoh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rhbgmcah.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bnxhjxax.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zuptdick.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hcdsiucj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jsvdusbr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rgtxksal.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2fjlgrcsk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2grkwtplk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2akfaklie.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2molnbzbi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2iwvjgxzm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fzrzcgxt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ffcmiehq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2alcsgnjb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bshurasa.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yyabvyzb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2anbjhldq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xtxxboal.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xojtumzn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mareptet.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2plqkynqy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dizryjlf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vtsmweci.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tntxthlr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ocpskvhz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2awndhycq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gotdxnfx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ksanybca.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zegpcrmx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nfggekhk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ymxehqgj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nowrbcnd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lxjcezsz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2dwxywzbg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xhmepojr.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2odchckin.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2whvazlvt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2znrdpwkv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ibfzyzoj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2aewbmylu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2acfpdexb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2cihwfblf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ydanwgxh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2wthzpdco.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmskcoor.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zmwblekj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gjyvrmcs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zysckvyu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2vxeafylg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2kwfrmesi.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2vbgirnil.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zwadlyck.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dcjgufhw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xjedsgvx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dfpgxutz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2rejhwwja.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2igelylxt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fvtjtsew.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ukedsspk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ddxazech.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2frrligmo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cvlfigwx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2orcbdoqm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wayumnqv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2llpqmjrb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2fixujjbq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ebupbpqt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rfhswnpl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2wguhxbdj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2kamazpkh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lcsecwfo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bdamitug.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zhbqbvfc.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2kscbjpjq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ewufghmz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rehhimzk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rvignsww.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2goqkdhqz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vskzfxcr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ezzrgagn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xzuzyuwh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pifspogk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ebyrhodm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vzlrycsr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cgicaamn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ipnzlnnk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2uwxgxhzd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmtburvo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iavgvium.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2jmvgfrqd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2rgbmzwks.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebibadzh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wcnbknug.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynjwuvxu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2xfjugpqu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2vkiivguf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bnywypin.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qxirxaqk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xbgdjbzy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2lcdtmffv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2htjwnzia.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2egabzgpl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nfupfxvh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fofnnrzl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2hrqdscfj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mrgdikdd.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pnxckbvd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2frjqfqun.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2xpqumrrp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bflexgbu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqinheg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2fehzcxvq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vnasorvn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qfewwasc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wudtwkre.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xivqcgwb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2oeltenwy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2cprlbspv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ihwnbrwg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2edasrzuf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2kxatkhou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trgmcgiv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2voapkyia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuhgqaxy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2salxryhn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ydseqvaa.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2rpazbudj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2irjlunnc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2axrsvtvi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2awpuakly.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xthwobax.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ntiaryof.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ibtunamr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rmgkihmg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2vwhqxihw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2urkotqaw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2reosuqnv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ozsqizmv.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2zilanjms.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ydduujiw.html


<!-- 参考信息 -->