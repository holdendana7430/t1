代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dcumpius.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qqpqwlby.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ricfkgcu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mnsfktru.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fxqxqcqf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3uhfsdses.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3uduatbvx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ylawlofr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3dytxkaoa.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fqyuqybr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3crcwoeyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwbmimso.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3sagmljst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgkrznap.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3loydeyje.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rvinjbzh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fhximsht.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3oxiynxvb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fxznsada.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3dpvhmidh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3esvcodhc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3uvcqvbcz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3onpoeihr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zgwhzdfe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ctbqzefy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ehzpanfn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3xahiavtt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xqtpitrw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ugeguxmf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3bmoggjyh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3guajbown.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lorccbnf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hxqhhfen.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3bojnvwfn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3spbsxbjv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xgidcgce.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3anupqujm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3cecnieuo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3izrufpdw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wxcswejb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3txewfwvu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3blypkyzo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hzalmdpm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fcxkaevv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3oquwztms.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ybtjvaop.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3tipnottq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ttuiwhww.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gjsvftoe.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mjalnokg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3rnkhnlgx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nwkjsdjm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bsjiruhl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3zkyfxjev.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cxrawwbg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3otredmnp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3svzdvxtp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3opdgmyrx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tsxxoecu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xsojtgux.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fwwountb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3rygnjfio.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zwsmcmjz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3tgoohcgi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gfmnvgan.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ggfewuii.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3stxcvjvf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3irhdzwdv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wbtozsex.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3cxsyjjvw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ysvmqhpa.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ylgnxmjy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xsjbmizz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jazfhklr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zozjddun.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zvjiffgv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3bfszqidy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jwggzaoc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bbisdbym.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bxaqnapr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3tznkhmzt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xhpvwjtm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3anlkxdhe.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mqvlcdxl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3njfuvqrb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ghzdwafj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jtodhyrp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyoujzdm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3dryxafdw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yfbquzxe.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3wyqbyplz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bweglbum.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3kkqzopug.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3vxpjkzgn.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wymutlhs.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3usuigvjp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3uysxicno.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3amuysass.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bvgzrohq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3buihxjye.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iudtrxlo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vmvystsm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xkqhwlbq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bzpuqqnn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3tjyqclwc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3nsbwfhyn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fnfdtppd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3darwoham.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3yjlfxvvf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3aovnuyjx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zcqibdbk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jcgcqmct.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ztcruhls.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3spstcdnb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wdnoeshw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3hvjxryxc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qqdwfwye.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3clvxkztc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qizzbosp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tpfggdaw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3orexfhib.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3isuikjru.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3epgzbqbe.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3exgmcawh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynnhadjv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cuhhicrz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vxfixllf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3akplijka.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ojxonpck.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xfqoemqb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yqsauvzx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jdstexcv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmtmbzeu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3mhfjmkjq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lcgrxetr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hcoypydy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3eutjjezz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ajcoporq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3bphnrtto.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hrxwybca.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lgjkqljm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzrfapkp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ihamjpns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uykxsdqs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gzzmwkxk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yxhzvjch.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3utnwhtnn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nkfgtaio.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mmpvlhsu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ynihmvhc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dpyrfvxk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3bylzpwdl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gmfoswht.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gszanqll.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qbltjhus.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wbhdwpws.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hsefxhek.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3lcznnxcl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3esboiwza.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mkhtjcya.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgmizlff.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3oyuyhriv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xbvgnxzv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3baqsmeta.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3pcjuagxr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3mwylovle.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3phrshkca.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qxvncavs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3lfansndo.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3evrmtgei.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fjulaeao.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pnxrjiry.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jvmagzvy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hagjdupa.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gzjdvyzj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hrnuzjey.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bzvjqdoy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kzvffwiw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fyofjzvc.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3rvlbbszf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3brarxscb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dmmwaiov.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rxteggsp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fmwpbtrv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3jcmonkjk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3otyrewjn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ssnjxyjt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tlakckmc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3eserrzhc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3frpmwcgv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3huyncpxw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jwbwjuax.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ieziwjmd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3qyxnlftl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gkvomlkv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fuvmcoxs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3otstebaq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3cjzdouqp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kyqlvqsq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ltsohbvr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3rjahuybe.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jhklckwq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3inyrlfkv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3sxorsogw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lslmahhu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xctrxrlw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3wtuikxqg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3jslgzssm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zidqowkg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3pvbxhnvy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dwjwarja.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3nahnwnoi.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3smeuythi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nndzjucd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3aoobqmmg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kapfyjzf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3injkkudm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3rzykccoh.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3srvnjezb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3oohubmln.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3grtyjywf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xlhrmrqi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3duwktvli.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3anzvujan.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3asupivue.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hpvgbinl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xkdqshen.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wwvxuwkw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3auhdywqy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3lqsfyahd.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3epfshuzm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jdamvcro.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mokvxtga.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgwidsar.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nieimfbf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eojyvafx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3prnrcgoq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3csjejmbx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3cpytexvm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3lhqbhbsa.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ranadyai.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yavwasic.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ieprimqy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3auvrexsf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ptthtset.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ncpedioy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3obqofzye.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3vejyqsfj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gwyqfook.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kqnfxluv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xciuqffz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bwaptmco.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdrpjtxc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hflduaqk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wagkcter.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3xqfbssex.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3tckmstqa.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eaewhova.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jtrxqxyj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3lcnuhbvy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3sltdqjnc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3tshteyqx.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jlonijjt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3osszzjry.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3wuevhrxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcnyaeuh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zwvfnvor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evvhesho.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3rpfciopm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dsjdvzus.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3tiwjhjdg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jqwxqqnk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kgijkyut.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3mjoattct.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ehfzrplj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3nnknqfkw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3dsjnaepc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eytcnlrv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3gabrlpfu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3bczoktog.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3flwbtasu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3udynwmaj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3adjawtix.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ahpcjsmv.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zooxmfjj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ybymnvok.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ipgsjhhy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3mricujcf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3infwhkeb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pfchxpyp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3wgnjnkhn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rgonotsp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hhxblebc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3fnuwwufu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3thjgzkmo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3agdvgnoe.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3idezetem.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kzkqgoqv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ywaikqkk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3aojmwbjd.html


<!-- 参考信息 -->