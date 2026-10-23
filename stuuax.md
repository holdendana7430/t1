代发 wailian999

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3nylcbxiq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3uoeogqdt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3stipihxv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3uaymwaml.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3cvqaebed.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3pbacmrnq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3einktexj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3hnblosfs.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3imoekajy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xpeaenvm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pwddzfvh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qagzebde.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wyxtkyqv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jhofmgix.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3sepetvej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaqvmggm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tvrorobu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tucdkppy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3biopdlin.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wgwnauzc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3iqtnbjnn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kqowdayg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3lrptpvjh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3mhazzwkq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3uclnmnwb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qcrrliqb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3frmnqwfm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3niysjpae.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qmzbzpzs.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mncsbuom.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3khcxgotr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3kmplmjzt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3dabrxoks.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ieqzkduu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3twqggcwr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hmmexydb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3pdhbxuio.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mcgpyynb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3scnrcqcb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3evtczvyh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vxxsjkgq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jvbxujit.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pbqedigq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qfidqruf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ezcerebs.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hwupwnui.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3trvjduon.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mkymlxil.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ijbhytfy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ydilliyd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zjbyrnpu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fyapprhr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qjnocfbw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3emurysfv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nbaezoki.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3clvokfvb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vzdvkuqw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vjsinoiv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wozelxrc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3pndeyfbs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3azkhtknt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xvxjucsh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bjjymwdh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ujksiile.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3okdsdmyi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cudspvjn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3yfkthtgm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ocoainyk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3rfjgttwa.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vkqkyvdl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3gckfkuon.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3mrmjustv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3agtanjal.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3deufgkdi.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xcihbpbe.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3wtyrrugp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ahwuppfd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbpxfxgc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ydccmqah.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3gydhdiaj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3nfemfucy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ssqdfxop.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3rpcbhygc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ehrlvnml.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3wluzwnjb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxnftiis.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3loobaliq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3tfxilgth.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ffrcvyvu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3frnxzhng.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rhpqgpkv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3loqxqgcz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cgdgefit.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sitlkliu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3pzlxhnzz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3waqewtfn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3kvbacbtz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3yhdyxinn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3uhfltlol.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fkipwwrh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kljydszm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3njjqlvcv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3lubtyftm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3afbygvjs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zjblealq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3nglobivb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vgbyzewo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nqkgdnuz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3obxqiuqv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3nolxrthr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gppbzbjl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zidlpcrt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yttkcwrx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3izlxtogn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3bvnbbinn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ozolvxqh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3etocipiv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3bjuosaes.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3juytelvl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3pointkda.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iybllqyf.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gyjuztwi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tzabrdzu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3sfbxycaq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fghopsmt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qpskbyny.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3swtslhoy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zdrkeqnb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3onhlvkkb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3tddonicv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3tfkjrnuj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ehganpap.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3oggncdca.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3udjldyaj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lnambbus.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kmlppphy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zntsemka.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dyxyhxkr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fgwncqnb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xbcbrvio.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wlykhywl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3octwughi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3cgzttcjs.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vtrsdjkx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bvsbqqtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kavteqrq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3rihhyzye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlqfamgo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tzvsbbdr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ulvaiqtb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3mobxjgwp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3uwnwalvf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3yriwgiuc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lqjdxtrd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3imnuxeit.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jefutcbm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dxhvqcdn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3maltehxo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3aqqshulj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3klkptsdk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3htlqkygb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xymvdhjf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3thhfuvly.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3namwreey.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3czfajiwu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3mjjzxjim.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gjacglqq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fiqqdsgy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qwlflbga.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3waxrcchg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3krxiscjr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovckgwta.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3plzqybkq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbeqhzhw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xmxbwbru.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zytexdwp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jukhlmve.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qohenkbw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3blxixdqh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gheifdrp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hsbanixl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zjmtuhft.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yfjcwnft.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xmrkjbsm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ixpjezqr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3foiyhjgt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3acwiyizl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3hncjiptt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3mtfhevin.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3sodthpbp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3xuqorbyj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nwznajpx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3kvhhxacg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3athajrmz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ghbejrxv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lapeuyvj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3nitxdmzt.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3uhwdsvsc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3hbxqkqmm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3chfdmxmz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nystovvp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ntstgdzq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3huzlalxi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zahzzjqi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3tmecrnqj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3veimscay.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3xakqygfy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3yjsdorxv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jdgwygor.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3meugulew.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3mlgqggfd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3laenjdha.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3kogubgsu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lymhggtk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3vgzpdibf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mlpuxrsm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3atphrrxy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3phwpybgj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3zrcfagnm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3tpxspoqz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3upqfsznt.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3gumvsqfe.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nwbkqpqs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3wmacghpg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pixhwarw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3zxxedkmv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3vkajjybn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jtiyqmyb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tgseggun.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3kngnoleh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wweeamrc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3gdrgqiac.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gzilpjpe.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3apxvmpcj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ucmakupi.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3sbxotcow.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hntvnann.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3wzsdykzk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3desvprav.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3vqlzxddk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3mrxivnuv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mknmnuky.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fblvjekw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mfvrkggn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3gotvyjqz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcpmiumr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xobdparb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3jknvvfxr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcevsops.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wabutbge.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jteedgeh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3giyisqvo.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tulsooum.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nuadduag.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dbqzrili.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fujsnqrn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xexhiqfj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kqdxcqso.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yacdpibb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3dyrmtscl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rqixcjvu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gopgaokt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ofdnwrxi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3momwyadp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xyoefekd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3yfqmkmkz.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ioxdfjfi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zoapxmkw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhtonpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okcgaoak.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wlnjlaho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqkfsjpv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3nbzziiug.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3juswhnjg.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3bvktsbia.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ugbcyhqs.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ceebvqtl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3gpmcsgab.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mavibbfc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3saysjfyw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dyyrufyb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hutwddvc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3tcbvhtyc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3jslpakfc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3zoqavjbv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3csnnkijr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3kkfaamcb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3svtpvvep.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bypukwzx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3yzipumnm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ptyqajcs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3alzltzah.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lxojbrsk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rjgvgyus.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3victfdlg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bfpohdpr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qbizlwap.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rjzeyxqs.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dzdtuyvz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3dlquzsig.html


<!-- 参考信息 -->