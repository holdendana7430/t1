代发 wailian999

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzlbmeim.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gealprikp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhjbcskc.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gftoyncqp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbzgtrzm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/goeyofdqm.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxbqjgot.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdrdpulz.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gheppizye.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gggvbdiww.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxwwgkzk.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gahjeiiun.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkqkkqfoe.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnolcpqdh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gldodqaxx.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmzfkuyj.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gwrirypyu.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgoyzhjg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gaigqdaxx.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gzayervwy.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakxkuctp.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gqlrubzdl.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpyiotce.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gqzogbswg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/ghfknnalt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfguoactd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghroeoeww.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gaemyildk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gqkvrwdci.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpmogeed.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/grihfycvj.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvgdhygi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccfoblsl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/grshajwst.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gpqbmlnzr.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnofbvwh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtgbsxzo.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gasbbtxes.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/genajxuli.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gqndwbuud.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccfqaqol.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gaxdbialu.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gdbqosfao.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxbkbqot.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwymgdybo.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/goexqrkag.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtbjlmve.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/grstkjfnp.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gojepcwmg.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhsffojg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbmxqzrw.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyamscje.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gdhztmthl.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gknvetvno.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtniiandl.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpdsbkmi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpokxtde.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gdbchebwo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gqvmsbbgd.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gmaleiypv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gunuuticc.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlbnzhgi.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/grebydfet.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gkuqifmsq.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzjvljfai.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvjsyvtr.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvfwpqki.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgongbtr.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrlohrzn.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzysnicha.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjtkktyj.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/ggwjzqmoa.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gwosvlvrl.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gzqnkxhyg.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gyfnjvlrr.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqbcxfbxi.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gjxlgnigx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqqdaepn.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gagepbpob.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqynukgs.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizjubxvf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsbjuzsa.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gemeokfss.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpdrrwwm.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdeevqqd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgwpwwtj.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gphbbewcg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gvdjayvfw.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gyyqbwbib.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/grizizvqe.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsgggfwo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeyujjfa.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkfavxsc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrhmlhdo.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gkrscqbga.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gwekzllmo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyshfsss.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/glwtiqhqj.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfkkbvjdc.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gfzwnwkiq.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gdqlvjqgj.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsffwhked.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gqtlhwmrt.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gffgsrcjw.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmqpllqf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemeopdgl.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gjurieghi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlnludxy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gkohejltd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxgplmvy.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimgilgym.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeyvbszi.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxphvnbd.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiysnunn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktpydvmf.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gjnmusjyb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gxahqllmf.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdcsvnmu.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcthyhovv.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxxuiift.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzssuuxni.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/geggypijw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gywjisvia.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gvhrcobjm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdodqnqzf.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhxatxsw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpshpiiza.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gpkshqblm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgmgqpzq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggebfwscy.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/glrfykomo.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/guxjjbsxx.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gdrmnofbi.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gswegnihh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/goxevovar.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grszuqdtx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrpvugjo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gecjsleid.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcvknizh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gizauuutk.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gjzfcfvmw.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsizeqzfx.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggxbvqcfh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gpudjkclu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueteijsk.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gakueewkk.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgqvpvhc.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gytjxmdwa.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gdevpomms.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsbfgnsz.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfgnizjx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaatsrts.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gptikzkwi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrswkelp.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfplpyau.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdjmioit.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/grekohwoz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudikloyh.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gonmymrgt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gdbrwwtsp.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gdihunrrr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgalzdlb.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/giqqrhawb.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/glsmyuvls.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gvstvhbnk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gburqbpoq.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gbbqgailm.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvadpsfy.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhqszsis.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfolaxzn.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmemunmk.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpvgtktf.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gucehhxgd.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/goldywqkk.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gybtkjdpk.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gtcobyoke.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gewwwkzuq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfldxouyf.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gqclabqfc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gxoluyvgn.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gtlvdobiw.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gbepbzmeb.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrxskdpo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpxkynfkz.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsowvuqog.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwhkwatv.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfdwylaj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsryeytce.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghshqsocu.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gkbxgcmea.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/glgjbnzrj.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gboyfkucg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxomdokgu.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gjqsmqaby.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkguaeqf.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gklhtifca.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gceprrkns.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gupunyyaj.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gjhccmqtm.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gbnxsowqu.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gutusztyq.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gclaxiyks.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwhwkwhz.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcixkzkke.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdtniejv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gsyhypoqq.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyggnvsd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbelkmch.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviudbcne.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaahjbnp.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgdnjxwu.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvqsxyus.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gdirltfhk.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gyyximdwb.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsvenldp.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gksuoofuh.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gcjlmseri.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyratsct.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/glsdfroei.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdkjkalq.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydlqypsw.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gzmqxdabf.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gjzvpwwbe.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gghcddtmv.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjplcwkft.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gcgvvkhgv.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfdlyavs.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzhxtjlu.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/guajzofde.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaxnwmuc.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvxnfxyq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrenoafk.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjmtzewa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjgfapyi.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlhlyajf.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gkuypyjtg.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwmdyvxb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guszkmbaw.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/goxasyojz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwszzbnp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxknemjld.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfaydgja.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/guymvnpow.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gquzjmkgm.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdoytokp.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoikzcdl.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goexnvhpa.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjguiasd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxufkkrpp.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhedfrfe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giesidhwx.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gslwpjwwx.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlvhuyrs.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gfaccvizu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcfwtnev.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gwavbbwrn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gulfkbgdj.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gizijqpfm.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gobdslhip.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gosehylcw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/gxwcbrkjt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gltfsvola.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjdbadhv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjhvkuksz.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gczvmjnya.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gucmezhpf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsplodyb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqefzjbov.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/ghizeagcb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/grkfkdocl.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gfbwajjxg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpklsdmn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbwqespz.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrfdvuko.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrjdnejm.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gohdjtnse.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtkslhnb.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghumgvhse.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gdethnefu.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gqyybmxhf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gugpdjxnc.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkswqylkp.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbthunvr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvsnezac.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gtbozcfyj.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrugqnfp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/ggxteiqvd.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyqyadhl.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gohoczpdq.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/ghehrcpol.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/grpghzmts.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/ggwvpgcgt.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gxidvwsxh.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gmfwqxjdg.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhtzeshr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgnexjjq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptnqnsdp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gefrededy.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gikonpzkt.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyhvcmqs.sHtML


<!-- 参考信息 -->