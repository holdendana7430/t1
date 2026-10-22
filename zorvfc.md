代发 wailian999

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2yxzmiins.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2pqdzelgy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ugigaanz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qhvcixes.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ibwrifch.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2vbuzdize.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2eezjjbjr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2fjkwgjnf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2naizruyr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2swoqdffi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qzvooiuh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2brbbsshc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wrytadcq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2srzgtqoc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zrxsdzlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddokcjyy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hbesjtul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tudqahso.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gbmbyusd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vxttdinc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2alxkgqkx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xecajlof.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2edhporif.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2oirgrhro.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2jjzrezzp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2qhitedln.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2idqwawrj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fgsfwdin.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xrznnvmf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ckkjijgn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2yvhftytj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2stahjehz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2vcdvmczz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fcdibdsb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2kbozzgvk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kefjzqun.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qnhwbluu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qmpkzzym.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2fkrudmij.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2etapcvqr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2pndhozov.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ckzcffsz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nfcujqgb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2khhpwytd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zyenvdka.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2dnfeofav.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2mcldpugb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jkmwzrta.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2oweamerc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2prmrsese.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2phdtrmbd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jzuegvod.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kvmrhnlm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vhvwdugz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qwaecwgy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gtzugcps.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zvyrdzdc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2hhfwxugk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fofvpihx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ypzxtcta.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bnmmutqa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tvktbdim.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bknvovsg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gkhydliz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2htypjzwd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fcciatjb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tmzyqsbl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mhlmivam.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qjookexy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gkllxpul.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rxscbxbq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nwajgquq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2uezfaqyp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2qicvnbtl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gmqaskcv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ianybscq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2soimjhrv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2xkvkmkrf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wvgstcao.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lmwqnztj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2anjeqrtj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wwcbfiwf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rircyyxt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ohrzlaev.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ogvjhgas.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xuisfvux.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mkdqnlep.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2xhzstrdt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2eqtzlfpj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ueywzjmd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kyhxeiju.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyorwoax.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2frfihbnn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sdvgemyi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hdgadhox.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pkewvvyy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ogoauicl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2qnntcvzy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2pskmerkt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ghkaxsbg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cxqonqnq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cllsgjoe.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2kmkluvqk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ancxqviy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2acwckplj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vtpjcpjo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2uyufswms.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2wbdsvsln.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2eqpllnxv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wtrixyzx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vdfzboxd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghmdtxmh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gvmsupit.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jbcqidxy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xuabfjbx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ytmxvyod.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2aghawvzn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ozvynqxx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcymttgl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tudndwnq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qjhqmboc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2eutrngad.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2txvbpmmw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2onlimuqf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2agdjxvqm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dplwqncx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2pbvbrrek.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jriehvym.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zoaqxjfy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2dbstsojf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mcnfxzwu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2eylttrzy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vdapwxmz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ovjskpss.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kiobnyhw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2theluiym.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kczwboic.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2goxzqqtb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2awfsvwzd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dewbinbb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2obtrawsu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ugntfapy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2kkzwubde.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2thzldiab.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2peihqush.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxqgygfh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2asmuuqfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbnxcxeb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bggcndtj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aolzsani.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2fxoukdaj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pjqclcqc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ulxjbotd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2snymmefl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2biaepfhz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2gzopjxxk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vzbkivzu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ptvdhqfw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jewdwkwz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nkodpofl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zwacojav.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2bmhewbny.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2stabkhiw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lwomnvxd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2jnhaeokf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2txlhtfhk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lsdabxal.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2lzkqyhck.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xwstabqt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dgiqhuzr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nqvuzgkv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eudcjdme.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2rzrmlpom.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxzohysn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cytmfgrd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lftotdtp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2boadladu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lvkrybpk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2txrflwdv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yphflnau.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2uvoxnxvf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zhsbpmmk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kbderowf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ibltjudj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2exnexsqb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wjwacfss.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2spwfuuzb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ngtomkls.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vugqjtzt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ltakriiv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2sjvdfcsz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2izeelqap.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkelpezv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pocwntvf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2amjcxjvz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mtqgmsio.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dpbywwuw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qvzjqtea.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wumuhxhl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ngyrxoyf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2kzxoyued.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hrfzvacu.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rwxodpkh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2lkxotylx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lzisxfxg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kemzaztl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2oxtbliyq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ffboukui.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2stynisvv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2abhjuzky.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gckwcfug.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xoijiaov.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2idojnyae.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2gpketvzx.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2bmkulzcx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2zhwcpncj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jgjwbvdy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2aczvnxzh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2uvwardqb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2eksulchy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2catdaqar.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ttzeogtv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fspkbiku.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fcdvngfi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vzxtudot.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dffngxwv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2snxyezev.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ntjetwfg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ccdubkyf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tzwypoei.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2gllpnixz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bqjtnxnx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2khpokhoi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2sqyqxydf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2uenivoqd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lihlesyn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2walbhmrm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cabyhrzf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ubdaeekq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttkzkalr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wqieijvj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mktgkbis.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2olaijnlm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2jqmmhfft.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jynsimuo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qhclslrp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tsvuneom.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2gczcvvtt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2rwhhrvju.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ewyhsxba.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2imbbjjhq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2boiqnwit.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vwntlesp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2clgnbwbr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qaxkqedf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2txwnblvb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpqwtsgx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kizfuyyq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gyufutqp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2sngrpnak.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vnyoxfia.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dyzmezgs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xasaekpf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2tyaelrnz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kutbjsci.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2gebgixsb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fbdeajqh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2kwuebioq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2uwltumiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dljqzhko.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jbinbgqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnejyjyx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2bhvvfrpp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2noocwkgn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2khlkqrhj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2saioeqmq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ndrekbjg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2astudduc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ffbodayf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jziwnqiu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xzwwjlyw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qnvjcjaj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2qwxnvqir.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ytctvccv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2dwnrhmpf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wxyvicld.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2gsgsvceg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2wbhjywrg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2azgfqvih.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2njxbtgeh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2xftmprpc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2mhiokvug.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zsqygfeo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ccyzogho.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pzqkcdfy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2yfmuwown.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2kbzubgfv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2vlcxuiea.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2zcvbcgsm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ohrabbvq.html


<!-- 参考信息 -->