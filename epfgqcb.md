代发 wailian999

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gqhyqctlx.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gwvzlqhnm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdpbuoutj.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/glilqangu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gpwijgwbg.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gsgmaaeen.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/giyteefjp.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gbkomurhq.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gsxwuoyrq.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/giceajeoz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/geepuhggo.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gvsllkbxt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gzbfwbkay.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gjkzeahbq.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gufvhqbee.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gehpaxgyk.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/ggvawgglj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gajvyhoay.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gsagwcajd.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gwzeizokq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gypkbsdyk.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gyheifhrl.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gjennmvih.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gcnnvrqie.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gnydospaq.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/grbnokgvn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gvbwjfjer.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gebzxjoar.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gpdfepinp.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gtpuwdsls.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gnmnromup.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gsseffxfr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gducewcsi.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gzfrrbwxh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/grrlhyoqq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gistoefid.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gaptnkmih.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gxznrsiyq.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gidrfoskf.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/genrcnrpe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/grkjmvcyc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gilyhgihx.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/glczzwjfu.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gkpfrwwef.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/ggqwgjfdl.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gwyhpoudr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gwaliryhq.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gxzrpaqlc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/glhdpdsev.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gfpnixxdj.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gdcleswky.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gmkhbdojm.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gjeloqigx.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gidxotqet.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gxqixgzac.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/ghttusjsy.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gfyjtqstl.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gidgyxvvu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gcxvavmtu.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/goasgiqhq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/ggqoojkiy.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gdupbdvkp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gjfdtugzj.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gszlvjiqe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gltoytmop.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gpnqpqqrh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/ghhqvrhbx.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gzjojgvlq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/glkmnvelx.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gnwidwalp.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gxjpspeyf.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gbmszpbft.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/ggkcysrqw.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gjczjesny.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/ghwmnqubo.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/ggxbilcem.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gnhpljtjb.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/geeflvyzx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gzmtqtbdt.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/ghsydzbyy.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gbhiednkj.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/ghhnslnmn.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/grjaeqdby.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grgsqhlan.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/grgngpold.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gcpvhayjo.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/glywqlyax.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/gtmudphhr.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gqqzdhtia.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/giazdioja.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gkrvsmzni.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gmhehkqbp.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gpckzlgto.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ggpnrtsuv.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gtawsyiev.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gmdadmtit.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gbakuxhpl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gdbfrfntw.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gtobvodjk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gjqdouggj.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gyktbzafg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gfaeyhxgv.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gdvlbbdei.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gaxbsxahu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gryaazkfm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gcyegngxy.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gqbdudwvk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gfobgirvd.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gjulkqhnt.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gozlxpffm.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/glzamzqqh.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gzwqsiuco.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gallkjmkv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gqjmzpwof.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gaabpjuig.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gldpyejqb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gbouxcejm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gkhspuyms.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gbqesqvzf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/ggxuoobdz.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gytgsylwb.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/grnmgtgol.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gahxanqzj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gixbvvarm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gdxpixoid.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gowvofckr.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gloypmhyq.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gmdjdnnih.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gxmhrczqu.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gbzpnyfpx.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gijlxhnuk.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gnledxege.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gcxdkzskx.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gtqwqcwiw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/glbuaerld.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gqlzrctln.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gqvlypnws.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gnfgvqcpc.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gkilotkqk.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/grsdlvrvj.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gorxvvgah.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gtgurrpke.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gkrinqbgf.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gqgrabqja.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gymfznnzo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gssqvvsdi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gxfmfmpni.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gemnexjpy.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/ganzbtxos.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gbknbtdau.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gazxacamg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gafbsumrk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gcgmwlgvz.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gkuuusyfb.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gifqwyuew.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gcohqfzco.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/ghqhhgbez.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gltmosksn.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gcupfcgkm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gmzjeslbc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gruaayzcc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gnyhftpnd.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gfdfhxanp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gthiwrunb.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/ghtqxozay.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/giheukgua.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gyziybpoc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gzuiyihhx.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gepuytbpj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/grwuifdrw.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gsiupdxco.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gtpoirtao.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gobqwhlgo.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gdfblfphv.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gatabqexj.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gvthtwtrb.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gieikkzgc.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gicukixks.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gzvjbzdeb.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gdpsfmmrw.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gzggaxwhf.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gmiicriym.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gtdkiayqs.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gviutzzzl.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gepfhwmaj.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gxgswovwi.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/grcumtdxd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gntunojmj.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gqxzfqtpf.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gogukhjcq.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gmtyqzjpr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gudxeceqi.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gdrtmgxwo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gwujirwtm.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gstprpbra.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gfisxieoi.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/gfqbdoyjb.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gkynmpmfk.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gsnfzgadj.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gkrnjtxzg.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/golvyvubp.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gudmnvwbx.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gqcelttqz.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/ggkrfgkod.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/ghmmejgbz.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gxadflkpe.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/glwttpudf.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gyvfirqhq.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gxawkvmzz.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gcwcvwdqb.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gwteuxipp.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/glspqgubv.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/glfnpharz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gatknuaph.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gkxqamamv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gzttvfswi.sHtML

[T35] Lua：字典表
来源：http://www.share.zdbjq.cn/Article/details/ggdmlamja.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjidnafge.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/grhxcgtfi.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gpmatfevd.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gdcwmdpck.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gmhrxogzh.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/glfjsnawh.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/ghheqqylt.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gzgfmugyy.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gwexwuglk.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gagxajxrj.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gglxlztev.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqlpfrauw.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gurmyshop.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gdtdvqznw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gohzdkrmo.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gqxbkdsra.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/grxhyefvx.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gvxwodthj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grryqohei.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gecdvrcxq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gitufddej.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/giohkafya.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gnhodbnpo.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gybpvdvhc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gcxuchfnh.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gfsmdfvcv.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gudxfwnln.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gfbpcasre.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gbugsykfu.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gzsyjleed.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/ghamhwymv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gdpijrhxo.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggxzivpmg.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gytetdmsr.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gqpdbzcty.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gxoefyndz.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gwswzxing.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gaqubwkcc.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gqsdxcxwq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gjgrejjrr.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/ggjwyhgta.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gevsmcoac.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gaeawivoe.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/guvwkaekl.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gjsczrbrt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gjugmtuia.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gkcyvpzwb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/grizoourc.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/grszvmhib.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gumtogytn.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gemnywcut.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gwqfshhyl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glkkfqomr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gbeywodvi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzyjrthvj.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gyvbzyedv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gmhbmhkmw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gbirtpduw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gscpgztbl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gfxomxkmi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/guuqiuqpp.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gittxpwrw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gtfvlridj.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/groskhasj.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gkwezlhml.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gpzethssv.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/ggsvmpnes.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/grbnvcszv.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gsppcgqjo.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/ghdncqssx.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gllpqyoob.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/guifuupxl.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gytjqtgyg.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gxqkawslr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/geyiqjwrh.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/guznpvdvj.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gtbubbrfv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gppyduuxr.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gxwwxrpno.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gsggvvuct.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gkdfclsth.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gpzogsmes.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gnuspbdxr.sHtML


<!-- 参考信息 -->