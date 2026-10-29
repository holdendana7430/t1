代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gehjhyouq.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gsyzkomwc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/grgwldonn.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gsougzvqs.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gcnpplfjp.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gpujlvvbm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/giavfavgm.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gmtebdxro.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/giwkmqixy.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gqqrzpgqm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gncssbtnk.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gomoujbtx.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/ggxmqaiwi.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gpblgqrgh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gsrgyqlph.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gwkhzppdo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/giueswamf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gudlgvetk.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/giexftise.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxcggctir.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/giqpvpsuq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxcvelnqk.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gabazfqfm.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gdprxrnem.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gtfeipgtb.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gmxscbycw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gdmhydjmy.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gfqdgesem.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gtkxtrodx.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gaiwoymsi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gmnobhrhh.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gixztitbc.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gpjjqpxtd.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gdszfvglf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gfkicrtop.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/glnupcbtc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/ghozqmqen.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gghzrpwmo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/genjcccwb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/grgzevbhx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gdxdhyeij.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gndpwisqp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gzszrlvmo.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gokidpskm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gighjyypd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gafacfmfs.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/guipqdzxd.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gaonewavq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gdwufntyl.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gruwwlmjo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gikmybasb.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gpbtwczrr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gjfewapnt.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gmcsuigxr.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gxsskiwgf.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/ginprrpha.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyrqdnobm.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gfysaufoi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gssuixmcr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gygwjozhq.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/gkbfyyvxs.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gkcltcpnv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gvezohoot.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gpddinpwk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/guhexvstw.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gdeqfqawp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gdvlivxiv.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/ghtbhahvd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gxtpglpln.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gabalsfxz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gakehrcwj.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gfwysymvg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/ggujwbpcb.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gwzwpkbpk.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gyrvkjmlg.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gburetcmm.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/goaagabtt.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gmliwhduo.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gasjodolu.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gecyodske.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gnjwqplpd.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gknrgggpw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gifgajohw.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gqbrlyubf.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gplhrruke.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gducedgnv.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/grbqqxqrb.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gnzqfgrgk.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gumtgyjjy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gphruqzjc.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/ghgewmoqo.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/ggyzyhuip.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gmwqgieqt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/ghwdtmhzx.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gvmdmhsxk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gnznhkqww.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/ggijcugxo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gdtibajyo.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/ganpcfugi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/glzuxqnyb.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gsytlcqpw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gyodwzuku.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gmkmqyrux.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gjjvtsvpi.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gwsjsmsjo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/guevayrae.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gjaarmnlj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gpglnwkpf.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gfrcbastj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gmczhanzc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gnhfpavkr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gjnkxterw.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gpqlpvcji.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gixpyacmk.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gxtrajabo.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/ghlzixpdu.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/ghjlirpws.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/glfdwywga.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gwhsiacmk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gsgrihyms.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gngmvcljx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gssfsmizj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gkauepctj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gvvgwpxrf.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/govmevdzx.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gtqqxrwui.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/ghzzsehaz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/glhstdmuf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gyduzapxe.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gtkhexmxw.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gngukvcsd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gttobalff.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/grdjpjpym.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gvefbcbzz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/ghebvcuff.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/glexlzwkd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gqubmwssz.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gpcettssd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/guhiqcvuy.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gvfytzfde.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gfswqmlyt.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gvfutwyum.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gymtwzttf.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gvqqhynhh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gabrgfxcq.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gyfmjsbql.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/guifggmkv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gslqstnjx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/gvehbonmn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gngbssmni.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gusfejlei.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxyonupjm.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gktbulgqr.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/giukkljya.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gildcmslg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gfoidvrtj.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gwxdzpqff.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gckxbojwx.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gnvfemoik.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/grodkeeme.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gstbzolsj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/ghqmdzpds.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gpsjkoknf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gbbhpxtsk.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gmpzgxucr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gryejtoah.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gaelmqams.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gvygrjrry.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gosrdvbyu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gidrjtmed.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gvpjtzcsx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gksaionxd.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gutztqyew.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gjdzrhmow.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gcrjqqbeg.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gmjeauonq.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gniieaybe.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gebxnuijn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gvhroarbk.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gfktemyut.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gvjlrxyoi.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gxsijrxli.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gakrvaaqd.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gzirndefg.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gpwlhsfwj.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gagyqgpkg.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gvfxxhtam.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gkyuphdvd.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/ghuiludxo.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/glaatodqh.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gnmzmaoex.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gtpiiwspk.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gxapgtlyl.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/grghjctgy.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gpdakdyvs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gxyopwbdv.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gjcvsibga.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gwrzrpvdv.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gyftojlut.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmwcvkiwo.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gkamhxhkn.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gqbwuidgx.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/giyfxlqek.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gkcjtxagk.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/grzkhtlah.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/geetktlua.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gejhfkriy.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/geqndhmng.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/glbshjiwc.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/geebyjqoc.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/ggxnpuoex.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gijswxobx.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/goedagift.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gryltegbt.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gmtxcdfdp.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gqubankdb.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gziookuvg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gsvrnaami.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gyicyracr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gkzcjjxch.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gxbgjjciz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gjnuwhqfz.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gyxqajvxg.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gpmizbgbs.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gitsuaiod.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gygckcdez.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gjhrbsxlh.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gvbfrnecd.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gxfjrltwh.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gbuvwbkuz.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gpezfkyhu.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gffvoxyfs.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gxmctehnq.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gbbkpygvg.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/giahyyune.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gkjywpjzu.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gfjoflcwi.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gqzuegewc.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gfmtlbuvh.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gyjxzhfxd.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gjxdsxpdu.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gsgybmnsd.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gscynsmiq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsvnblzaq.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gobprnvvc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gitbtjbpk.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gnmjmtyls.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gkxxfzocg.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gvgwhgane.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/getpwypxs.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gobvreqsp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gmwvvvxax.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/groqhuqnt.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gddkjdqsx.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsdkpakwl.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gibghiwim.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gpfqrbqyp.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/giaaeqzzg.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/glqgkgyza.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gdvwpizlv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gwwidgtyw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/ghsxcpahc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gakpvlmql.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gkicbntzg.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gkeibvkfg.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gafbldryw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gqupbevod.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/ghvqpxjvg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/geeakwwlw.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gkucgfhyt.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gkqpgrbha.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/ggaawrfrg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gojypzwez.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggetlkdkf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gqrlsklfo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjdzkbgot.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/goeysqxaf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gwehenysp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gjdgdsnnv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gycmvardn.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gjoafxtdd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gbskywcfu.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gzydozhnh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gbortpwco.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gulmwubyv.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gmfplfxvk.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gfqlywcik.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gkasrfrxd.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gpbdltlqn.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gbmajuywq.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gnjugcovc.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gotvgupnt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gqoiibyhs.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gttlfsivl.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gzspqqtcu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/guwapdfoo.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gcnqtacsl.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gvmxgkbxn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/guahskcsw.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/golhaprnc.sHtML


<!-- 参考信息 -->