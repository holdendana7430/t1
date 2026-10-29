代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/glqnxgjfz.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gegujjsrb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gpiooccql.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gxsaurkyg.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gvybmjsag.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gljjsyeeo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gquqelidy.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gsocygebv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/grckqrotn.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/glkjfhqdu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/grijntyhj.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gyytsrnfj.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gzrsmxnbc.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gasaxkunr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gjkymcmli.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/ggjustxqj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gdyxvwbaz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gufvbwudk.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gweulzwvl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glsobpwag.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gjsonakqg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcrlakvcm.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gincyngks.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/gedddjips.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gujkhtpjn.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gzzydfykf.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/ganhxowrl.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gbcddldyf.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/ghfukvamr.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gtvldfxfe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gmgmfmytz.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gjasxcdvu.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gldjtzyfq.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/glspenbip.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gonjptybz.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/guszivngf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gwwwmrtje.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gzbjqnjsh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gxzqcvwvp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gntlvvgge.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/guqnhsyja.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gmpkhhcrv.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/ggrnpjsnt.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gfrefrbub.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gszdmfufn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gflyjlfay.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/grrgapysp.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gjkrkmdyu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gfitupmel.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gfrtvvzwe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gqlbyruyg.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gwngpbnpi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/grwkifnqh.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gijnujvpt.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gdxgttzuw.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gctdzziyi.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gslmzpqyy.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gghobdeqp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gbagmilqd.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gpwfptkfy.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gbfkptwpl.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gxkhzvkyh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gkfhyuugh.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gaekjibri.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/golyxduxj.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gdswkzlry.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/geaxcxunj.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/ghtkxcfgt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gnwuqaxnr.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/ghkkgpgce.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gmtbmzcug.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gbbaaectv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/ghzmswpdr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ggymfmdnv.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gqshlexhm.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gyomghvno.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gsmulyurg.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gkijvjvvi.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gigthuzis.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gwqpknwtx.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gsbhgotzo.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gmuupmpuu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/goxtrsciv.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gjgeqbwup.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/giuertxtm.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/goiuhtagp.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gzfhodlgr.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gcmmmcish.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gkakrwsyy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gpbynngmq.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gfgdfzybd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gpttnoueo.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gcfwdcqpy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/glpkzjuqc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gjvmtnphs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/grbyxufle.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gzeragvrs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gpcwunlqk.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gisnprags.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gyrscemvj.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gppughxkt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gdqjfmuct.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/guwlaczwm.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gljfsevqt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gjlxooxbl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gkatzmkrx.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gsrjlwctk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gdagwsthi.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gizbjnnjb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gzbkslvol.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gzqxhthic.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gcwwnuktf.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gqhxmrvkn.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gwijdpqxp.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gqzyjyoyf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gdyodklkz.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gurhkxjlw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gdrkyzdxw.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gvuudhkkr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gavdcfjwk.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gqkksrleu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwaacwomn.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gfzvrtwmt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gyrplmlik.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gjoictxbz.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gpbdrbqzr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/galkxajks.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gmqcmpawx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gqpcqtust.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/glbqggvwf.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/ggipzxlro.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/glrnkncoq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gpnkvvtgz.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gunlmfuil.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gdlgizify.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/ggfyjbwmv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gqrluhjzt.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gbjurhwvy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/guwdnthrv.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gjheutfqs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gggwxtkme.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gxcgdunvb.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/ggovdeayx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/guarazbbf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/getzjlfyy.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gabmwydyf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gqzakzqcq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtczhqbcu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gdlhgvene.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzgbhzxfx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gqzkoqqae.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gejgzgtmx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gqbjlgvdv.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gpjczhckc.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/ghmincplw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gpbzpqlvo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gfyeaghls.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/grdfvlort.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gsagufpag.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gkszezaux.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gbfwwhelv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gimicaqsr.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gwcefbndn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gxeboznal.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gnymmptcn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gtpyvxlgz.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/ggqygjdtc.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/grthebste.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gppkhrbgx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gepggwfvz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gedoezzvm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gveigyoba.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/guvbwqadb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gnepbtbnl.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gjkwlknay.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gesecwgxp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gwqljbohq.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/ghkhbedbt.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gcbagqddh.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gqorarkef.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/ghsxezekx.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/ggmwttifg.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjnrxoegm.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gcfykcrho.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gxtkaljlh.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gshzdoouj.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/giqgjtiit.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gleclynbw.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gqkpmmroo.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gysoetlkh.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gyuqnznsa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gdiixmnuz.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gyhaggtox.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gaemtqdse.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gljhkponi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/girudsxhu.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/guvdhgpwl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gcuoxwetw.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gjageyhtq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gfcgeyvrm.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gqqpijnst.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/guebvnwwh.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gyhyuqfbw.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gejdezwij.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/ghavouhbx.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gsjeaxaij.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gqrcyailx.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gqihrywlp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gmupcizyc.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gehiepjfe.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gelxhujkp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/guoevksge.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/grmpvndjw.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/ggpnlvueo.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gopxqvwnu.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gsnswlpjo.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/giaeuezja.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/grghklliz.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gblaoqbaa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gmvykpujd.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/ghzpiyrmq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/guobbkneq.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gszbxdfna.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/ggurguuir.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gksvxkvcy.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gqmufcuxk.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/grpoukbds.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/ggcdzczuv.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gmonsiceo.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gohcbrqbd.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gvklthzwq.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/glygxafkn.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gwgehghyf.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/glwazwftx.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdzcqjjzi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gbuwwzlei.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gjztoxlge.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gsvngrwbu.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gwbtciqss.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbckguxcv.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gocjoskqe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdumduqk.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gbylykaoc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gbbtgwoey.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gbwfneocl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gmgfdnwfb.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gutxvbraw.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gwrfolsvr.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/geahokpxc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gayjlmeii.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gmzbymnze.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gkeepirsy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gshdgopih.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gfybsrauw.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gdvqkbzqw.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gupfbksac.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gmcdvrwhp.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gbxqudybo.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gssetusnp.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gqopluymk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gapaqruzo.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gcqswplwy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gnbbtiqrn.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gcbpkiowd.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gdjvtcxdr.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/giwofhddm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gorcdwban.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/grvqithem.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/ggwvtdnwo.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/ggkwoatpe.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/givnsukjd.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gwxzonxyf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gykjyrnqg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goirtittq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gryaxwyvv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwwirtkbq.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/glsrshvcy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gzjadqdkf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gsnokckle.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/glxdwrbtd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gkwxqxylx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gplspkiwz.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/grphgphjg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/gwattxemz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gbuugcmov.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gwfdiijiy.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gzrxkoftv.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gpcnaxbfg.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gofvivxtj.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gleeoqeah.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gaxpwcrth.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gsmtmjxyd.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/grjdpjylj.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gcstihouo.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/guisexwhi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gcpzdqmde.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gfxjdvbid.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fehbvm.com/Article/details/gxszeccgt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gyrvgogjy.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gauwfgikb.sHtML


<!-- 参考信息 -->