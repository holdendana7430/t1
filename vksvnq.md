代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2xsxssvwc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2cltvpdha.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2herqtqia.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cnxwjeol.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2hbgjvcsx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xfztqwcn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ydjqpefu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2qvfrsqpw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xmbhtvto.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rbqtosws.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fkblvswx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hsrhxpfi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mrilndkw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2youghtzv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kmckagbv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wgrfjojx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rrqdjlcz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2adsfasfb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2sdztwzpi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2tqupxztp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vguzvarb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ybmmktbc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2jehookjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtgpptbl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zbqgylrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsmmmadv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zedvkgwp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2bjhuoipw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhebufwy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ihjbzedq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2qnpdwhjs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zasfqsjw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2qcynnzfv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2llaxronx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hrcqgnmy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ibdbuepu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2actwzsas.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xxscgpbd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2irprgisp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2frlmhody.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hsudoasl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ykehvphi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vfvadasu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2cybjmbln.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jmpcbvsi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nkopzefi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jwovdarq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mgidnljz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fdxqzhcf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2pcgygskz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kowngehn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tsichpog.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2luxrylto.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zgzlapqq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hnjheyru.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2umlyymkz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2mycdqggz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yieflewz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pjrhagav.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ixmauzuo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2cdvqmckb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rggoiyfi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zfekpzkc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zpthbfty.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qsefnyfy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2oipkeewt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rvfulozw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mjkjiwjt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2canocdal.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2fvdrzrqh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2snqmpwvu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xyueowcd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2vwkjpjhy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2omecikcp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gxdgjtqe.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rdgdkxns.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2okzrlnym.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iegypepm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ptevhznc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2stochjzy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qhkvxhnq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2nerjgrsd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lwshmnui.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ltyuaapu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2edwpyeny.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2apsofwbl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2uyulvgiq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2usiskgev.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2sxfvwink.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rykdnpaq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2aqynmucm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bdujkhlh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2lyhvramy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2eldwumml.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2bgwbmpmi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2grdfgimv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2mfhuqwqw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2whkbboys.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ksvtghak.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmkxcbgl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hapmfzdt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sinbnyli.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2iiygofnf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rhzoclpn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nvhhebtb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xhnmlvmu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2yycrjlnp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bmzwqhgx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2hxiwwyis.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ymlcwdhs.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2tegpcnqz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2skptgzlf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lyzmwtgr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gyadronn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2imegafie.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ltjikddc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wfakyroh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wefowwzh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2yzjnignw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2siycqzwy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tpwmzgbj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hzykoyui.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2nsrnjhuw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nfrdomdk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rweropmt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcabsjyy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqucttrb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rqzrsjrs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pqwxrbmc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dtjwamzs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kgtdlbur.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rktgmwgw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2asacwprz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2xcflbkek.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2kunzxqmk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2fgnvhmfq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ytyzwikb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2arrzjmic.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2rxymltfr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2birkbiic.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dyhddaeo.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ivneodud.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uctsekaw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ehxwhqpj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lqxdglvt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ucplvizp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jovkviyw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zqoetupk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ozotexpg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pizkptnd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ojznjbrc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dchqvvhy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uuyhbafs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqtgjzsc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wmycsvmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvhzsbjh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tjnuzouw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cvccjskr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2tlbzkxzz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2jrksujyy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dhqsirzk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nborecof.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ijbdcuae.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mrbdsdes.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2diepnpey.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2sbwcckci.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2iwffnsct.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ubtmfnrf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lfyqdbqn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vtxpupvr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gbsiqzpd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qiedeowx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2lyvpvlpr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ukyclkyk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rfkuersq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2rzuzhljr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2obhtbxsf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2oqgsydlv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2udccdbft.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2farnrqfi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xzqgvhwo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2iqihifou.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ujkuxesx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gjawsnmj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2uivmzcnk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2jkfmtcsh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ufkxmmby.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ljukdugy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2cgbdoqhw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2akzrhmgz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uvijpxsd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2utuebmir.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2yscnrars.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hdiumygg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ykcfamwd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nzzftetu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ayysnokm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2gakvpsjw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2tiirdnyv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ejkcrywx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2zyeykcdf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ptqqedil.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hxdlmiat.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ibrmlfkg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2nrsyucdo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2frtwllcj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2xtezwthp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dwtgyjtm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2konluclw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2sqeqxokh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2jtsusfiz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2kbyjetel.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2onbablyr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2txcwmvjj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2azhzbgri.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2uoivczsc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2usyaozad.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qjdkuyda.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ycwvbbum.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gawqgfxp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hvuirszk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2cnuczokz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2uiznwfaz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2nzivqfoc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hajcrttc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iumharxg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ahkueapc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ienvnzkf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tbzmjpwp.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2sidghopa.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ipdcjoql.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xcefqmqx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tjippnaq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zbnbibda.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vtobmwsx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2tttjameu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gtqcxrdn.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fkpqnelq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kwciqbpc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2crhqtyrx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hfjpqikl.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2hvuqsvqb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cnapxgyq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ljnuapsf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qnmyhrho.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2cixhwxqe.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2iqrihxes.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wsfyabph.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2uanxuovp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2kqceucch.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rilgkisf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2hxbfcggl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2hjueexiu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qrepwzte.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fulmykhm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2aqrcediy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwjmqtmw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rkhdgxes.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fzdiripk.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vjouliwg.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2nihcdcdu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pwjbyygp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ngprkzaj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2yaapilol.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2vmmgruod.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cissehxz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nekjzbxn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2psezmhvs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pgyuwexn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2szzppmqv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wzctasjs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2rbgdnofa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tldrqlmt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2efmwgdjd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2evydmtsf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2bdpiiavz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2dfapjoge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npylbytb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lxkcqacu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amcalbec.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2zkwxkdmt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qdcomgue.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wzobryla.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kihqxadb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jbaabuhh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rqktqqwj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2bmxkgkmr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mmewmyxx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2eymniqus.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jkjdyuqn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wxiwhyzi.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2bxdgrupn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2dsxvdkzw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2eholqakp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2bqfhjqbz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2yrpshkuu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hvwpgrmp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2klsrtslm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2mlzdsmsx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2jadftnbq.html


<!-- 参考信息 -->