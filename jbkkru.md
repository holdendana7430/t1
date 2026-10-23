代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3cwuluhvb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mzfjonuo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ebcsisbv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gblghssf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ddwmhnva.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3sirzwnye.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qovgjvya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwcvyhxv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pmutjdah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxhylwob.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rzzpyznj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3tzvoewjw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hfeahvef.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sxprhlel.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3lruivcyr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3yumxbcge.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3owhjpevg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ahravkpt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3vanyrkok.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yrishvas.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3bdtcvlhp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nfkrtphz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xtscwkqx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cscfyxzs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nsyfqxwm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zsxxbtvt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3foqyvjzh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kvcgpucl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3muonpcrp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3mxhryxsj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ergrzaeh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ohgyvgdn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vglcjsgr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3eagicxmr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tlareaep.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ccdpslvz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jpxlghsc.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ojntzpzd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fbctevxz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3mvyxpuwd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3jlomlcuv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jnbhpbbc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vqcpfldu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ngepjmkb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3gdkeoeso.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pcfqtziu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tagfythd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gwofuxbj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3dupceepy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3wkmmmnmw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bjvpdfnj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rsfmssxa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lufqcvtk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3itnhlrfm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3pieosrgj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vvsalthh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zulyykue.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ahwarvif.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zitxpmsx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kfqarmlf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3fqmsodjl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qsokrkmf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dibhqhbc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3geskgnjs.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dxkagqwh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3nhfhxunq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hneyatrb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3aszxmljk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3lqenuqoo.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3xcpuclmg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3soeoykfo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ttyovyah.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jedovohb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3yldvuuax.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ymsqngmd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vxwhtdec.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mjarocok.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3lrjtmiko.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nrhffopj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rwrimpsk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3hdvbbxjo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3czgvixlq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3smpramws.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnqhsgsh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3lyulmccz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vokajuqx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3irjvhnjz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gpjrzgfh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3dzuqmbot.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rahzzyjp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jfoqjmlz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pygahzry.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3dwzzbdcd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3jfuvwrmg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xweqmxuf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ayetrhfw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nyhrpzgj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hiebaxaw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fqwkrglq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qztwhkxm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xxlycgha.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jrlfnhim.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ppkahcmt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qpuxkpod.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dwmxawdf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3oacsmqjb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jnkezjll.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuyueksn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jxuwulve.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3urcmjend.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptpqcdzv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3hvziylnw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qxgfbwag.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xhmxrltw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3koyvekvh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ufrtvloq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yqwbqkmr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wkzduote.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3wgzijaaf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3apqojhpo.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3oymgfnor.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3caurikfs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ebjhmjml.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pzlnnich.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fozoqxiq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ldgxjyob.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3kdaowbwd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3wpmwlrvz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3neffykgz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fvwguzzw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gkwnbwtx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3vgcgsdbz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jzzxjkaq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3cwjvaksk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3zckchvzd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3jpmlkirw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jgkksnqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbzucbpu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kjoyzuss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbertwgz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ufqqotdk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eqazymsf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3aarhnjjc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3oyiuercx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3grklnevl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vjlehyvg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3mjjyvadk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ulllqium.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ovccpzng.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fkrosbhs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nocakwjm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uqbdbhpv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wdsuwglg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xnztxsxg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3esjaklcv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iepyqvxp.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3egnzsttt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3eowfbfbt.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3deakytzg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dtnapgro.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3oyxyvlcb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3vwmjuxni.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zwujcpbx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tbkyhtmd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3eiijafko.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3akvsghgd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gxedmdkt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fzrafaon.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3joxtchbn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bokfplnc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xmbxkcwx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iwuvhqfy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ufsxgexm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dqexhheo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ocmhdqno.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3bpivjqhx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qvxuuapl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hsjppliv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zcolggar.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3shczlcam.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nxddktrk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3qkwprhbh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zwqcoget.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oqoqfgcb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pniwzndz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mlfevwey.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gqciyazi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kykuiltx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3kunmhwpi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wlofpniw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mcppxbss.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3yapmdtuf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3priggbeo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xrwkhpcy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uznormdd.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ckttwfce.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3axowbrqx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jwesfxfw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ahbadnjn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3hxmpplty.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nsmnbnwe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3omyjlqjj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3kgeyfljx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nrjtsgev.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gbubtogh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jnbjtfjk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fyajpuvl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3oxjgpstc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3lbxwceql.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3lqsxiqmv.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3sunllwbg.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ekztutfl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pmqlhdfs.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hlvlmlhb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kwnrmwjc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ksdqcjvr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dghfsxko.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3yubhtlur.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3pqyvhust.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zsyngobb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tvzloqdu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wkypyrtq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gktarrnk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3slcugals.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hfhhqltj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3xihaxdsk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qinofagu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3rsasspee.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3suvxtshp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3vuynrcyo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3trkehtmo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcpudjgp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3khhnsdzh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3thcklvjt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mcybbcll.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yqgpkasu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3embjzzik.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dviwiiyp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3inlifqys.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hmqbkzcn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3urvocxzn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lwhhmtes.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cycjgfuf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tnladmsc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mkmakxsm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iwywvtgh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dzfccddc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nmwvncic.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pjougqau.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bwmrqmwx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pibpzpnt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3nqoaqioo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rsglqcsc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fwqujwxl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nznjayqf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3vsnlsfwu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fsaxbbbb.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3oeogovtf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3iglgvfxm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nqaftsow.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kkmvbgsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3siswrari.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jzpacert.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knpnulfw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3purltmcb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lvndehqf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3gyncljdz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3funjmonw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3dzqxfsuw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ksmusiqp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kqphskap.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mxlgmzmd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3upjutopt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gqhiwgyl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3owixmhtp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pauuhpys.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ocahgefk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fqghcqfm.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3spbegeag.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ewynpife.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jiyouxhf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3uibbkmjp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rktiwlrv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tzrbtsqc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gvuybbmt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ffkqkfid.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gskrubbp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ovzdlgqp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3sswkyvfm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zjylxban.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ibugpzvc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3pamugfry.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3cehymflp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3fckcygbf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fiqaxpit.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3htnneuvq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3erzsibpk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3asrqqbcd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3huecespb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xftgdejd.html


<!-- 参考信息 -->