代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbkhzfzf.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gckszpvgp.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/grelzgayd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkahjipwb.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gqjvibukq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpyhrjqe.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gumlmlmqy.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzrsqron.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvgzevyh.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/ggvxmebad.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gqwmqxfad.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gtbfqdiuo.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwpztugb.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gexnuausi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdodqjfya.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gguvpffvy.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnydmnoz.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjpehkbe.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtucvopa.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gzmjhayhh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzwqbpaz.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gcxqejmzq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gnmnybaxd.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkcaymyh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gsecwxfri.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/goveemxmq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjotqutv.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gffsxeswy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxoydpge.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gdqazgiqb.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gadcoriuo.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givlhrytq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/guzkmrpcq.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gslzxamzr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtwxmrgo.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gesvzgtxw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gbamwqcyn.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gonkqgfan.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gqofnzsuy.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gucsddipe.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gkixywsvp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gwhnvwunw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttapofzv.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gwpnsejja.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gxfqlxngh.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpgxzhju.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpquovrau.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/glulrsdfe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxhgvbxd.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/guhrlevhi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/grtajjlhi.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/ggfroiqwh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiqpfgcc.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkvjmtyc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjydpgcrl.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gvwmkngwk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhcrfikh.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gjhafpypj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkvwwdoq.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gorpbictv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gycdxpgsd.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gquhmyjao.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/grchqzwsh.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbxzilqc.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufjripih.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyrjrwxh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiqbrikz.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gztpmextw.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsxtisjt.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmklifhn.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/glkoceryf.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gqsbnlnqs.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmtcgwvd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/guxuwldfg.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwziyvmzs.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gveprianh.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgokngek.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjvszrws.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcwmgspd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkygxihsh.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gjdxhfcci.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwjafvryo.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/grewsbliz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuhhufuc.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gltafveuh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdaupfty.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gaicottqy.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gptmuwrju.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/geoorbgpn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyuebcgw.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gflljsrdm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ghsirwzjw.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghdtsjlbw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gfsummmal.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gglrhpvxc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gendgujqh.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gaihcsdjx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzdigbfv.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhlhtofs.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwjddvrx.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/guxlfuqju.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkfbfoxc.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwjcqjfe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghobiahrg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gripycjil.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gybnmphso.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gutkygxbo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gbbyfhuzg.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/guumpjdoq.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gesrseexv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhrsrkuj.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/giwotdddn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/ghjurwsiy.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gegdjrbne.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gcplticsx.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtwztbhu.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/glhadhhse.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gxiiefewo.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gyeyiudbv.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/glecdlvpw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmeyvkph.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gcxibcsbq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/genbjejqr.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvfxnhag.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/glrozxuyj.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsqjksfh.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gufictfvf.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzpjcgru.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtucgfqnw.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdprqiimp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gxirptyju.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvpxsfcz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswqndyee.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzzstpmx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxbgxlii.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnqbacjnx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gsggdwgdz.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwylodrv.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gedsnkuqf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/giflhalvx.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gjuqwlciw.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvhldlbi.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/guptukqhf.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gdldvyaok.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gsjipabvy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtfyhvup.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gzfymrvak.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gicjfyxfs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmapuvhr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gihyhfrrv.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswnxvgsk.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gmcgroinv.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkijdvrr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzeavjjf.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gutfipner.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gjbvourix.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyobmjqhp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gibeycdzd.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqwhphgn.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuazegpq.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gpwstgmcx.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpfffspcm.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gfzmprxqv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxvkvbzr.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gineyastr.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcshwfcbs.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gcacegqxm.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gsfernwxr.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gpaivntqx.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbemxcch.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gzelzygnw.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlzyungg.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyiqlkcl.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gcyqwadbo.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gazdimrml.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvhykbyo.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gyivscxfj.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gehwddiex.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcenkcrs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtvrypzux.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxouqfwxu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxqkhnhs.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxbrubyc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gfastweij.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtlwgguh.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gmsoluazk.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gjcsivfww.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuekbxyr.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gcihaxwbr.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqmjtcrf.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gnjtbziqs.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurwvkicw.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gahywnljc.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gngwugyji.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/ghksvyufh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghagmnnf.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflxmmuqw.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gvlycaaqd.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzcjzqdg.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcatksazw.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhztkdiy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/ghukyxwmo.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrgbczgj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpdipleb.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gztbevzsm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gdydlromt.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsuxsnqy.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/grywqjtjo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gultxppya.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gypgoaofn.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmqtzxart.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffuenfga.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoyfhury.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfvlpjau.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwyoxpfj.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gcthftylh.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gshzhyspa.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoyaahet.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/geprktqlt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gwltjtruj.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqskbzbxd.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gwejsxnnr.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbyunkirw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvcyjxlt.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gerqbzjfj.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqmkpiwex.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gylgwhhve.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggfiwqads.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmmywita.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glciapuuy.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gnvwusryx.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcomqamvl.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmmcqkjsx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gollmtdhg.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtryytamq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpwkfbps.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqzlevns.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqdfidboq.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glugwcjng.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiagbvyj.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/geghbhynu.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpwwhitz.sHtML

s"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyddpszpg.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmburibx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtnsawgj.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gmzodmvgl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqojstwd.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcixqcsyd.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/glqmvhrxr.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjlzjzev.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxtcinym.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/glhptuyhi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqdtjzrh.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ginqghaau.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/grsmartwx.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gbmnvgycj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqadylclp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gavfxlidw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtrnntol.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/guccqeeoh.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gaxwffwan.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gveqypvqn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbhlzgdq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdveowdfp.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/grxdgtajm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnemnyyvr.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gyeutnrde.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/ggexsrsgo.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gtttbnntj.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskaqlhts.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgtwdsvs.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbgnpidv.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzbaumpx.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gzfaazmqp.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gggjvsczl.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbdupasu.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/glovinbrw.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvfzuwtc.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaznxnzz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/guvqredtk.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejrwzyqy.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmdwijdr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gjvenltag.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gevhzztjz.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjtyegpm.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gsyyawcck.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvbiezeb.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gydcrkddl.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/ghcutgepx.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtmlqroh.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gmyikmpza.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/grynpgndm.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gbfrfseqg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgugxgkd.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbbstxzd.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpytfxoyt.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzbotjlq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/glampwgns.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gwnrrkymo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gipzrgsjo.sHtML


<!-- 参考信息 -->