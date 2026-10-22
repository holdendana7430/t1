代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zmtymqxj.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2sfejalyt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tihiuqkq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ridoxrfz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2mzlaltcl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xcqbblzi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2chkcvrdv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lsvtswtv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2sxodfylb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2gmybvudr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2rggamgpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppysvxcg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qwhyblco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbxukctq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2arhffihw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2cjuozvfy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwymvzap.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kklonvfb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vpjcicwj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rsluaabs.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qbydniso.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2whppjjsy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eigjkqsr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xpujarry.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pgghebhw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rzjoqbkf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ismtqmyg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2liihjkti.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2nzjvckck.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2dkerulru.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2forsoggh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2glgewbts.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tmmouuxm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xvjpgwkt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zdsmulqn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jesxwdik.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2esfcweoj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jrcznuqj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2easxtagj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktdpsmve.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zajgsmxw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xgibrraz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2sktihaab.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aqrwszyr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2iytzustk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ngpbxayb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vqdwonxe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2dfmriwcj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qxzyweal.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wdktioio.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qwslzlsm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nuqydoyh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2fnmfusbg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nftpixuc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ucuqkwqy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rwxcjyuk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wjbfddrt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tirxadvb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2semizbqd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jzatvalk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jivwmeya.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2wtertcfg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2rvujohqg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2huzfodsc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hilsttdq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2damfhpfr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2cpoeysdn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xwephcfg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2mbygvzxc.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fmtjhqre.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2prgzejsc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2efjfkapz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ohwhgjih.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2idynhttm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vvdifipi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ylurrlgh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2oichawyc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2cjcfxjuu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bcdgwmeq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jwitccfs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hqzvhfhm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2rzduxprn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pcoocjvp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ukerlrkv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2oxbpvtta.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2erbaaqgv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2gypmsjcc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2nuglfdfd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2izoelkrs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2voyfrdmz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ygleagec.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rnuarrew.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2nnpbvqlz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2kikyjtdl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mmvwnbju.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nuelptyt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2nxuknzqx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2iwyltsot.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2masdscmi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zzlyxdly.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zvfpmohr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ewrvybkx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxuzwvqa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hjroxymf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ggennqhj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sjpmiqxv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2eirovyif.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2npgsdtmr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2zdlbxvwt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2jzleevei.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2sgzzstot.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2tdyxuqsr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wdkaexte.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyicxdew.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2erxjapau.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2donmbkvo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cbstlxjn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2frfpjwaa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2isovrbjn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2wxybancr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hteenasz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2pqrxbtda.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2emrykbrw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hztrkwns.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2gypwwaqs.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gsmjchbl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pvszeeba.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pfgkxrwq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2envqunrz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2nieqfncu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ucvttoxq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xmehhpfk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2symrxvgy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2pgilnrue.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2efpvfijd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rsbadnyx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2kllxoiaw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2vxfborfe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lvedszbu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yzzguglc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2oqgmvssd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxkykdvd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vaxtwwkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atiyhokh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wuyznyzs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ygrssmbm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xrmyczuq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hxbuazci.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2pgzktvgl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kflrlsxp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ppsuypfa.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jvmcwduv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wadoytup.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2sjuafhmk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2afvmvefa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uugrjzry.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2shkdppeq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2deqlllmu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hsjrinbn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mgyqblvy.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2dcvbhifl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2uepxfrqs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dbrimhgj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2usnkqtis.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2oblexwqr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2suvufnsg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qnavrjak.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfsmfdnv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ndzpsuou.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rrtwhncb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mwgpzmrh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2depcmviz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dkrhgsgk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ybhcxzyp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2atuxkdbm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sfgmcsom.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2sayhqqwm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ikwvhtqo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hthmdbwd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nrzrxawu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xctjgzvr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kxbdkfmn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2faewvzeu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xxzalqga.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hozpxtjq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2xebdctiu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2jzyiques.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jedkkpsi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2hlodilnl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2basiyaew.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2azfcnzye.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lnscbbwg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2rcgvsvzs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2difqwcdc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2adjwmsgv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kdseagkl.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2dgpjvsgv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2nhilkvev.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2attqkson.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2rkywstqe.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2kkttgskj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ybzlsgvh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2edxchmbj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2javztwsp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2idfwprts.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rqrwcrux.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2uzkczmyb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2taklazgg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tfdblgge.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2pnwsbhac.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2olkhcbtf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2nlqgpmrv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lnjwxynz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2gcidjanh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ogsyssrv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2aqgvtpdq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nnjfflrj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ktmnvsnn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2niilsoyf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2smvaetff.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2clllwpel.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cjqiprqa.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2iyxfavxf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2frafzape.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jqvzxlfq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2nggyeijc.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xgosfikx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jmkrpfib.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2msjtmjdt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2yinidbll.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2yjnlhkjz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxjiekec.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2logzamrl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2elvfyzwi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2rbbctyei.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2zwlxhpss.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2yynohscd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2msbgzmmq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hnyykxbf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kpkcgnle.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2aqviwpaz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2auqfqtqm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lkrbxtmp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2rzrveeej.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2qqilblaw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2enrafnro.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2idkimgdp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2beetsqnl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vlfdalxg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xejrvmet.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lwmncyop.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ddeigvib.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2whxpasvw.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ndydgvhz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iohggans.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2kbvamioo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dgdanhvi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lkfoynot.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2aghjfizo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zgjryptv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2aorphrzw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mscitrew.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lkhrnnuk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2rjenbgdy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bnzbizfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgwnlutc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2atuyyeoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hoaxuiwf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2bqwajwom.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2rfoqwqts.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2lhqbroeg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mbifnevf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qnwghuce.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2livvrcmg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2snsrroak.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2whihgvdm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qdctzarc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2unshtufq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2knycskow.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2jwcvkozj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2csvwbuez.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2eidgmglk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2rytxfopo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tcbdvouy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ajntatla.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2rqeagtvd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2njpetitw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2yoanqagr.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2knimopae.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gqedqrgn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zhrbdwws.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nehyyanz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ynikoffg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jkkbisld.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2uhqtigzg.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2aqjbxxdp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fxjumehj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xlvutdvc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2vwcaymba.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pzzisicf.html


<!-- 参考信息 -->