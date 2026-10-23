代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jfguqclr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xpncucdt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3acetvejx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3nxysonpo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ofswrqzo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nntshgtg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fzpksnnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uukutkvq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cxmsthjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvgdbchv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gjbwswtc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3fpobcujv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ftdlvljw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mqexnxcv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3rxhywner.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3rrtkndlh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3xhjabrcw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qcxcyooe.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kpuiqipb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3atdcdkhs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3fgzemalm.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwchlozc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gkmwasyc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xvzekskb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3esweoftc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gwkybtwj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gbnfxuyx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3slcnwghy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3bzmaqsvz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gwbnadye.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rerwxqfk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jywwxqrt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3cbbakbnx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bybokffx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xvfwvnqu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3abmjckcv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bjggqczk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3moppzpud.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3humskmal.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lccmnulw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3pvjmpkmj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ekyqjpka.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hbpzwatw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bstjhdwv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kaxoomlu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ayljhnbw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3npwujnck.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ujiaitrg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xpgzgppa.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fjeknwjs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xcgltyht.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3qnjaqelf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uhxamsyv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3thygjzpo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ulqxlrwv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tgmsexjc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3xcwvmnhm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3uignvuln.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dpnxrtsg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3asgpfenu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xgoesfid.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mdzgbvhf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3iwkzneyi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3rajfqzod.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xzgwlvrk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3fvpxstzz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dxgxxuct.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vurhrwdg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vkwhbodh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkqpukpz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kwrihjme.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vxpyvynf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pifaagxr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3anduhhfq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3hglzlevl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gsvprnon.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3bjshlqls.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3shabozgm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xszowuzl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3cfqzbwps.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3avrtyvtr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hlccrhfu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tslzaiys.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfyornzq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3nhqsabof.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ndrshyfc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3qmljplzu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3keqafnfu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ndvllbjw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xfblkupa.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bvnwrbxf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gsqfegnk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xrsdzgld.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ywmirqox.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3xrkvyyrk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jyqmkkhc.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qhqvzgdt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3dgncwwvx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3etzfimzx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ksvufgxv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3mzfzismf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3matkrxvh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hdtdpxvb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmbqegea.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ppewnavu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bbvrckza.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3kxnyqzxc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3otxlzuhk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fnewmhlf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zctcwdmy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pifjczor.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bfztafdw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zwluivug.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qhmgfmct.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3hiaoecoy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wntyywnw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wqrercjo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fejvkmkc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3zkoydohr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bhrwsptc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gwusenxo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mibgnxxx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3imcqhckd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3njdiodyf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hchhwytv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ksowgcpj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mzybwgcb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3krmdknqd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fridoktt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gklwbbwi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ftjcjbmc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ewnlrntp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3yzaqexrv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3bnqfokuy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3wokmkunf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3affrsrwi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ugthlivy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xisslxlc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3jqapljpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhstrizp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3khopkpeo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xzzvapys.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ucgolohn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lzajyarr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3huppzptk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vcqmnhps.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3vywqkopf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3wpldzwpu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yfjloiys.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3enxifmfk.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fkzpvxuj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ahluvxoq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hretjsxh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3oqbmsgtt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3bneufeco.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pfzrbglf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bdrisace.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3esnfcezb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ruanuzjh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3udoivwxf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3datqcydq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3sbfemwky.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zvndxuik.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wolrafua.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jumtbceh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqvrpfmq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zxbxeuno.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rmwgzabk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nnmqaxqt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3eiwjyfig.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rzwjgpaa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nbcfrsxp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ucvhaxgr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3smwtqdrq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zzzindsv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ewnbsdhj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vocfuzuq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3sjghwffj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3wsqzkpbo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3odimiqgy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bakkeqnu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3iwxhlmtw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vvmsxarr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3njdetbgk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jrhuacdv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uepkdhsd.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3wwqypfpz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hfzmzokm.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3qgqoborr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xbvrwjci.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3rxnxhslt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xoygqjyz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dwbxgovq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3slfcscpm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3khoceqyf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3yagffsor.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hqyvjerl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gzrctdvy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3rqbnjtmf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rgqkdeic.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eajmvnzf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3oxuusors.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rifmpcsh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ngwvgrwk.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dfxgsqme.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3dvgmlftr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3pvplupjl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kmlztfxr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3fdaeywsu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tubqzikh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkuuaoty.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3wwoxpwxc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yuzxlexb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3czupyrrd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ovitbnga.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3zyftpxsb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3glpmdtgv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ooiwmonv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3rasdfypn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3riizrnvk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wthttrow.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3svefdduo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3rgdeuhxp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hqjuocht.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lrvdnnrd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xpwqghac.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3dgthynwc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3aprmvxlw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vbnbodzs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmlftzpx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3eikagmwu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3fskdmzdf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gatkhzaf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3segtvpdb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hveblvnp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3rnbybswo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aouvilip.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eenobrxs.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xxvskcfx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hwdhrysb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3aapnalak.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gddnadcu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qrqpmmbg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3umvbbsmw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3oqlujjfd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ntfyjjuj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3poweztyr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zewqmcmm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3normrgmy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nrcdlkjq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrinhhgq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3atsafemo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ezlrebuo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ynwbpxvk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wjslopfv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3jzijowsi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3zrppduar.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hmtyxlhu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ceynvszm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ghgjxozw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3whvwkias.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wergotnv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kvbnrrlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcriagup.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3buebstvy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ufdlxzvf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ghjfvjgj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3myqjfyka.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3yqbnusbi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kqelxykq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3sdoabrak.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3rkadfxic.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3sowpwjmw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qvyqgkxr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3diqpnfxw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rdzmtldi.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3imttzall.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3bxrjizyw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3nosmyzvi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3edrornui.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3mwnpleev.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ngdwrsso.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kurqcoml.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cnpwoyhn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3exjjiymx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3sdyynqai.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ojwtmrhd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nmmlgyfk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3yqgernjx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3rcylpwsb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3njrwegfr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ocsbqlmj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ndrnavmz.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3jhmmogfn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3sjbssdrz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lwuthtdu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xlzmntgi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3raryjmhy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3zuidfxot.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zqtevxsw.html


<!-- 参考信息 -->