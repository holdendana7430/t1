代发 wailian999

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xuarwpdx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3uumvmgph.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xjiwceaa.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3bhziflvk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3owcfgdzh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3kaeppnat.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3tvdfaghc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmgycfli.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rcpvppyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hphjeqzq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uamaotzp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ampbhood.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3mdizqbqc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zqcqurna.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3kxbljzve.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qelywxej.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lnefdnpt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3mjxextng.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3juxocvxp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ctwolrru.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wizcnfvc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lnemhrpw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3avfbgxes.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lzvfrsvk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3awyjbshy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3yczcsxdi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3mbkfenux.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3sjxzvlqw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3kckxnxeg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ltrfmglj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pjtujxqk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qcovzpag.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3nhtnnxwn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fmupcuxr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zvmtqlso.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3deymrqyy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mlsljemp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hmhebfiw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3yyhnspws.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3xukilowu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jloilahd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3rzjiceoq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ihaofcow.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qotnxrsv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3puwknjir.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cgsqewxy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3oogscyav.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ezdnpwoa.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3fusiwaep.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3mamchvrl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yfcxnlnt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lkvxbkdk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rtwwmkhr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ktbnhcky.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rizbdawq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tlxngikn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3pjdauzwy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xvqbnlch.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kyyeqkbj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3uxkofgal.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zlylwnmc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jenwkhly.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3vvdtqsje.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kfwdzuix.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3zttrkpxe.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fjaqfbbc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tdvjrrbo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zpbxiuuh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zjuvdejm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3chznobsy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ogsclneo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3yeyaqowy.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lgeludia.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3rwrocciz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3vqzfnvyu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3numkhhwz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ptwusxjy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpmzfdyn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cgfpdkyj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3gegbngij.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3osokjgmz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ftmjoumh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3baqpelfq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3svztxvxs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3tzbmcmhz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3htiervzx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3gnnymlzb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vdhppeuv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tyvjdruk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3okagmpiu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3uocyfgql.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fauufkrg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3nvolnlun.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3tvzzolvl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hgzfnzmd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mdcfzrkm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ntquyhpk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3lfsfwymg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vacpaser.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dlpikgja.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3shlzadhy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nvwwuybr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ussdrvtk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdpiyvdk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3wmbreunl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3kjqbvcck.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vdgdxkge.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gpbwcipb.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3lhioxabf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjgwqxye.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3asdwbcdn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ncezxlei.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ohatrwxz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzgrlafb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3rxutrsjg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3trqdqffc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3psdddvgg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ifdazmux.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kxfhmvxl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wgpfpypd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3egkrpskf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vrhpdpdx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3oquonbme.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3joqrojmu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3rxunkmbs.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kamavghe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wlyauipp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3vjiufbuw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mimkynbm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jusrjzgc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lgupfjsr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3oylmwtou.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3irnpmxpl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3oefyuadw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3orkhltcc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3mkbdcskh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xvlacxlt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcvyuafu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lubtbkgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qimoaqvx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hsxlafss.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mftpjjva.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vgqwdhzv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yfwapsjg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3kbyrkqzq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ioqilevg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3woojtmrq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3cxjfqlwb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3etlhdsod.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3avguoemw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ezeuvdrz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qdoakwna.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zlbdtqaz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3utluwbok.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ufbfrnyd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ndmibjct.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwfqxyvu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3uyifisjj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3dtmojbaf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ycntvagp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3rhcnqlld.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3rxgcjayx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dgamosah.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3crdgmpfd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uuoeavbd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkaiiopf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3diavynfy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vamiqsee.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3hmkizriz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qcnrisij.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3moiewrat.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qajtffel.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3cwjzwohm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3sojzkluw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kqoilrba.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ibvpyqda.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3renmbbny.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3inpqmlpz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ufbbgkfk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gqxikkow.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3pflduayt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3sxwpirjw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3tjtokpyn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3awfjrjtu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3dfnmipzh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zxpcmjtj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3wrxmsgnz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nlmldnwe.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hgrcatxx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3uyfdsbhu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ocrpjymc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ftvjkkgk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kxdcjguz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3tybbfore.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qvfcltka.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kukgnaar.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ljahtjnk.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xaclsajd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zmmxwytq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dvquzyaw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lgccerdz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qeippjry.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3auiuoafi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nakkstqp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pzvouljo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3zkplburf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kcqkkccf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3badglqup.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3nmshxipq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rrhwlebq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3webcctep.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3gwxnffkt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xdjenwyw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3clzpksrq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pcpqjfne.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3fnidmbda.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dknlobfo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3xptaddwa.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dxzmdrxr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3spzynpqq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ohksejjx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dmwtuwva.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cjgjrkxx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oabxldcv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3majxxzcl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3cjmohxiu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3knidibrm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vyjarfbr.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3tytzugyx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmbxwsif.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ketnmavq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgjjwhsa.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3bxaejoyx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3gwbshhnj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ngtdpslb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mjmzxyfh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3zbydqyzv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhyovfso.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kseioynd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rgpzvzya.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmcwluay.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pdctljvs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3scizczch.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3spxgbkrl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kwcasmrb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uljbpcpl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pwwrvrrg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fxlbjegz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qndmfsgu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vqkdlrit.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ssdfjhej.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3dlhphhno.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jdynfqgb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vqsejrfn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nkitlbpl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3cftnnaqa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qrcgtcgr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lhxsuywr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dakdrsau.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3huqzrivn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hoezmbuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnzibmvq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3agaxetws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytsjhdhn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3dlcazzwb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3uxwiezej.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wlokqiqi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mmadplbl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ztnizvnn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3jjuqlwdn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3aoyekpkk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jkgyywnd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3hkwttoqe.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3herlszdq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3obkypspx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3aymbpqjd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3fylgnltw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qtxrwwbh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mhvtdexa.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3cbrfeoiy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ptwfknop.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kkonjdgs.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3xvrfgfsr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3alzmyxyo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oziakpyx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3knjimzth.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qksovevq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3nevenxom.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hwahwgkh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ijkqqhuq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zpmxrrvs.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fyvzkmwz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ibbocvzq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ufuwrdxn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3pujreslc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3kjzcvhrs.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fpkwwkui.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3yfcjlprm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ksrqaaug.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wvrduwqb.html


<!-- 参考信息 -->