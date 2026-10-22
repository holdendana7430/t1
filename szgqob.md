代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2eqxhzmav.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dndggfmh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2iyxbxasx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ewpyzoha.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2qxqoephi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2loosqbko.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2wuynuinu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uxygxxhp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2pawwpoba.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxrjzqxa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bnrimcnt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gonypppg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2fyqpfurc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2tjicosdk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2muesciwi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ebsopaiy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rjliqnss.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hapwcsmm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2oeqdtpxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwbiuabo.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bdqyfdan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuhwucbj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ftxxnmvs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2loflobxx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2omemelre.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ilzknwea.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qmpjhqiw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xqkbfasl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ecewikji.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2iiiifoob.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2olifqdbk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ndmppmqv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2iuudiqna.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jrutbuay.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2iljuhcxy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bgaygano.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jzldydkd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2vcbcdqjr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cspqjuum.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2yxhkvpdk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2scapqmif.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ztyskyou.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cuwbqnge.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2deoucgmf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2tztrflyd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xmqbimys.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xdahxqyk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zjiixeey.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2sxnuwpwd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2mtorubrw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xujnmkxy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fkgsxiin.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2lifmrqyg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zhknaqjf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2pabxvzkr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ofjvcpsb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yfdgight.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xxjporso.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2khejftag.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vosmssbx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jwdfbcrn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qzqhyxxu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pzsvndfn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lmjejcqz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2trbdbtcz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cmzjoozf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ojgkvnqw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cktlsraz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tzpzbnqe.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zfgvuwvr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cmzybhkk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ccnjzjdw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2oaxpvoxa.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dkdphets.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2scssxdwi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2pkazztff.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vnitjsfz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2evjeabrn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gdpfkzwk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dtbjgzkq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2otjvkvcx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2byufslgd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2seovvtja.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ujugkpka.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mwtfjhbq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2otfipazr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zfpqsljv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mxyhcwcm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2allhdhtc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mihyltsv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ptmyvtlg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2athgbbio.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2cxirgryv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2gcrrtqvc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2tvceuhoe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mepjimjm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qckozxvp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iaiuwxaw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gndbkcbm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bxsumodp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2juqxjcel.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yhkhqtzu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zttotfqb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qsacsmki.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2sdohkujk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2emvlfsst.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mdodarhu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2sjjvsuom.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2mqhocojr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ywospogx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2cvppqlfc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ehfjmytw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2dntuznaw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2tlucbpod.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gzogeeup.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzxfruge.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2yqmkadvz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2twdajtwr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2wwgeyndj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2yhuucmmv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vcgeqwvp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2euatofgl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gknvoqhr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mjaioirs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ahihqext.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ywxrfuxo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dxjgqlsp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vuctysni.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vrutdtfd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pgmpjqzw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nvmvfrza.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vdnmourk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkvwrwfa.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ixagbdkh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2uvvqeyof.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2asjrpmmx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2dtlaykxe.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ujmlxnui.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xicnwxxq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zsnqpxjx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xqacycbb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2izmoqkin.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2aiiorvck.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2igdwneyn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zuudvjdm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hsvwwnba.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xktxpvag.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2tntxtjrv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yovzsljh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfhklizz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2eoktnvgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oikekyen.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zxfurley.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2juldtepa.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2eyqufvmv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2nltidlnj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2hfiaqyte.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tenowono.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2qhfefsrs.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2qbbxbyjx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ghilhxcm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2bstjyekr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2aspucnvx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xiprduqj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2adxauakj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nlksdrzk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gmaufwqx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2moidfdif.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2psvdoezy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lrbjboya.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2kedqhfdu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2smjfkkug.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2byrpjqej.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nwiooaih.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2dtrjlgir.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dmlauegl.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2nyvaklll.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2teskhein.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jmprvvil.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2namkqvgm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rekkxfay.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qsejkhmm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2reszqsuk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2domwbgvz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qurbqpgf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2juoejyuz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2znnyxumu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2innzyibv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xpoapqay.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bvirqvtq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2siecowyj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2yedesism.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xtqhupqs.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rskeoqev.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jlejwinf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hhglfyvd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2oaaadrud.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xylygine.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2pxgnnvzs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2igbtcbhn.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2deckxvib.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2kmlzpwev.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2fqelnspr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2krhfiwgu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bcrftdbn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2mvygwueb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kblhbvzx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kvwyabyj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hcduhwto.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qekqbntf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bnqexowu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yyfuxlea.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xbzlcwkd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2muryhoin.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pqqyboul.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2nbcwedrx.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ozjpkfkh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2snxlyfkd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gyhbxdnk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2prgfjtja.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2wlvnusuu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ajuiulur.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qzgrawcl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wfchjhdg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vkbfcuwf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fidlfwrg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2orlrfrsy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2eqftkwgc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pzmygsln.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ieeakdxv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mjqlgagx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ppdljgjq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qldqlphr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jreftqku.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2gsgucisw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2rlqvpcel.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fxqxpttf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2icolluqp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ykkvrfvz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2efnbmlez.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kbindygs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekndwfjh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2kmbgtqrw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvzzckpa.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2poaqicis.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2kqoqftup.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zuymlset.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2fjxrcyal.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2uubibkyo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlzbhzzo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yymjzggl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jrdlkxtr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2nzjjmtyf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ghsyhhbf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xhqfgili.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ldjjmfsp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2hrhsakad.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zhlebgqa.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kissryyu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qyrzybkf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ibfkyiaw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vnnnfguu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bcdvmdtc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2anbruere.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zjpwkigr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iucbkfrq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hochdcvt.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2laxnbqrx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2qxcvtcda.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2aqpjnmvd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gyhrxcbk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hluydvon.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2acjnenad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpbvtknp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cpkkmsxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxhghirp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2asxawlfo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ttccajtj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2vkhwxgzf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mtdhfhpv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2otganmej.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2dvdgxxmp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2pzmknwez.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2puqgzjfy.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2eqlcjlgn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2jusucvkv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gnjucjpt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2hqmjtxbz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2diedqqjo.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2pdicbigz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mtpqdbgp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tcgdwlwq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2pjwyolwh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rxfoxkaf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nvdkruft.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2oewibkxz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zfvztpve.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qedpeozz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2muogjqfv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2xipokmfq.html


<!-- 参考信息 -->