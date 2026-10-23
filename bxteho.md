代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3efkygthg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3omzoxgdb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kihdvcmg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wznmpguh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tuwnolld.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ceejgjyb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3llcpolfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxnbxutj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dbvcubgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uugvpemm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kvsituqc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ykuigeoz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fmoawtfd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pkjybaoi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hvdynmgk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jwbfaqbw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3pgbixhtr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3kuuugppp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kyomdcvz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3eblxeaeb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zdfuwjun.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bupylbed.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3edhohwas.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rkqcbnjc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3yjftcypx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wcsyvkwk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3eaaqwoie.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3sjdefujl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ikkpkmxm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3behkdmul.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3oixkuzdt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tsnkzuxf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yuivtuqc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zsqvqdcf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qozxsrdt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ajgwitgk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3olgwmwid.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3anjceynv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jtbtyhvq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cpwqecip.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3epaskhrf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ygxyrrqy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mwcltiqx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3drerubyx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hxoqavfx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3caidrjfd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3euzhjaal.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3boocqmsc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dhffwtmc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xuwjrzyv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jeqfqfdd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3mrltwymr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qduartkt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3sdsdlpol.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yvtbpkee.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cxhcjbij.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zimrwiqw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3apwwauqv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3prtdkwqb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3uiprrwdz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3fiuykhte.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qjuospss.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xhtkzubd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ghvqkzgr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3gdkkofkd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pvpfrnqp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gkkophcw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3aecavbfy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dxtjrrgy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3kwjpuabz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kbzguxch.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ujrsuxxf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3goyvsyhu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3xgqwxzyq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3rmdxzmnj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fwmllvha.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xzyxpwwc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rufsoncl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rnrisskm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3dtcqaxhf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ypoqtbvo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tzwegbbs.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3gyubldwk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bhvyiqeh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3kxqlrsqy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rokqkver.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vnacwjye.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zvklizki.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fdvyetwo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zrhjipho.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pjrxcyrw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3hpuxocjj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mntbbyop.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3twgmcppa.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3zpopnaht.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3soikbkjp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmnpwgir.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3lvkfkqvb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3oudcmlsm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ldbmhajo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3fhexpgki.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hnrhuzhi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fgkuouis.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ileoimty.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xcyuhwnq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lzosdsae.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3trtrwgyx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ayknmhzo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3djgvxgmg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3peubyuqx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ufblzyie.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cnkqqsjw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ohczbtad.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cnzfizsr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zdsawwqo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3urrmyfdc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vamjtpue.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zkflwove.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3sjrfqbob.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3abiumcph.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hldrzwqk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3soxysfur.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rkxdkbjr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hpzkllgy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3mhhqqjsc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cwjyqiqo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kijbzcxs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fzbwprnn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3yzssyubm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ghcjrsgf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ssmerudi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3uphwezuh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lszgkoza.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3udsqfdwt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fquczrml.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jnhqrkba.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pimuesig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldveighf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ezfyfeos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bymrfrwn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ocuyihxz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cayrsfih.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3knpkvydx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3mkotgngf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3eyedvgec.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rlqosfya.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3dspnqhqd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hzmjucrd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lfjttvog.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xldstvpj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yvhdpchc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zdsfptki.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zgivxbas.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pdsxkpoy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3smjexntv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3puwjvqam.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3iukfzbzq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ozzykntn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3pdvkxfcu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xzfconrd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wnghvhji.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3mvjucakf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3uuseivvs.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hnjgxywx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cddtcdio.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vyftqntk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3teocsgqh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qqwrradv.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bhpkrrwm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ivbkoods.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rinsliku.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ukyvvgsf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dkkvhatp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tqvcocom.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rofoxdph.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3gffxingr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3spcpbosi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hjkblrlf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3yznawete.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3udwaydnd.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qjuywdit.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xbmrhbdt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3chuazgmo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mbaaqvqu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3viwqcsar.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bcieqoer.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3cxipgqbv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vmdptiig.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3nhfwsngs.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3rijlucdk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zrxpppjm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jkpqedkh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dretvrky.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rffqmgdd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3pqfxhgdt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gsciobyv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tznuweyj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lsuzzfsh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qakddgcm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3eovughch.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3izrbwvah.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rmgvqvmb.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vlsxfucl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qpqlhoam.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ecadcbdi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3llnwiivr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3npirwmwg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3sbovvsgs.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ecgiyhlp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fkvaamqv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bbyjlbgk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fzobayho.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rzweyzmj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3kbeftulv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3kslnnjun.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3tahgaeer.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dgpfeluj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kiwisegw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ifilvatc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ujpxyupb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mxvfpvkq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ycqiolgg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3owobwpfd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dbaodzjo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mgzruzyu.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3kwhytucd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qtvglwzx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krfzayhl.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vdzbpcmy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3uxhntosl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3rnghptwr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozgkjdkl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ilfisyzb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruximoot.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3akstigst.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3sltftfsv.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ldsicqqw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3onvxqhpa.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbfzeeln.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3lmmiiaew.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lbveblwh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vngxtmwg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vturfytv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3aksfavtl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kaqkrsvz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bqxgbmpe.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mximedla.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wwprxejd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mbzcdblg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pxkmmueh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cyefzhzy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ounooetx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fbausvze.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3prkfadna.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mosyohhb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3jqsvuxwk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3oiyjfixa.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3oniuttne.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mnkfmzfz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zdvnvilk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3mhvphdip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjxwmkrj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xldwdiwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omgksqnj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zexpkmtj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ooutpjgz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ukakdroi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zgbjwama.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3gruohgcy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3vwnjkzjm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jjlyrdmb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xozzvfyl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xdvwgqgf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nlthblep.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mrwbsnbd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pzoevbbk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nuczijse.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3roovznzs.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3igqdzutu.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3tqoyhtjd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3xjzfbzdb.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3eamskprb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fxvllquu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3qkqmuvlw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ccseoshh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3osbkvrzo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3soyqqlew.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3masbqvce.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3cugndebc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3bdqmiagv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3lszlsojv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dtedmnbl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3oexypgft.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3brwgmlvj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3oxauhekv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xpfreafo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ryaodixu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qylslzon.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3yfjeckhw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3geqvdeel.html


<!-- 参考信息 -->