代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2txcdfjdp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qrpgabyy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bjtiyaid.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2fmoezgbq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nfcljfqx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dhgwjxlr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2hjsnbbfb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2fzgcfpjr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ddemgozj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2opfqtwha.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bhmqtpya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hosjyxxc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2htuwgosx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unihfybn.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2timhcmfp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jrvmnuom.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2lkhhcltn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rdwurqrd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fviyojir.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2scxdfnih.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2tsbeochc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qltlhkzf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xhjriprk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kahawzkb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ufkldmmg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rrfhpvfb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kbotoypx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qrwjeapf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ulayeugk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2aehlmezh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ixwfifbz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kxozdtnj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ugjuqfph.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hhbqpymz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rvxfjtpo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vniwdjxv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ywoivaxx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2otsngtar.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wmxqgkwh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2uomkexnl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lvhphbou.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vdffvmkz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xwyfuvoi.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gjuakoin.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jtmmdqaf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tjtvuxzm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2wblvpvru.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ewdrgfco.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hzqlumtb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nphbfitm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qgevqnso.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wjlkihru.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2orhuazbn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2mqimtsyu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gqyfwvwk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vobsmhdp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hydycfpf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2bxxalslb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2kwiivxum.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wbevcptw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cfgrdfob.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2drmiqyap.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ixznmzcn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vvveyhyr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2bsrbvdsw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sjioyqpu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mhcqrafq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2tcdhcjcx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lfjhpfrs.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2xfvzxplz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ynpkjotv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2blyudyjv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ghacrxmi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fuyawrgw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2czzwrfgy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2lubrifbu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2mvczqyft.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2elheozeo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2snyrscso.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2goqtrjox.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2kppvqunl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gosydmju.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fkplamqk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2afkyolpl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2rfvbermd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2qfsrmrzw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ukipatdd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfsbjcth.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gvztgsll.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mrdiehsr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2kpbvlntg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2abcdkxuq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fqbmscyz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aqvfipgq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2royslmmo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cehobtwf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cohwggwd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nvjrdwve.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2jshkknzk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xrtnyhyy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zkfwsiww.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pmazosdm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2zlktylwe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xhuocdmk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2tcjanfse.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2sylgxlrh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2iowpiqpx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ezlmmjez.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kvfitdrz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gpceoqft.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2icftfldj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2onjfmsvh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ivvrkerm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvvgfrmz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lqrlpbke.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2lwoqxgbj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ggecxsvq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2guafusvh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xtwcvraz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2hkilfyji.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wibgnnsw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kyhjzcle.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ejvzumzh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rbgqkycx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ahbyizjb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2eimrmnoe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2sknksrwb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ypgghtok.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xwblgmgl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2orubonmn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ynazkhpa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2kbpszrfi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2unlclvkk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2sylnzclc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2icfdjvcs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sradbsrc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nkinmlfn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2kdbekqsd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fvxhfons.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zhlkyzeg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2thyjeltm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtganjdm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ycuatwho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clymzssr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gmqgzkjx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rlijtagz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qmhhylha.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2jqzmzpwi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2frptspgc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2eunlqlml.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2prmqqprd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2dcnoheax.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2otwbkggg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ngreoflq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2byndpznl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2azqwrykn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2euliaznp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yuflwemn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ojrsuoux.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2biolmlkg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2cysayeow.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2rdxbdcoo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sluguojg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2tesleiai.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2crajfqgw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ukgmqqnq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2mdkbobgu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhijxlkd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qkxmairg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qtgymvxh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2diwvwlhm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2udktjxzk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zabkfgam.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uinbviqv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iqxfpmlq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qwofswes.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qbipbugx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lttxknvz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2plabglyn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ftlbavvc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mpyikaon.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rzfifflh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ktxoukoj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2zynuulyd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2rcswgflv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hhkkxqzz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2qmjkrnnt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dqdklonx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2dbutkdyd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2aephmopo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2uuvtouzh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2odhaczhq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2mzmtgzqg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xknefehm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2deqkzamr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rthyarcd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vjgfmjde.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2lqieshod.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zprylrus.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qhwphjcz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jkziizuf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2boopzyix.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2crkgffot.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lrhmbtgd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wrqttwnz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ioqgfxcf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ocwdzzbw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2chdqaldv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zqsctadd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2gpcvzcbc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qqxbtvad.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2lwjsxqhl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2mdqmyxej.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lxpjvaiv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vfjvmkxq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bgnnlcjb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2llzekyok.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ljsmmluo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2djrkkbwo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ebosrrnv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ulzbokjc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xrhsmcqk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ycfybyhh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2jvmjsnff.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qonvbnzk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vszyoxln.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hknitwrz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2khwhzooj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aoxwpwyq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2swbseykz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2krsjvhjl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2tblvmejz.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fiolvyup.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpguifoi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vauchuvf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivynbskx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2dbjyyffe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmjqcwjy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vbfzwuej.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2drqxkvni.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2etmyjboz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ergqblkq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vcrprffy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2sxmoftof.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2qemgaxym.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ngltlaez.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iqoldsqq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tajsowtr.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2msphmuqb.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xvxvfviy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2atraqzsf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2aoupreza.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2cogftfjn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2kwdfiuwb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ygwpwkhm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nplwofmo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jcjdwdmy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sjbyrzum.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zqpfovqc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2jttgilfp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ivfybuch.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2grffkfpi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ikkkbiet.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mlqtvlom.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2eavksgmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwlfhhvi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uedbxwok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2serfawll.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2rbrdwiyn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2quthldek.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bqfuhrlj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2apvaqvpx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2owctqdkd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2urdyqtio.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2hanfmnsu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2pcxivukr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2jtkllmct.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cijctoxp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2eaihgbpp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2cuvvzirx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pjqtlyww.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2idfwrdph.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2sfbmmvio.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2updpbrlk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vcvljalf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ctyixxuz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2itubpfsf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2mqnhmxzs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ckzbccvm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2frdbgbcd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ibfaegew.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2sroumywc.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2qzfmwalq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ucxtpfpn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2fbvqnbnk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tpcpcvoi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2gwqtxegw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ngvfjwvh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2nttwftjs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2qaqgyfdq.html


<!-- 参考信息 -->