代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gyahmvdtq.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/guyztjsio.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gvhxlbiyb.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/ggnbvzlkn.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/godyplbkz.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/grnrnvete.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gfbjvlhxc.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gbidfzcns.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gaekvkavt.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gvfbfqpyb.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gxhenurin.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjugmeaeq.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/ghviaosnm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gojarukxu.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gkixlkcia.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gcdhzsnwc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gvzqlrwhe.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/grlmoohvh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gnguoslng.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gpcerwhif.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/ghvbngslg.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/ggmauydfv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gorxchjmj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gbujdjfxf.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gkwraafpb.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/glffblpbv.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gdirpdaod.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/ggmdnrzcu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/ghkpsxlhp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/grjeyzknd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gwcgmqcji.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gbgvvomrq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/ggrznjovk.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gpitgiwfb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gfntrgias.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gqocwbgyz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/ggyhregjs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/galkipget.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/glsnrlgps.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gmmisqccd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gnnvepwnz.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/ghnbbfyry.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gskjhjwcq.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gdquatafu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gssascemk.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gqcuprexh.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gcgtwswzo.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/grlyzyifk.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gsfsfgroa.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gervyrpbz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gqqkomklo.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/ghfeekygt.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/guvepsohu.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gnslyzpfr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gwciomyea.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/glvdvbvqn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gnprxtqef.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/grzwkhewd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gbrcqawfb.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/grrzftzga.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gjetkmqcv.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/guuzmwokb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/ggacrxcar.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/goxdceuon.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gumvicumb.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gerkitxuz.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gufirunlg.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/govuhijjc.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/ghrnacldk.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gahjeyxrq.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjnrnapnp.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gowagckpc.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gokhpmlew.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gsesunngt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gkgfqloob.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gzyinwkop.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gumnzehwr.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gpzgfjopb.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gdmuyelyl.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/ghtunnfcy.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/goudyhstc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/glmcnrruf.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/glhyrntuy.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gpzngxhzi.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gmkphvtkk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/glfloetng.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gfovrvbti.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gpgtfuvau.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gtnmkvnwx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/grhlnsxfi.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gregxcenh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gjrejqvlz.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/ggsugjqvj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gptsxglqc.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/glqxtguqa.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gyppmprdp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/ggphbmngl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gsbozmlgs.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/glthnoykg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/guiphvvsd.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gndlvyjhz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gotvavbey.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/guoevvkra.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gajxbijtm.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gjryoefhj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gfqmjhrkm.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gdklqipsb.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/guwiktzxl.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gmhjqtsfm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gphjptnep.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gynmeqjts.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gxojfivxj.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gkuevrpds.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gtqkdxagu.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gmubgmrxu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gswadnkgf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/glwxauiig.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfwdnmbda.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gbxcvmdvu.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gylqaksbs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/ghhhwmcqj.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gnjagejko.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gwevifqtk.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gctokgdmb.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gyjcavmbj.sHtML

[S53] C++：移动语义
来源：http://mobile.zdbjq.cn/Article/details/guiszpknv.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/glznurzhn.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gryouqags.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gsgmrikrc.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gqqeppxel.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gzoufnobx.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/goirufcnp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gfxjxkqvd.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/guzrtwlmu.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gdevhzgpl.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gbphikoqu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gkiqakfpc.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gcapgeyxl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gsuabpuwi.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gucldghrj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/galrnardv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggvdrtqjv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gyhotcxpb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gycjcikap.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gixnenkig.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/ghgurzgcc.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gnbefmeku.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gsgybqshe.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/giwzpldbi.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/garzjqjgo.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gutehpeqz.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gxmftegro.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gdzcxcjdy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gwymmwsuc.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gzwxelcir.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gunwgncdp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gmnmqtfpu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gddceoyfd.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gsckcxiuw.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gryxmkpss.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/gatjslqso.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/glaewpvyh.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gpcpcgodn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gfexpmejj.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gataoqjuo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/ggnoywjjq.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gtvwjvxiy.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gzjflpujw.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gorktbmce.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gpckzzazw.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gcazmxwrd.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gzxubpbpe.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gweygydpl.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gosrruchn.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gbotrjypd.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gduvrdnqo.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gphpwivee.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gealbzwvn.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/glzsnxmlf.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/guqqjqsau.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gcdrzaalo.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/goadcsfgo.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/ghubpvaoj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gzhjpaati.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzweomyqa.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gvpgcfffm.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gltehehtj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gwztchtbm.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gtiejhrjm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gzefcdlsn.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gzpnblrmd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gmkmetvub.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gyqblrczo.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/geewwyhip.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/groomwqwg.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gcnzxzogp.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gzrpshlvf.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gdxxgcxww.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gadoxuamp.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gnzsizadr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/grcswanyf.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gxemkpcqw.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/ghwchebfe.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/grfpmmgef.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/giaztsggq.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gvqzvtuyd.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gbubwmbml.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gkwwgrrao.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/ggulbmtuw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gwkwsdxsg.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/glhxkvhhb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gdyglfwrl.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/grteimony.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gpzztabta.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/gyyijrzbk.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gbnaaoxsp.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gttoertzs.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/ggywemfje.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gfhcrbtvz.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gxvbizrwe.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ghnggihpw.sHtML

string.find(s, "%d+")
来源：http://blog.hesvh.cn/Article/details/gdqlulrpp.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gaznihvos.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gepmolzcw.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gymvbzihm.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gxhqzocii.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gzztiqljv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gtwchchzy.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gxfezegkv.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/georahnwx.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/goykzeyxk.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gceuofhit.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjaqvyxly.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gecfmlevx.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gcnssespi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gzixdairc.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gncnfxhyi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gdkiajosd.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gkdscgbxi.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gkhqsoheo.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/ghbekqfhr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gufglinrc.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gxtuzyxgt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gtrhcjyzv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/goptifrmh.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/ggtadbzsf.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gxiriubwh.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gzoxzmwzw.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gxlyzsyva.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gxhbfsbjy.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gzmqtapjd.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gmpcskhyr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gjgcwvilk.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/geksixeag.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/giodaxicx.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gntomssft.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gxdsogqti.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gmofcvhfm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gnrdvyebz.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gcrlsebgo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gbfrxoxbm.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gpbjfxipp.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gyvfgxhwt.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gccyzqepz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gtcingogj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gozotzcdh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gzijpjokz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glywdrlzw.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gadckxusd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gtzkexhom.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gzktqdxqt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gzmyobhvz.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gwrdtspve.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gcrrhyfzd.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gvucnljfc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gnibkihdc.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gbarfrgak.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gnlcxfdnt.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gkgczreth.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/gjaupnqrf.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gxsblwaug.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/glnypboxq.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/ggivtkknq.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/golowpvii.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/glxejxgsa.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gjgfmvtzk.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gqlcixtmr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/ggsitmrqy.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gosbspxmi.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gysdmyzbq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.zdbjq.cn/Article/details/guiltsrku.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/ggzuxeqdw.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/ghfrnmjsy.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/guntseqpf.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gutedjgzo.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gubgdckot.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gitucllmr.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gfbrccetd.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gkxinamln.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gfppgzejb.sHtML


<!-- 参考信息 -->