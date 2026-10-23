代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ficvpylm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bvywkmpl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3izvfpyjm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oechyojf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3mpwhrgtp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3fayqtxyb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3irdkcbiw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3choyseyo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fqzoqrup.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jynmxown.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wwxqxjne.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3cgjqefte.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3doiyhele.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fzcjcmzd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3connwvyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3algkkknu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3riizqxlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivikhahg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zlcqwgjc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3lzbsbnab.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbceipyx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wevbfixl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hcbfbvct.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3mwbazrkn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3unsloqhs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ztqdumwj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wobplbno.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3psfvxcgw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3reeehrxu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rhozuubt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3lanyjfuy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ooglbkdp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3igvrlbok.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3xxbmskeu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ulnczsmj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3tchhnzck.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3npmztqdr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vquevyxx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tteijghy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzpvdgba.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wtmhflnj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jyenejni.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kkuboorz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bnqkrsuz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3aikxqndj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dwzbhuzb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tsdoyjho.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dlutwxht.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3iyplovdj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3rxbklund.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ztleqwds.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ksfeapsb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3apfruxmq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vsqzjwid.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nalnywee.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ufummabi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kbqlvwne.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zuyblwmr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3blwaefdm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mznrqofp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qxwaqtcv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ubtlznwa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ntlhqeoy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3skxomyfk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3uucqecma.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bqnqqsop.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3jiysuxkv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zxdkiyyf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3pctyuknw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zfwbying.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3gxnzhsok.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qvseggff.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hswydjld.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3rnwzlcwq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pxuzrdzx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3epdypelj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3rfezjztc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3nfoeipuz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ylkeqvai.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3sioqizfz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qjnabcqx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3drvemqcg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3esrczxfs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rxqstbas.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dzmxpbmn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bxakwayh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ifrffzkx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3nlwqawmq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3wzhbiofr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3dusgadof.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3llaecflt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvlxzxro.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rhzhxuln.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mrlemmrv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3plysxito.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3czvdbpvb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3jqeipvay.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3iivrkbdj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3gaxgcuox.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bgrffdnz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lbgmvkws.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3delzxhfp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ceejwsvk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rikqajwa.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ftevvsas.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3xvqlvmrt.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3dafjetii.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jojfmukq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ehywwwyc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3sozgwoyh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ucobyeio.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3estzcbbe.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vjegkclh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xegebecb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3thsazivd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uttxbopz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3smjmskhk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bidkzgzd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pchxaqyv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xxdoefkh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hadzhrwl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbrizpeo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xbwavoie.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3kmnfevww.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3itagfczy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xflfmqry.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3itavofdy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3kfedfjxp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vorauivy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3muylciuj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xnhffchf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3pbdizlkh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ylurpryg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ojikukfv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ekxmhajd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3pcvfdeug.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlnitbgm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wxemrqpw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lkmlcdvr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3suwwyhqe.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zgnbupxv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3yifyysjp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mtnmwlgm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jgazkxyj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ppeuizfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmsmfftq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dbmzrafd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgzlvmml.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fjqdddjs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pjbhoaph.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jyqgvwea.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ndocnpvm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3fzmsgxqw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xcenjtmd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3sqjsegqi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kogqhgyc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dstywfgu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dvcnbixp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3igcnmrji.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hquqwfsv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3drzsbooy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3oormaenv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3eshculfd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sbcyzqna.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vzfofacd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fdxxnylh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ovricqxb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fmitxchr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3arjwopvl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qyyxeall.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ftankoxo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oymzyiro.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3gspxdgsw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3awpbilxa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3kibbbiii.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wsqnznuk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3wuqcjwiw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3turrwywt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dxsssgbi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fupxvryt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3zbzlucsw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3tojyemug.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3axvsbdav.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3adnzhvjy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3khqieevf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dxnhgolc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hsmgltqz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3yichyjun.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yfhyeiga.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3nsvjyahd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3gblktrcy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3cqboqtac.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3bhezqrxu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3rqmrtydy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3zmxdqxvn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pwqeimjk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zrlrqjix.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ucitgrly.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vslhekye.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ylrtsljd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3siremzdo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zdntdgfj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3emufregi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vnkkabvt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dcoebmkp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kzfrdkme.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vnujhqry.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cfmkgdrw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cwmuwkij.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vawzbovd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hwiacofu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qrzcoevq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vzxcnvck.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3bgplxzfw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3thjzcleb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zkdwnxzs.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3lsbmkufj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ircmcdji.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ffyrsrtg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3awczbjwk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cgnqtcma.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ropimgqq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mgihxdyv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3shouezqr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pqcbpowx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3esnshlqf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3nbptslwb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3sgftefxq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dpcodarr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mnnyhjnq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zlzwvdml.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3klcebtju.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xvigvavl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3cvwlnmky.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3azytrjta.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ibciduoh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3alvhpzjq.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3rwpjmkap.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gqykmzlv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pujdonno.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3pflgormc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kyikdfyd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3srkqerna.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xbzhngsv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dacbqcsp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xwnkhvrx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ivqclbqj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ebdbqgfa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qidjtktj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eiknodbx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rkkbkfmh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3nwlhcbed.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3czvhrbor.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zrginoon.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kabmfdgn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vpcwapuv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3objkqtvj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ypiavtmc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3aliefrca.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qxnleota.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hngfgzpy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3outefcme.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bzlfeywv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xvwwkrlx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3cirsuwew.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dmatjdlv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3thlazvxt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3chldvpqy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3urxnsdyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qiakxofw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sepswqui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlswvfgi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ebduzhqu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3trujgahf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3hwdpygge.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3huabhllx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hukyvcnc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xpcufhqo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dtuvdaqz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3iwowwwmt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yteimrlt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nxvvptov.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3krefnmas.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3bwwcbphj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3opyrilek.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3umyvdjqr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mtyoauto.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3mldvugxz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3kksujuki.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ayyzmbua.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rnfxmptt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dpsopyxz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ulpndsoa.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3surcvxfb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3sgjinagt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ykywpttv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xjxhedtu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qvacigby.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3domnngyo.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vnkexsmr.html


<!-- 参考信息 -->