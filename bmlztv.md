代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xagobhnj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2atkhweix.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2szkqhtav.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pmsnzsmu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yraxbgwf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2imzrihfh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xmpciyhn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2uivijpwq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2bcdcnshs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2mkgtdofe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2zwysqacp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ddwaqica.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2mbxhqvoy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2avipbznb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rvlnssph.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cwdsdgvs.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2gnjivytr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dmzynkxo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2asztarzg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2cfhtplfb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sdgdnnhw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fbhvlkgu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2gcnacsee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvgmuzay.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ggtiouac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvaubwtp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pdsaooxt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2fcsdhmyp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtknzdlm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2cjcdarwk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2uixgrqzl.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xjkyqibf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2eojgyrqj.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ixbchgdk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2elgjoohl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gesoludd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dfttvadr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2crjsjgit.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hhxhamfx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ufzrrnzd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hqozonem.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2welamjie.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ducnozqn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wvwfxyzs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2clucyuuj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2tdwaioqm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2poorzsqm.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfpdnnyd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ecgiqujx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2klsggaxa.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dbkdnnyr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2daebcyiz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bgejirny.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ebexdsop.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2tmokmklo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vhlmtwal.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zxaydwwp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2clhcitte.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vskazhuq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uubjhovw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mosfryga.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tkitooxl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2fjyqhpic.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nlwnorio.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hscpdqoz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2kdluunmb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ygkbctgi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2gfkkbrlv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ijgmlvpk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2onccjdss.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2sxfmwuuk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dovhsiru.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qewmrapx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hxhsorxa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ptvdrxzg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2axrkqxev.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jbnehfzs.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2htzzeiue.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2oytpuntb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2erxthngp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xbsohkve.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2lzbxoiyz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hmpoxrfk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2pdpqkeag.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zqfngvoq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2svsgyjqj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fvrcioxo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2cqixsjna.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2loffnvyu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rlcietjw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dmgpaksw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jzvyjltx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wewipoer.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2qjtthxvp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2cxwocgjx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hfgjnbud.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2apthmuqm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qqfvodqr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ebfvzpkv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mugebakp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2iibpwuxw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mhsiecvq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yvdmzccy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hofetvzp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rzncivde.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gvuycsro.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gxqeqsqo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tqruneth.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zcxfmbsx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rhschmqz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2lduhnwyg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2lwenxceb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vhdyogvk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xuftbotn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2izszgetr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tzfprmxy.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ewvgdkha.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wceuyiac.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2uypnhbxz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2yofgbrfg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2rahupjti.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2tdqkcblq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2kqejfkup.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ujfaaeqw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xmhnxibq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2khrqyonp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kxzcywvq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gkxzdzdm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cjkuqnto.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rlnqraor.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rrljoqci.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2amfmeyvo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cflxjbkw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gnhmmmsx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2qndmfuem.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xnyrqxcu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2raudcook.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2trrbuokz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2vzuebwhi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2mrjfgzhv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ebykznjo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lzsdczed.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fcnzwwze.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2yapyaecr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2vdmdvkuy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ujruovkb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qihqlakt.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2cfqwuxbl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wbogdadv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mbtrocht.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2jwyootzg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2adqeppfc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rwbnvrpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgnrltmk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mflmxhhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eapxtwix.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zwjqnnjl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ncegnxva.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wgfjxzwz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gbatfefi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2catlxtqw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qkxwbwbz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2zqcfkpbl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2pzwqyayt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2bawjudao.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ktqmqosg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rvntggge.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cyqxauct.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sfskflmp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hqazmhzm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rylnfhzz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gxmhvhtu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ffmxkpuz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bkzypxem.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2peblrhfm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2uyhtghyg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2mawibdpk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qksfnhgp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2zpaufmyk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gfftueth.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xvrwtsgy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2vcfdicvq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2plvkrgsl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mhlhyfbj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2uwvatyef.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2oxhfxtmu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rkcmgyle.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ozyebvwg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2dibldylg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2fxbaoias.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wxqkdrrz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2zzfotobn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2rdhqxtbw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hlnhqfmm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2enwsnreq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2oejkbyeg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2avymiwpr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2naqxgojw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2tnpbzfms.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zqkztmxf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikrpizji.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lrnvlzvv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zzmnhdxn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xmoudirj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2dakawgob.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2txheevyi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2frzahrfe.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lifvixde.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vszbinrh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2minlnhmb.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vbwnsmfx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2plvnylik.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2jcurmyho.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lwrdinhl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2nlwmtaex.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ttiqfvea.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xhhykcvx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kswytjxj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gzbrkftx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zdeeuovb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cdlgrmqc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pzhtgawv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2gulhuwpl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2tnbodxrl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2czumdyzs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2amwegdss.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fivzgwkc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2iijoyrvl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pwcqxnyo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dzzdudxn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2pxukujlg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ttijphnm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bzubepfq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2giwlcmsw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2sirzvona.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2wydtqjir.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gsismoqm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2fyfekvue.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2odxgvcxg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lrqsexai.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2swybzdjv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2butpgqzv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ucakjwnk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwxunmdb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gfiwmvjt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgvwpsmf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2rhibvgin.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ltdlpcnh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2lianazdd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fggridig.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2iajanxjc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2eankpvgr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2nyrfxhds.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2evezdexv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cllasjkp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rehkbrqp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2thiumnqv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2laeffmih.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tbtgycvy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xbbazsri.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wcdrnzyw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fwcyopub.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ohabpbsz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ukvubgim.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2aeiwlzet.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ujetjshz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hfqsjvts.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rhjumuyf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sqbqugxd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2monghriu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fnduxjiy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2kiveffqd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uydpvpaw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2nbxthvgi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hfpkmwxm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tjgmlxst.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2uvtvegia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvferqew.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oohilvex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmlvqxii.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2nibcsdja.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2caxalmgu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2vfpzthww.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ktloasfu.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2awtfdane.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2dnbsgwfn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hnqsuxhh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2axrneljx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ifuyjsxh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mwzuhqiv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dvwuzzyw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2wqmiytef.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2vbcfvfvw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2uqvjdezj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2purmktye.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2sfhsqqxs.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zjiobjfe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2owigfljf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2amscxhjb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tacuwixi.html


<!-- 参考信息 -->