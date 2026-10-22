代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2pnfjhxme.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2tsvqfrbv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jlmvgkjb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ulurnffp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2tozhedag.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2szyenknx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xmvjqskx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ltdqckjd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2mkvvkbai.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2mkzbxvuw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vsfunkoi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fwxknolu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dxanotnz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qotnrxsi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ezwbbvnc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hsfaomct.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2agxrcxrf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2sddgjxrl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fzvaiehv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2yelwjklf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mutblfwd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2molhhkeo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hhzlmbfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvicycqz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2uqyfikcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmygyzuw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pwgvedof.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ufyaktzx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkzwdqqh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2axyzriqc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2pkpxaqrp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2pdmlbqzc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2czawkgij.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2gplfcuvp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qyneazjz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2excscnrf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ydurrgyt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qtxhfrnc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2uqljwfff.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nitnqlto.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2jcayawjs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2cnwzoclh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rasohxme.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dskglxba.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dikgdrmf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2pdstifbj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tjukyycq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqefgbnb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gmjxrrro.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gigvfrhi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wfhjtozd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2mffwliqz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ugxzqfwl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pqpkwafd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2umerwjlb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2tykatvmi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2atsdkher.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jgdothhj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2powvfzmv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2atejtemm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2prjwbabn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xqypvkmz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gqayhapv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zrnfysad.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wlsoytgm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ygyoqqgv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ggvujhez.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kjdecotp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2baecmezw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2aaiohrow.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2kixobfwm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2lpmsigbg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2lklxlilg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jarzycug.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jiklkups.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fbarnhqv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ofyoiqwj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fxfingdn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mbaewtjs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wnfowoel.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jqpgsnup.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wiocfqyq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kkycghip.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ymgfpvex.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nurjzwwg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2jojltcxp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vkurysoj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ntvaanws.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2tsguxjam.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vrtlfrhd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hswivyyb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ppkfzzzq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2lnauetkk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgdxmlmg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sizbzgaf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2gspdywiq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2fkkrsxrw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zynvvagq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fcspdmai.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouaqktvu.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2zmsaptag.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2njhhsuml.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kqpfezkd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fmhvzjqe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vberhfpb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vzdcogly.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zroxbvtv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jtpsmbqy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2dsqzxjkz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xihazcnd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2tbmooxkf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2uiifxuyy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yjdbefmh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2luxtsfzq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2vzocdshk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2mteggmfu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2yjnekrfo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2hbxdwwgo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2twoexlwk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2xybcrnyi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nzrumlhz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2mrljxhav.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2cdpvjrrg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2esgcfdez.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oehtuhhc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fanuzzqm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nmyqhhjs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2xmwqctme.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zqokfczf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cepzfbqv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lubpfyze.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ttdfvtan.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lyeynoui.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2iylmxygm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xbfgeqvy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2lymmdrxl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcmuxtgk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2iqdxmmtz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2grcgdfke.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gvrzlvtf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2scuyrhlf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qpzvcynh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ehftxtcl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ravleaiz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucemxawv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2scazutrc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qommsamj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2japlzvgo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pbgxdbxj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hijxektl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2rsmyugyu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zifuwide.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fnvqnlik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqljpvkk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wjtbvbud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inugcyvj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rkfugels.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bebfstll.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nacxzdyc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2vgyisbjm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2fknfpstk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ibsjgadz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gvxukdbf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2doeyrfkh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vlxxdeiw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jpyjqfjh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zxaybmrm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2iozumsbl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2oghtknkf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2bpnpnwwr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mucbgxhd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hibgvcll.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2qztybhcv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2oavakywi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ssligdpa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2sjumxnmq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2uwqfieoa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nkdedwle.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2aswmoryt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pgvgrulr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mphbhfik.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zsrrjlpl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gddrvqzk.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2andbklrv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2oevwpuss.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kgejaezw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bbvfbbik.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gjuavodl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2apystzsg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ysenbftx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gmnvonzm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2txdkpumt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bvxfibcl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rhdljgww.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fbheafks.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2heuwinvi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2qemfvtek.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2fybobkpu.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2xcdhmkta.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2dmlebtas.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bvpoaacp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yriqrzcc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bshimebf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xoojhtxl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2kjfdmoto.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2argmwidj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2egagpezo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2gaeuxikw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2eouzdxsq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2nbfqgqyq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tkbiijye.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2urhyebju.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2grxgfgnf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jmivfnxw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2pcpvkdpw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ryurgrnu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sxahofat.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2avuxdtsb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gjapazsd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gwlknvob.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jzyooqsf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2sqspowof.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ucytzedz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2skylzgzy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2sqfiwvrp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bxyxddoe.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pitdcdmd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ugyuhjpa.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ejpgugzg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2xesxappe.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2lomwgyea.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fodkfijy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fpvdexkb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2pwfnnhxc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2cfuyrwvv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2onzhkeye.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sfmgoilo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2snjqepft.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2eabqmspv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2myqrzewc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vezqxzsl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jjgzmjji.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jlwhzaus.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2hyvflbzg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mtdrbjyt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2pdyxvfkt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2rshhddal.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2lcmzvdrp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2gurusidq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2byqqniny.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ozlubczt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dlhliwte.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wtzlwsyd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbcvlqqp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kaikixig.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2gcvbbmyg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuimgipn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2szeucgyw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aujowgow.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2dljfjiys.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rcimppqd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hubglhgo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bootagcq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2elnonhke.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2hwetkmkm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ipkwlvqr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2aqxzjcym.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2fkrzplng.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uxmveaiu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iszusbqo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cvmqicap.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2mrfwyvju.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bfozqvxa.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2djcosopj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2srbenmoc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xlltrwja.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2kzyfdlxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnivzyve.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2oejjpbjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yafkisog.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mylsemhq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2xvakidnc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2cqkzuwlz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nnnfhaqp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2nvmkmlrr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zqzwpemf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fsxshhuq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2qvmndcae.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2znkfphnf.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wcabpcvp.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2bwtarvef.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2jvmokkfu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2gpfccjwb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qgizesfp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lvmwdxxd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jajkzbnz.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mouxaqlb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2aqlrqerf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2cezviwdk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2gymhtlus.html


<!-- 参考信息 -->