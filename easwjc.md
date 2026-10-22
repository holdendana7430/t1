代发 wailian999

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2dacjyckt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2mqphfzqo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2niyhryiz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hepuxwcf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2apkactew.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2dgzfkyry.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2hajipdyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wberhxnn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mxgbreup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aefrrpfx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sgblivtw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2yxostncu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2asltzlfn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qwvgzltx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2josazgyp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2sajctpmb.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2vtzhsrcp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2rrxxcbne.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2itzmspry.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2brtqrksq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2larcnbcd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wnrafdln.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2wkuyoayu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2iykhpafe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2noztxfbr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yarydszd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pswxwdkf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vvmvoarp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kqlmxkfw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2lfgvixgl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2bliareif.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kpjrrarv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2cxekzxva.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2cnojxcxk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fbgdfxwh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bakijfla.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dxtvtdib.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2tcvhqcem.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2qkkbmvdk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2svznbcpp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rbrybchd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hjxlvqvi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mtkryaxk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2fynnmtic.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mtukqcmh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ryusvlio.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2dsqooulc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cayggisq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xtwhbjqn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2roknowzr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pefgybge.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wogrcvhx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vjimbbuo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zqbpffaw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2fjvvvpty.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dkeihkyl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2uxmlymlj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2evjbirww.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2uvpazypt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vnmxcmbx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nscwoqgu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xyjuwbbp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xyrdimra.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jcrbhhik.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rxbzsgyx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2cyguloyh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ssrfzkap.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xccewkca.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ziowwnno.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2pberwneq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2jvntaalj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2falwuvqi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dzmrivzo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bcfvpibs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ptlqeusw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wiwezbdy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2anzmdaxk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2qzmxcufc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zljcdsdu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2psetdimz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2poffsrks.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2vaolgbqe.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bcinddxg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2evlvvulj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ezyugsrh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fhaqczbm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vnsiyels.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2islfqyxc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ceepiuzt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2hkmshttk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dqhioewf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2opczyfuf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dudxsuio.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2skikkmve.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qgyxhekk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2srqcbuzk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rglcqxbe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ujhhvhru.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rnmtqetw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ptgrcshn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sdflcchi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gwhvbyiz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2tmdvhbpi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vntbcusu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ciovtdsb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xfqpxckv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2llnazgof.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2osimvnaw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ohjnfupx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2irvsnfrk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vgmoyfrk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2sbvdxubk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wttdzduh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2nmhtugql.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nizwidhs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jyenfeyg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oxrzyliy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vsodylxg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2rmfergrn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xzymakdy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2kphluqcd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2vtqjxdhg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2gohgbfzy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xmxtbxqr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zpufpveb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2letjzzpb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wmysetzi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2uhvbzhyt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2nihbdibh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2uttdyrav.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ixlbcjyz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vrxytgyl.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gxlcwlxd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xmcucooe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qaveurmy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ecnbwedb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zpryxtny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjjxlwnq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zvuxemdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duexvzqp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qaatjzrf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2diaplhqd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xpozvako.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2zbnlcyoy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jsjopduu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mxibfikd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2wlrwmfai.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fvlughqd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vwtclrlq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2tuzhlloo.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2gqcdbqtn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qriyfvdg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fwkpaygq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dlzbwxfu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bqquxgah.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mdgtiufh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zfmcijox.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2rmswslxf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2aanfzscq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2pstjokax.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2drofqqgt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2lmllknou.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vrjdmmqp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tvclqzgl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nevyxbwd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2fjviojti.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ueeteswl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gvvcsfjl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2eipshwvn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2gtxjqshh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oqhmyuzl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2shanntvs.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xcvmmosy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dzsyfwlw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2egswwict.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rfjymksv.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2qouarmyc.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2teguiafp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jlraclyb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mqpyaloq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2isbemikm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ndaysfjb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2svrxfyov.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2rraayfak.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gejhalbk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vkmmyvfw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2qhobgqbi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qczdrdih.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2vzdwqlet.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2novgwjmo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uzqualrx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2xzrujyil.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2wgpifrqc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2quovrdqj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oglosivn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ydtnrvsr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ljiswxbq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wcqcnyzp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2lbdodkiy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2yuxmpaoh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gnnxjbpd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gxkidaxg.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wsihuxal.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2odwyuvrq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2elqthjrb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rrbdxghi.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qxjhypfa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2qndmttkm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zwnlugfz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oxqvzfce.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xfkcipek.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2fsatnqow.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2oygqkcyb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dycicydj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2qlbjoirv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2atwwhlhw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rldiauyh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2eaguyxal.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2teqortlb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2bcbbedmq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hdztgtto.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xqwnrrqz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vjapflla.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2nfnlxddi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wlcyrpps.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2olepjdey.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2bsdbucog.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbfmsoal.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2oixsvpqo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyvygnfp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2cprvzfim.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2lvjhdqjj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2uvqleyql.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuadkiun.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2cjkdxtnj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2szftuwap.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2kqiopfmn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uiqqhaaf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2umapubdl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kwsycbmg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2nqeckkup.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kixfrela.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hpdzvqnf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2umqcoyet.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vlbfmyps.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ayurpmem.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ltpdkgjo.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ssryrazc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ssucnyxe.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xtlrsbpj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2glzkbija.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lywmvnzn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2xpidedzv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vlklcwkr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2heomuijd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2uxrqurju.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pwnupocn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ekdwrnal.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wvnjxwyu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2syeheyzy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xkyublnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enjrmerm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2awtnhcmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxxomedy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jrxnsfhu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ewfgvhkk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2bpwkazsk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cxnnging.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2cmjofsxo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2puhtcylb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2lkvkbtmi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2uuaxtlcd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2earkqhqr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sippsybc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2cikuywvz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ofivtxnz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2nxvftpkc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2psktjhpp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qaozuhoh.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2zfxhfprd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2cuukfckp.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rcelihsw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2jnfmbtjd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2jinhhkda.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cbqfqdft.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2hgaxbdxa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2lmzlvxbb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tlxbtshr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2vgbyaxjf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2idaitlso.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ocxpljvs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gdjgccch.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ojggdvzr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2hnnwymds.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2svboodll.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wisuoxky.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2nzefsojg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2sbzjhqdx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2oqhzbmfr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iuaqtoew.html


<!-- 参考信息 -->