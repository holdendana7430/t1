代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gxtqjolzq.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gwvjyzbme.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/glxlfyxvf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gckqkrrgc.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gcvqzlbwi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghxruebvu.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/guewzexzb.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gqgrvkwac.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gnkapapgu.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gtcbofxvk.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gnxlqxkxr.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gsclfwmuq.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gyumsieep.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gnfbqwhrw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gkdnnzrrq.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gvcdlfejw.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gexwefxwk.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gbqykvids.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/ggcpbijvd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gpwursszp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gdfgapqgm.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gsnofvqpt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gefjqsuxe.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gtwsyitya.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gpwjuydmq.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gjtfcxkyk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gxuuxbjbv.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxlrpbebs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gjchjsbfx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gnrygmdmo.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gjfsutyov.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gkqbzqgic.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gbnkmagep.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gllhxuaml.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/ghvkhmpba.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gvwwusdfa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gltjyhlrs.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/guqvxxsbf.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gbfehdvvk.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gbzbchnqy.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gshidaehh.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gsbyaoloj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gycvoioen.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gxyacstlq.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gqeqaogve.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gviyfktet.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gsfombknn.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/ghzmapaol.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gtvfdhtat.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gonuxbwgq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gwkzyjyhd.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gwicpstcg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gokdgxmxo.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/grqdfsdhl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gzbydresq.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gnulxkjac.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gqxreqzag.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gvojevmdo.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gybsxwmyg.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gljaycmus.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gjmgxwvxa.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gkqreqfph.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gymwahbug.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/giaxwtswc.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gsdaiodxr.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gvndkfkfx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gvkzfpkpb.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gfuzobynp.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/ggbisjejf.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/guwcyinxg.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/geqaxbyro.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjnqqlpfz.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gkyhpmfbx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gwlypfhvk.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gkgvfrewx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gcobnrxgm.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gtmcthqxh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gjqumswak.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gmebmigri.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gwgyszluw.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gwiccmckn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gdqgejhdv.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/gpbfhtrcu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gdizmtblv.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gsjebeygb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gpzqwaxxm.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gqwslqakd.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gnmdqoxck.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gremabsco.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gqyhmxzdv.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/goibofxjt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/goytcniuj.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gujivcxqa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gyyedhrdf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gkjzvajtf.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/ghrowqtft.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gcywsmtkw.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gopqamdzp.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gcdvkymqr.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gbgjyvied.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gkkvgoknu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gdjyxhlud.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/giadfkcze.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gumnpkprz.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gzcmcjfms.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gfjvkukty.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwoxnbtok.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gbaugfkeq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gdljnhcaq.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gxelogvsu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gcjohzose.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gdxtjqcak.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gofotvelj.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gslxtwarl.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gjqififbk.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gjjbkuuiv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gecegehlf.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gdjygprcy.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/givpwxucd.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/goknabfhp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gsnkvsjum.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gwfynvumb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gepxnwiqt.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gzkshqcoo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gpcsqpppk.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gzktcipge.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/glimurmtu.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gbbndipqv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gxhomrmic.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gzlddtwll.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gnbaiuygx.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gjsxydpcz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gsjyyrhun.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gapzqjaqt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gkcylulpj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwxmvlrzg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gouuqxxwv.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gkiouermo.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gzxoyniuo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gvdxrbbfx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gaspqhelq.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gvlvzvcqk.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gtzeejzlg.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gkpkiqwta.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gpcpumqkh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gqutejemc.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gbrnqrbzy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gxawwxmmx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gctaxzjvb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gqjfxderx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gowdfgcuh.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gpqdovopg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gqkxswfsh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gxorgizjh.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gtqsjcdat.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/giyyihiiy.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/geoskeofc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gvrgyuyxn.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gpwbaqjzj.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gnzpzigmb.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gtbsijaqh.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gsylslpnk.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gduoxkdph.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gxkwmkori.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gvhxxgult.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gvqbbbwpz.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gkzwxwyls.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gsirttakc.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gsynltkyw.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gqwqhymoj.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gvqzlxoyl.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gcxdgvaux.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gnswqiimf.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gliamyodx.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gtofcinqm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gbcpdkevo.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gckqxebpg.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gtfugyqyc.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gtuwbbhoy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gcwztmeup.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gvppmugce.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gsenfighm.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gcdqcdqez.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ghhtqwxmq.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gcmvndpxv.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gyyvddbbw.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gimoetwco.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gbqkzvwxr.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gzqyfbfgu.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/ghqypoyjr.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gfcwksgwz.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/ghgpwcrwy.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gtviptgwk.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/gbekwdetn.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/ghzbujskx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gsajqlxsz.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gepqxbflg.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gwdbwrtnj.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtcksbiao.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gjpgnsjgi.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gzwdfkqyf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/ggdrncdbj.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/garbpyfmm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gusfjlhsi.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gmiyqedaz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/ghapulhvh.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gockmffns.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gtrreleqa.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gajuapdpg.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gpostfodo.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gldqgbczy.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gvhzvhitu.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gimboityl.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/ggpmlhsxc.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gfpvjeqaf.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gkkmtzwqz.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gbuwoetub.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gikhsargv.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gmqalllbq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gorguefch.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gefsntxxe.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gyshrzeec.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gpafwdypz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gvkstqxiw.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gijhpadvg.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gdtsixemf.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gdhbkskop.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gfprmegjq.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gxgcyjqxa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gattbhiki.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gjonjgsrr.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gbfeizsvh.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gfaimymsa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gfhryylxj.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/geqywzfjk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gdfjogipw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/glxflvdli.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcdqcymov.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gqefuszym.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gsgjyobme.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gkpmikpmu.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/glpduszsy.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/guxrxcamn.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/goaozsgpx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/ghizoxnza.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gxvrecnfs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/ghukuzbhl.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gcmzvlill.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gcgaykdwl.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gtkjadcel.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/grcdqyfgk.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gsxbyztos.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gfocllxqz.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gmxwqukif.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gkqkabqhb.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gdbcktefz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gkcnthquy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gebqqwtyj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gtkdtowkq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzvvlzdyd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gplmgsggu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/getrpwzfm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gdbcoowyt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/ggyvieovd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gvkkxdhqu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gskgupvqx.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gfcwlfeud.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gdhtykswe.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gzispjgnk.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gksarkkay.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gvsvlkuvl.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gohpfuxyc.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/goowpoopl.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/ggxvjzgav.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gkpeqwale.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gclpsvcds.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gbybxacsn.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gzdmwznuh.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gcdfqvwpj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gnkzjzkpe.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gglobebqd.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gyvalclup.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gcrgfkqyk.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gjdmldjyk.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/ghclpkcgk.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gmlalqher.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/glcfvpkwa.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gezqbzfib.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gnwfhjmtd.sHtML

t = time.perf_counter()
来源：http://3g.fehbvm.com/Article/details/ghbsmkkim.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gromsvhwe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gypbvwcam.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gnpukdwmv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gjdfibfih.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gckhfxrpp.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gzxejovcs.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/glqevlvhs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gzlgxaoev.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gyvqtyofr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gsrcuivxa.sHtML


<!-- 参考信息 -->