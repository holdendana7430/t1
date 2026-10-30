代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/ghjytqote.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdiigheq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrigzbtf.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtxttpdl.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgfvudaj.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkdjhkcs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtmvzwlu.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gcmkfmnbk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtjkxcye.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrhzgtex.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqadwlkdk.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gowlkqcwr.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geebqnnwl.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/guqivjtpz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybcsvuas.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gebgsiarz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gibjlvthh.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcqpqcss.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfqhzfgg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgwhsjxz.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gujmklegm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzctodfa.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqcmxuvc.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhxzjwrf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkxkwbfsq.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gjleqqfmi.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gigpchjbe.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gfntbkaje.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gulmzclex.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtxsorpn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxshracpq.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gcisjodst.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcdnhwrh.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/guniysvzk.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqmzovbc.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlxqmfik.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnqjhuih.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gxmtzlfse.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gawhrsdbg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmfvlisj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/ggwcfggjf.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gtmjdqerk.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqvvnzup.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsxrkofi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqmprbmd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gadobwnvl.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdswungog.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbjerxse.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdbkmybn.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/glscxjgiz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/grlgncrlu.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gdldekzxj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/grbcyhcub.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/giadcbjcb.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkzlcexb.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gfjgubtxx.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjehfemw.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazaubgme.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwzcqpdi.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gujeorzlc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxrznivw.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gnssxusha.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gdaaovmno.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwucztwt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnwnpkdf.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gczygejie.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdlopdvz.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzkgmqux.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gotamogpr.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcblpirxj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtsgdqxv.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxqsfnjo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gwztzyghx.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmetyabs.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gmstumqkq.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxzjsnch.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzprxlpcn.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gsekplkyv.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gsodckdfw.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtioqowo.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmlxcsfk.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqculmcpq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gospbmyxv.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gznbpdlns.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gryyzedsf.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gvjmoucau.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhynsffb.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfoxvnilo.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/galauvpso.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsjdflrz.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkpkbrjf.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gxwdbgdtf.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/grwmuhxhh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gsqvmqhuw.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/ghkuwkozl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvbigicv.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gvsisekwy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gselussne.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gncjcflkd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaptrvzs.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gzneryvjn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gatrigjhx.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/geiuhlnwc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzefigaf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprwuqrng.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/glmifmkgd.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeosxhwu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqlietrc.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/goiozuqef.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpitqzev.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/galfervls.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gwtsergzf.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzageawp.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/geagdaljp.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gsmbormfy.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydvxmlzj.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/grayzmmnz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gbbfffuhl.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gurxafusw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gownivrmy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamngxifz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gptywuzgl.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gynoystth.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gevygahfu.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnzjhfxk.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeilbenx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqetdthf.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gcitkvrly.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzzopaeg.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/giskexpsx.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqrxpgxd.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/ghzhbplif.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuwcwsmp.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/grjxzsrja.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlfvnkwk.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gyamkuxep.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/govltjorz.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glilwizoc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gwpiqnxcw.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/golfzwmle.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqmoepzt.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/garpylyhv.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gehbpblto.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gfolxqqxy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxbbpncs.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gtwqooinn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdyqlraj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gchnaarje.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gexfozejw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glitbjvfv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gjkrdlkfn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhalqfcz.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzeumrii.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gblzvsmmc.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gknwudfqv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gguuvgtsd.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gilcjmbzk.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gcgrlftbv.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gmkicleob.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gfqsqhbmj.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gnsrzxbfy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gshdaevsc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/guhlemmix.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gcarmpnzi.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gzsivpdsb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmageviqe.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gofxjhzsu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisnxfcgb.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwotczcrt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwortvjyj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gjsbolhnt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmjoqsrj.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlqgzyix.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrzmllvd.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gwhsvduzz.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbqmduxc.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfphhpkw.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gytqsrylp.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gmlvteerq.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gggwukhqh.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/glwarrtsj.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gtfavpvih.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gubecunfp.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/guobfkpww.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/glznvoffk.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvelyejb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvriabbm.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gerxnbici.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gelfioxpw.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gldkpituj.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gkksjcive.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gpfjgwzry.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyculhcb.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gjklhxvrr.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gqovlnunh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhzdidmo.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkwbakzhi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghistimoa.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/goehkqbzi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gwjljfiyi.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhbdwxqa.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfybbbcet.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gbxcmfsbk.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gscjogmra.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gevzhmneg.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/guwhsxbub.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ggmeboqww.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/giqxtahra.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gipumtcdi.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gscydugsk.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/guyszgkcq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysboeyvh.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvehwvuka.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmotyihph.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblsgbsnk.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gzotulglz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/goqjebmop.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/galwkdpfr.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gyeximhwf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gxgfgiizc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljoybnwl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdacuwhj.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitromjqz.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvufglfnv.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gxwaljara.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gckjwggyz.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gepkxabjo.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuajhgjo.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsocswbvn.sHtML

string.find(s, "%d+")
来源：http://3g.fanxiaobao.xyz/Article/details/ggujmtimi.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gtltdoonc.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwoegjsh.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbopuxrs.sHtML

print "Hello\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gtrnlctky.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gavrkkqmm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaikbucwb.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzogeuzbs.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gibahadts.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/ghjgpsikd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdiocrcw.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gwvqffozu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gecabrquv.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gzxqdfkfq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goarrnpcm.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjytmjcj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grsuvmubj.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/grudgeorr.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcoxvubg.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnzvpeij.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeorowob.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gehjczbvd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gpfimfyrt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnxcytlc.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/glpjjyslz.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnagvcahp.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guasrhawc.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gquhxkvaw.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqpfmpvn.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxbkcgtr.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnhsqxxe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhkmcytt.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrgfsuii.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grujaqqnh.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvvdmhkn.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgnkeijv.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzinnmgt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlhtmkeu.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmplidxx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/glojqhbzx.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlbybxxl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsawidvzv.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevvbexid.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/grtnudshu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghywyblua.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjigdigf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjfauxtj.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gobpdqktw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbgiwqcv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/garftynix.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggjjngzta.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqqibfeb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggovfopde.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaxxjdvz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gizehmzaw.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkwvmrou.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/guighmtoa.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnltoksvl.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrcreygt.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvzkfnyr.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/grcewhvaz.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfzgwzrp.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gppsrlhvu.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gszcwvvpz.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gdjicmyjy.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfvyuzxz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhlxsrib.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggynkffui.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutcupcje.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/grynmjqac.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gutcjzagi.sHtML


<!-- 参考信息 -->