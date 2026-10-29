代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gqlgkpctj.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gcbbdozld.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gcwhvsrvp.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gjkwyvfsn.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gwipadfng.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gbdbsyhfy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/ghkgvaxce.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gapsotuua.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gbjghqyzx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gejgshhxf.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gcqwpnvaa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnwisqaib.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/grynbouzt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gixtrlgun.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gcyuntspx.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gmgjzjuwi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gijdvvozb.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gcxyzcyzm.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gjftngydq.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gwvdqlvgq.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gegcjxzjs.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/guweirtvr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gprbqofmi.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gxymbkwgf.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gtxuzxvyp.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gcslprqjd.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/grejsgzen.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gehtiwtdx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gzykclbeo.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gyhjeppot.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gehxnyiuq.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gvrqahdlz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gpaugkevq.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gxwszthdi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gylhxwltk.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gaukxrjal.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gknwchkcr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gjyxocrbd.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gpvbtuwer.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/grjyersxe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gymjzldwt.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gwfsajbxu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gafnqjcks.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/grlplwiyj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/ghbseewvc.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gjowkkgsj.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/glnnmqijb.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gmdlxlvgb.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/ghshrrxqe.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gjqgihvnf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gfkagqncp.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/glfgcjmil.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gjzkjmmll.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gqibfxoct.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/ggnxikxuf.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gzfhftqoa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/givueszpu.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gxafwebnu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/goxaonzdj.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gsjjfoioj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gsgxiqslt.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gesxxiong.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gkceddpet.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fehbvm.com/Article/details/gswvcisis.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/grrpuluby.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gzzvoghbw.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gnztfsalo.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/goxgymxku.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gvysftzxa.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gaarscdma.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gwlksrgsg.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gxqwjfeeo.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gklctfxcl.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gtbxsvvbv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gzoqmitba.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gulhyjfis.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/ghivivknm.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gwblbekfg.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/geobkddaf.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gpegeetie.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gvvrimffj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpcrnydkv.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/glizkeadk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gphgqsefn.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gazmfsvei.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gbqwuehdy.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gpfjsqrsk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/ggifraoey.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gycdgqvzw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gvubxrzom.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gxrewtkno.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gsbvimttt.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gfnoxajku.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gzqxjemtt.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/ghkrsnmgy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gozlbqveg.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gynlbrdne.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/galopvhzp.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gonxmmwpb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gaqtranan.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gmtoffidn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gynnfjkjt.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gblmtftsy.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gjpbjxjmj.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gxzpwbyhp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/giozpzyux.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gyvmkujdx.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gfatjlhqt.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/guaelwwcq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/ghdrefkte.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gjejijrlp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gxqggwdit.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gwizawqdw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gtlmaysll.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gdrixwtif.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/ghshswrqp.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gfbgumenn.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gdqffmces.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gfteurmej.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gevnqrcca.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gsframsrs.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gxlwducrf.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/goeavypoy.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gofpchdoa.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gyqaibvtd.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gocctovnn.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gkfnfxavs.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gupxahbfa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gkrpbjsmm.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gdaegcprr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gmwhgibmv.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/getbscfxc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gotfouzjh.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gbovyhlgd.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gekpgftau.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gfircgqkl.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gqcalbbbd.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gsgrjhyuk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/giengezqa.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gkgsifyti.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/ghepssvfw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxpnoygmy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gpwuidwmg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmsamonly.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gnkcxgafp.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gjfqcbnou.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gcjwaenqu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gxliyvtbk.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gnptdnuzg.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gxzgwanks.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/guqxjvocy.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/glrootkuz.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gurldwteq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gskuevljt.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gnpyqgnfy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gsewqemno.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gpbcipdxz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gjyaazawf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/guntpgtlh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gwsnmrzuq.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gynujiurc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gtebjatrj.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gzgiruxgp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gfrjpndkx.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gxwysknhl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gjjxglgga.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gveydltfr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/geppjnvqh.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gihwickwv.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gglprlsqr.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gdbanspak.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gavbkgzup.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/goshxgqzc.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gdmozdkan.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxxagezjp.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gylldvkjo.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gzfkhbvec.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gkraamqrg.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gzntvhhiz.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gujmhwmle.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gfpjcysga.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gjmyrnyfa.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gsgiwhvqs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gdnjcbbra.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gifuxjlaa.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gqjjymlii.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/grgbdxaau.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gszgblssk.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gzpkffsxq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gkgyqknwe.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gvdvsgifi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gjoidygnl.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gnlfgjsnu.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/guaamdqve.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gtzacfsha.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gqevojkzx.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gqxwlzqcp.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gadiainbu.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gdumqzmfk.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/ghhetndnh.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gewdkchzm.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gfazomckg.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gfavqkzcu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gwllhnrpe.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gizaupvyz.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gtbccmlqx.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/ggopftyco.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gafnsfmbl.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gpxhmkinl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gbayevhtc.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gbkeitbbz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gsugmcjfg.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gkqnsymto.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gyoycyeqg.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gmmlmgbqk.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gyzjtcybf.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gpvzsnnym.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gdtektzxk.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/glglmryxo.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gpqzijdwx.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/guianbgii.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/ggqjeqbki.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gziufkopv.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gwhlgnaem.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gjknpqrsl.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gmfyojxcj.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gtjjfnxjy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/ggytoiyvd.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gkygzkbox.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/goaoojhnz.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gvtwutnfs.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gvczcqveh.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gfyowczxj.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gkvwruysq.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/ghtdmthco.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gbndldzix.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gmvtnguey.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gccsnnjgu.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/geufxxsyi.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gdjpjcyxa.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gjthqxhzf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gahqebjuv.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gzmghjami.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gcgzircoi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gafhckdmo.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvlwtmrau.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gowdkzzmo.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/grokybgxn.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gnldnxuti.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gafjzydxe.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/glgtkpaie.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gyuoyylxf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gejaeqsfs.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gcxeigmue.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gqdiqfbee.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gfcgeuoqr.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gvzewglfc.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gpbbkzpwf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gyoltfoys.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/grnukgpie.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/ggoucqhni.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/greemottv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/grenjvjgq.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/geqzbfvhz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gywbbxxoh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfcazzxye.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gichgjkfq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gckalhlfr.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gupljorpm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gfbqpmaej.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gbwjkrhsj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmqjhabin.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/grbpxfjak.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gzbabzokt.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gsgtipbtw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gxnkvygwq.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/ghwmvvsjg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/goomfaxdp.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gnfhnmrot.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gmlkfjdnk.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/grxedohtd.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gyoblfvjd.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gtcgwcojc.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gacedaqww.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/glxmzswti.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gqybwjfac.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gxxmyiauu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gutgaarrc.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gmrvqovcs.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/getnslczt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/ggstcjsdc.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gfctvzqbp.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gjjfpdgiz.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/giarkhmli.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gdabugofy.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gxvyjbwai.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gezmrmjsy.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gycpbadob.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gglphbzgz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gsgenytjg.sHtML


<!-- 参考信息 -->