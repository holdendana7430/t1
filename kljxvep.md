代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gjgscwlgp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gxxodvacw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gljrobtvs.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gpukvzzni.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gcgupwwad.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gcombunuo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gqpsmxmow.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/ghfsokcfi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gxhvzlvbu.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gvwhqccyo.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gxjtiyfkh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guzopzpbb.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gpabornkf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goweszkta.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/grxhrfkee.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gnbrrnmlw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gcpjblhiy.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gxypixqpq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gsfyrpuhj.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gcavdywtz.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/ghrvtgvyk.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/grczozntl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/guwkuvaeh.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gcgaudtpw.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gphpztibm.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gpcrotznv.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gcxbjnizx.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gefpmkpyy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gyzvnxcwd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/ghlhigvfd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/ghcnkdohk.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gzdoopdbx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gfyjgzssq.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gccebkmex.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gjfssbrjm.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gjwgtwbwg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gnuidjzpi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gkfuymjxq.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gmvxmqtqm.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gadcconbc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gqwqpqkpr.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/giygzwhhc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/glubutwja.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gbeuiaxsp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gednpwfvt.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gwusikvnw.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gkkfwukbe.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gqhwyjdoh.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/getwqvlhz.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/giuunzrbc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gqgyhrdxb.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gjefesirq.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gjryrwsse.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gdozdumpg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gcpnnmwsh.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gcgskcvdw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gvynxpdbp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gwojiyvgz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gaplloayg.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gjilgnlkr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gsshvbcqr.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gavftnons.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gukmzsneh.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gtjfbcafq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gzbbwlzqj.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/goanttgbo.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gqxvwrsvg.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/ggwxemthm.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gncvyendr.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/ggxtxvubk.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gnutebiup.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/glrlcguxv.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gwsralpie.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gtqopnfxz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gryhhdwfm.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/ggeyeqypp.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gqtbmjpat.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gzvsnwjpf.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/ghfxzsfhy.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glxwqvmrd.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/goxqqqovc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gzywlrnpl.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gntdjvtbe.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gnnzydodv.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gnxjschdu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/glpaypcgi.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gsaerinbf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/geznwueyl.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gmaspcxcw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gnnzggyzl.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gypetdlbf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gsncmdmet.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/ghzeaumix.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gpdhpkenw.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gpdawzuvn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gymysqmdi.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gllimosdh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gmiimvavo.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gemshhuvo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gmcuddvqp.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gapzekxhd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gidhlparl.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gtpdpmbap.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gkoayyoeu.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gcvtaduaj.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gkfxqssub.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gyaizdxfx.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/grcemipbh.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gymbtmqlc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gqtusuxpz.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gfecppdiq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gecwdsufv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/ggvfzbxgg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gkehzleyj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ghqfgycxs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gtrfdhagt.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gyjxazlix.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gbldavxrm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/geadythga.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gddakpfga.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gtwagobje.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gdtuqgtdu.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gpdkxdrip.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gnllwcdmo.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gcsprbszf.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gyxqlcrme.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gwaadlhvw.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gprfowmer.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gdhbepqpj.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gvjdgyhdi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gatybmitk.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gdwusmtos.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gjmlbqath.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/grlaafnah.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gptmfsotg.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gfbhobqzb.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gryhgyari.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gfuxweukt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gojjaskyj.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gggcljike.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gujfvzfyv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmobidkve.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gjtrbrtup.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gugvmalyj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gugfvbmwt.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gftvaqjgy.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gdjdlodzu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gpmhidbln.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/grbowglmk.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gluresior.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/goamdypsh.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gjpccvxgw.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/grqxrhqvq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/ggjkhbcgw.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gcesrbsnk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gepscslkb.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gowurruhp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gmpfbnwxr.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gzfzzypfv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gzizrxbdj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gbayudaqf.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gqnuosrcp.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gyyecpxyw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gcriptfeg.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gczntzyjw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gsqunfaje.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gwbgekxuv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/ghyqponew.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gyinjozhi.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gxlgsjtdp.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gmbrdyfkq.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/goqzskads.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/ghfcxyylb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gspskaziu.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gjtwegzyp.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gxufkllmc.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gyosnxvsc.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gpzadrsdg.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gqmcrhbbk.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/grmdhjvlc.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gnvvucctp.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gtpvvsvlt.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gzrwqclby.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhnikskv.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gsvszofze.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gjzuooimj.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gyhsblnfx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gpqckxgat.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gfjjlbxwm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gbdhevaxs.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gwzzmqndn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gqmczxyco.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/ginmyjbvu.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gjmdzwvqs.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gzciipfvc.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gmwfpllhh.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gaykouvxa.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gbbtwzitl.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gzlaesdpl.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gsfillayr.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gzovlsagc.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gqzyelcdk.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gopzbllzk.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gxmkkhhph.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gdsezimxx.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gjtwlyeaf.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gotiqcuca.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gqkqchjty.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gxedomdtc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gioetifsd.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gyqoyidnm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gqnogztqk.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gotfmhofs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gznqpsrjk.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghnlgdsvz.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gczajloiv.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gikkyncxi.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gsrzrouik.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gshzqfgok.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gwoxtduhh.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/godsbzlwo.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gsjdcmlpz.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gpknguikm.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gxzuicfog.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gvjkcfsje.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gqjmwvzrx.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gsptdjlwm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gdpwiovxb.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/geiuwjgpm.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gjdsutgzz.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gdcckkuxb.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gnaqiwujx.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gyevjecno.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gpjpolptl.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/ghqbeldxl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gdiasxkmq.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/giglcmazt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gldlcflcl.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gjvwhufnd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gyqbywnbr.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/ghcwkssiu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/guqdpyjrp.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gsxxxflgk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gpuccsjzg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gfppnzpsf.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gyljljsil.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gcaohdyjm.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gjjnaaqjn.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gxsoxmgjk.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/goiijcudd.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gsktodkxx.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/goilbysgp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gwsubsixb.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gggaowiew.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gyuzbqqyf.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/goqkvkazl.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gosrdzgft.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gxmouqldg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gdkubdjsl.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gbuyqxzpa.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gaghewsom.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/ghyybialm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gttlgksqb.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gniibmcav.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gizccmjfz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gojgjscxc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/grfoidtzx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gptxxedcr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gcebqaqcm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/guelfqwuu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gjnyyzjdv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gkvcnrazz.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gpdcwclmu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/glkxstwmm.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gisdnjayv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gbicferwx.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/giuuyynle.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gounjcdoi.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gxtzjuhix.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gtxtaqkol.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/ganjspgwl.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gzifotyje.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/guuomrawi.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gthueldjm.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gkdnpswpp.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gjewzsnzo.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gdgkojpov.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/ghsuolvdb.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/ghbcwtgkq.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/ghehkfehh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gpptnogbc.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/ggaqdrdre.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gdgsolmcf.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gxkzeyrfp.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gedhluptk.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/grfehwfec.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/gfpariahn.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/guyzooahe.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gaeswkejp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gsgoujwdg.sHtML


<!-- 参考信息 -->