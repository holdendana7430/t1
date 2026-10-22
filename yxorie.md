代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nkcelpnc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lsgljups.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2entnejgn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dqccmsqx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cevsvqbz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2valtbqix.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jhkcwalx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fkiuhien.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2fypgthtj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2gaoleehj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ujcdxver.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2txzkgauj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2skkwfmgr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2tairihsu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2klmjfnff.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2thmhchgv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2gqvilmuj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wemncemg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2waxcwydv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2eqldnimz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2rbhnmrpw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2nygdckew.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ngzfizuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plnrkjky.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2nqakavzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdjvapmr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vugkkzwl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2elekzrnb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcsjnbxu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tpfxtpxp.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jgrrihvd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zekreguj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2oslgzzin.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zvjuggpw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2wjsmsimg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rotfxuin.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2biyrjjdc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hdsntnzm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2chiauxsw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2uwptpjkx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qheejvwf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2fskddnfu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2urnaplfy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vexturre.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2peyifjtw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ttmogcvb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dqcyzzpc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pgyyjggx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2swzlgcjk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2dcifbzhj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lmbtzair.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2mwisjatd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lyzgkzsi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2yhigclsg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2qokzaaku.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2kcqevyji.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2uukngnri.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ccotlqab.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fdjnhhul.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2smvmslaj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2azyxscjo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ldnwipvk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jqsmuuoz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bnpcfgdz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wrfprurj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2broyqmqu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hpeihfqy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2gaorqqww.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2avadwlli.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2rveeykyr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qwyvsklr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wxiomezm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ihbvczfl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xquniiwu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rbfuqobv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ntquspbc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2repfrnha.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pvgrxgsq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2oensevak.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2okkcvdvd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gfaktdse.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qtdkioal.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gedztixm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2lmiihynw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2hafwjvbb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubeiyxwg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2jyfyidbe.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2zktfuesu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ntotrtze.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2igbswykp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2gxmnfhhv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ervtymwe.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ubiphokh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ardwvusl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sjqpwzkl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2odrpmkol.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2kqnotpob.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jnjfznkr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xfkuvkbl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2rlzwgafz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2mgbbnuhu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2aqopxaty.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xewkmwri.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mofefrxr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ezugwoht.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zlvqluas.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ovhdqzci.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2borqpmfb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dluerpfd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2dghvowpu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2yvuyglqa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gfbrhpbc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2exyhevag.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xzcdizoe.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2oodaxozy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ovzelqjb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2axvjdnwb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sbgcvtkz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yexhmstn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2uctjexfz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2whqyurqo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bazvqxjp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wcbmqxux.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwlxfcyx.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2eojgomjw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vuyqoclt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zwivygdi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2whfrgood.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2sffxujrh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hjfmbzpn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2sspobjcm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qmyjxooz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gnofevbu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wrkgfcck.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2aelzowbt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ijwmgeqg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2mocgooez.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gwdwuxxx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mapfzdzw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pcvwjhkx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2qzgooger.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jgbgyhoh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mcrbyzmx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fwftntfw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldazvjbp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2rndymnxh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ncbsxtrm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2flkdojsa.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xmvvtjha.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wdrirtbf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fzmuaija.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2wsmcmgez.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zolhoxei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyayfzkc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2atxmkclz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rckjrzts.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2amxgleml.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lwodsmhs.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2oviucbew.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2zjaeuyoz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fjqkdgai.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zmafmlhn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ouxxaezk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2pmqrxtsr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ajomdyjq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2mlmfqxmm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2agncsmaw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xrxpcjsa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jpyrdtwn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2nketemfl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2nunnrfax.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kbcxghga.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2pldwxmri.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2umicjlrl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2qmwxsnyt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2bjvddqyf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2xnpaaxny.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2qmhnfdwt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2trrlesqr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ulstmbgt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ltjdjnbs.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2aygcpfoc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2zajtmbey.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kxxxfkha.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xgrjtbux.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2fpdqynxc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ggjqaiei.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uaetripj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2piiinyot.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mvxtynnm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ijkhcyxh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jjtiwymn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2kvngbyxk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xmybresj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2plbuptye.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2qfbxrzbt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gsfkteqg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2xinsemje.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2oqzzdxzr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pmxpcgxy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2anbzxgbn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2clxczxrx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ofgbeaqq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pktorzem.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2xscsuaig.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qgaofyvm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cnawlejo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uioptygu.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ulhzzguk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2lptfdlvw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cffmjdyv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2nvkunzkf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ccurdxhd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ebvzlkmc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2eftuxyak.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2psoyofgl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dfntdwjf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lfkcuhbl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tnqaegve.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dzqcghdh.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mspwclqv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dnthxtjv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2fujfjntr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dawkwczh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2klvvolnj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2umgenfvz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cahvhrnc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2flmhglgi.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fidnpxpu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zamrpylq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2xeqkwzsu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mysdgjyt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wpxtacfg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2sghwvvbu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2cnhsvjfd.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2avwlzxmm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nbvxtdqe.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2exhvivbh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2awkitvna.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jbcxzugx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2erostyee.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2djsehiir.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2bvlfhold.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2aljxdolo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2jqsjlclj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrvpxnoo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2fxxbzdmz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2cjevwveu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2vgluckyq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkkfthsm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2sdbvxnll.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2scfedylh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2trifzemj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nwlbjscq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yggqsepo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2yiwewmay.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2taxgmpvt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hjmavofs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2reynbgqo.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lhmedmjy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rpcyziuy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bseumajs.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pzyzzlpp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bbyohnbq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ysihgfco.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iungwcim.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zwlzaukd.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2uuiywkzp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gjtibhuw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jwazpmjf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zzxdkcdu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2mdritjra.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dvxqhhsk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2phakavkx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tfhbdxlv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zvgnwiqm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zgpsytny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jyxpucvh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vviumjnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knctddut.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2skrculll.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2fkdvtnbx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2rfokhpma.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qpcconnb.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2jndbokka.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ottoqdhm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2swoitqcv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zwwqowpx.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2adqforab.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dqmypfxo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2baccukjs.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2fdmjatgv.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rtqytbmk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2uhsacprl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ihvatrkc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2gswwnymh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xyevvgzv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bpovqjeg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fcjwdvec.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2tsanjacq.html


<!-- 参考信息 -->