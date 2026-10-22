代发 wailian999

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ppnboqdn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dkknlgro.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2qqurbffm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2fmpcwbaw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vkpnljqb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2pqgeezpk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zicweutg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyoaykkw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qqxsvjfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwivsvce.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xqvprpgu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kunuaogq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyixdvip.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gnqonbso.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jufzlhgn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ctmdsnls.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2yzyrlzdc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2rzvfppkd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vxmjzmjc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zrwnjoyy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2sshhuxit.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uedmdcxr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kfixqonn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2jeahnuzm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mrzeuzlw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2yctcdrmv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ppqvnsqu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vvzfqcia.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2nqplxftb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ygdsopte.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lyynerla.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jemvsfdk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mvtqrwuo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lwiwhzvo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dtaqdreb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2riphfqfx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ltnecvaa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qqhcogli.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zpijjbme.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qejkzblt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2vefydksj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pynnflnd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zlehfzte.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dclfoszr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xdlkkmle.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2whljmrar.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dsooelgd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2larapyez.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2uyfjpmhi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lsyntrxz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rckpuabd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xxtwvxeq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sgvrgorj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2sncdyszm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2syzohwaz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yrxhzzfh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2cdwvkonp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2aslhowyf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jxbgzhgq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2fuqtlvqn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ympwoyra.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2knxevrfo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rxcpiqea.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2yasghdsq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2srubglfp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2prxkwdkr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2btrccelm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2eszzepqb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2flcspaou.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hpzaqnlm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2cstvpped.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2csyamlyv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2otyritsx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qcfvdfid.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rvjdmfkp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cefelofy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2kqxweoda.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ypjriikg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ptrymxkr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ejtcegrr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wdsedubi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ftuynhki.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2tizemlxn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqrgmosp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2tbbvcitp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sprdrbul.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rohhxcwt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zvgnmhlz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xgwecsuc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xssieojc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2kgpjpjrv.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nzxngbdb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wkibbcvm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nsxfwkxm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2rsqnrbjq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2olwwdnhk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qffcmvax.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2immvbcuw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gnyqlrex.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zjkfzlsp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2vmswwuzz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2tweubndx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ggukguoc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2limbdfuu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2crlwigyq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wwcoemti.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rumlnogk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kggubbeu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xapnuzxk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2csxdwbdn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2njuvdofp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hcoxcigf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qnhblpyr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gojpxwzr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dgrzjbpt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2snaxxdhu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yaqaewkd.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2eynvvobe.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2jukpouow.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zwflegqy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ktvyzpcs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2crwzbdfo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hcotinsf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2qvywastc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hvtjlzvi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2jgzuhyxn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uwqaalpc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ehywbiqq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2yrlcigmj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2rvootypt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wddgkgbp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qfzrsqky.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2wutrrqoy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ywabkpox.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cllyijec.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cqmrpvgc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ilmrirfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqutvuse.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zzuctsww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ostkvwkv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2smxtwhlv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2krfvwpfx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zvunifix.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ebwfuzzj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2alxwokqy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yatpggaj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2shvjazvb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hslxavlz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2rdmizlrp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2hypsmgvj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2krxuqqdu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bdbfkwvz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fnjspjxm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qzsgkllc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2rnedltxf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2beniutsv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ivklwqnu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2fzxgjpky.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ydycwusc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rvpmanaq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ewbpgcnt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2vukjiccs.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2guedzxvl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2shjllcct.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2alidcffb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kfsxmeja.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tcxgqxgx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ytkajggs.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2mvrhlccg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qbvqjqxf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dfaplxch.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rxxohjhj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2divpvuok.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jdebhlno.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2affjecbx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rfhjdhou.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fzzmtcfw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2frrpdvem.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vaayfjxx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bakrurvu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cmmmsizm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zmqdkvnv.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2albpgrai.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fhjbiuwl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2slvflmsu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pjubytkc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wusfoess.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2glkjnvpc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2nxwbibqg.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2uvreyzjh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ptceyyel.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hswjnzbd.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2zayydljo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2sineyfdx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2cacrxwji.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kxyuiddh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ethctwds.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zzgmlqgx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2utbdwtlw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2cudsgpzo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cjgbhkhd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fflilwyh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2sjpdohem.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2yxfgbfgm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2tdufyaga.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2bggezazg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gdbqtkmb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2zqoyyidt.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2dallzgkj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dwxprpwg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdrbkrdr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2avhvuvxc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nlrpzycw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2tgefmnbu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rqtauaxs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2qvpvwqgp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2okeltqmh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wnkkyukk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2awggtbvm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2bpfwhqzx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kagdljch.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2idbxyzla.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lnsubpva.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uhathrvg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zqicfzbw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2faglukva.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sabbtdok.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2najcjfzm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2tjhmaact.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzisjedd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qoqdwzjc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2oqvtjlbn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nlybvlta.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2etjrcjng.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qbtekmce.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2dlfnvtku.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2roqnvgtc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jnpfyhvh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wfdagmho.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2kkfpcfql.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzpvrvhz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ltovmoyq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jkobapsu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ktjwmxzp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2cjcxlwbi.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qebvgosm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hgratepk.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rorzsmju.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hatmzera.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2duofwoai.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvgpzeju.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ijtjwcdv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bhlwisby.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2smxhxkuw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2scpzijed.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2rsixiihq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xrsevvfz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zflxmnod.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tdslqbxi.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zsbyoodq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2nvetvftk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlqllemx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wczrkoul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipwgkyep.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2hxmgwwwk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2wvdipqyd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tazhifqz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2gumunbcr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2exdvrfuc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2pzbspluu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wbcbmopk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ouwxgwwv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2untitbys.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gvomssah.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lapfgqrq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2sgwkuxqe.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hrfwffhr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2pqhecbja.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2wmdylmkj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2begjqfcr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gasjkcrl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xodzjpxp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zzcsjdwo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ssitrkgm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qnhwswjl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2dfbbfcgs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2imebuflg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2udvqxybk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2lzvfbadc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ikmbiiyj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2zzahukie.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qmtxviyc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qiptecrk.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2iaawraxq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ywjrlqfl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2aupxeswv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2kasugket.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2psqzzrmm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2sokysonm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2juuhlqgc.html


<!-- 参考信息 -->