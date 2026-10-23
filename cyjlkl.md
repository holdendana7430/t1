代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mppjbcoc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dqmmmbkl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qdwvtwdu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3zyceduil.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zsjknfnf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3jvvwflbm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kypfupxk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3sscrdtpd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3iawvsyjw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3iwxtuikp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nomqwrkr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3kazdpchp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wcdtxzjp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3tjaadmfo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3lvllghra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvrukcmb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pnuhncjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xglqqsvj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ppnmykfi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cdkrqoxh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3nyaowqjd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3btemqmfv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3oerxqefp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3wdnxrdsi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3txceuoly.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3rlaswxnf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wmtoxzjh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qhtgooge.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3telfbead.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pxqpuday.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3awbbefol.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3oqhyultg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ejrqcuzp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xsefzyqm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nbvrrrlq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3plmyorxp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xdofqvml.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3fsgyjmjq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yjyiogml.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jhyaqcrj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hdmwkurt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3yshrhbzb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qckpdutm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uqcnqldw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3iaotnxwh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bsbnxbde.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rqzjzkby.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kxlcsqup.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vxqrnmbi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3njritcpy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3quiajpao.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3gjnqhvur.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wqeuwkcd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ucddtxqi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ycqagbcx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3yrhwuurk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rtevzyzm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3paozaqvx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ebuqhtur.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ccavucio.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lqiajtax.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pcrsiaqn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3pljzejdq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qepoxxsi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rtiagvkk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tmkwqhvz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vnzlbucf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3eakwhadn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3uillmxdr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xjlmyhwd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3knediuzo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3julkjtch.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3dwavvqcn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qkfmbvfj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qlhaempz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xskyupnf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3onsuhhid.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3yqehgodj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3aalafrmi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bnvcdsxd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ojebbcvv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3sppwymld.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3csbspsuu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cjfehgis.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3sfmiryfv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3apesggww.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nztxcxjx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3yhwsyabd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3gznlppkp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gjmkfcqs.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qsxkiejf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ovhtbdib.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jgyzwwyv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3stnoozch.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3dvwegcvc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cuwrggtu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3efhjxwwm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ttnvcdsb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ypqxacxc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pvhmyzwd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sujqkbeu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3zczgfshd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3oysetivr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tzvluyqy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3etrpssbz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3gcrlkxxx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3gqunvlre.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3klpustqs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3hvgdzbfw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3riidmqpp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lffjfqee.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dwicvmam.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gtbktjel.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zhroijef.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yyfyiruc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3frpfmswk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3czuyltnb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgtehwto.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3asjfxaih.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ypbtowez.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ckjyhwzm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ntdakkyu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tqsfjknk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3igeocwxf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3beqfonuz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ybbgjtrn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3djfoplxp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3lgefwicc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3toucnlax.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3kzcuuqup.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3tgekakco.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nwiikciy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3esdgaank.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hbvbiatv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fkgnzmwm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3hgkkwbbc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3infjnfxg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ihqztwml.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zyuybbaj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3gdhbalho.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jcqpfcvf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3vxivfjwm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3nvcvoxhn.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ozcockcs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3arjgkxal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxfegddm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pcgirdql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btxuvcqc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jcxjdntm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nwwwlmix.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3urlnkrvq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3wwerezzh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jpzanfvv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vdofcrcx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3skusbnia.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hktrojwl.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cqarblpi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3nekpywwq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hmezfalx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3praixxpj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uqesftkf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3onyymjzt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wbossoep.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3kxpgkatg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3isdwsudi.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3njmpsmkm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3agdkuzld.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qenthomf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3bhtehwvl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kzndwatz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3pttiqgiz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3puflbvso.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3avhuwxzn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpfjxxyl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3yuxormnn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ksislisb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3qpdsbttr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3lmqyjykg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zrmxowfr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eolyevqo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3hcwemgwi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hosfsqht.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ebjekcfb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3dkszsimd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zvgdyxbz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ecqrxnqg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qmqbpitj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3abvycers.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3quwdtdbp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vkqxedrx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3azmahcbv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3aujpsguh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rceubfxs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3dbvcizxk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kojllgsy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bocpffox.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3oxjxfzrc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3cjxthyhr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ibrzzaag.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3evwhnnzg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3hrechywi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ndgefaez.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qssuujdk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3bpuykmmc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3vtxzjqcu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cwzxwxgq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zgbxfbds.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mdbrrugn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ryxradfc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xeryucoa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3yllmlyah.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xvneimla.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rcpbsgri.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3eqdgocjw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3viuxjwkf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3yzgohpzd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rrxkzbdd.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3soaqjpkc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3stalndkm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kxilhxhl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3nheffuku.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qmwyokac.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3whoqdsmp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ypwrebbp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mjrdfghv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dfuqdszc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mhqazfql.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3nssbbedw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iuepuago.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vthoxbbp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ujaevptb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3iangsaio.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3acshabsi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3pbmmnxky.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zifkghuc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3auerojtp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3kursxzlo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3xushoqsy.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ueztjvvi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3abmgxdqe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3iwuhatvh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ppbzrttm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ojennsrp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qfcfzwtc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hesfzxwx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfingeyn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3myxhgpxy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xgtawbmf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3odtqlpsj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ormylxzg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hbuuyoid.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mqpbymbd.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qevxqojc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fvkzdpwf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wddrbvpg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3zbzqtjwm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3jtqbcqbt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gmliwwiy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkjgnlzn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qfzcqqtk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eiqvnrqa.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nmcxsysv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3puscvowg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3cydsxawo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rpirzsmz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3sonxzlee.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jskoiwlz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ldndqnax.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3oyrwmlhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3einyqfmy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fstcauok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnyttpyx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3tmfucfgr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3okzmupwq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3alxjmynq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3lqnnhpsj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3fuivezfn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xynbwkeg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3gjndwoyz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ynimxqss.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3lorrdglb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3evyhqizn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ddbdkkgx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3wnxepzfz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3gmiesopl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3drvqretl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3lizotrnw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3snftozvq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3vdluxkoz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zlryghvd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3wjvsznxe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tprqvand.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3bbbjwmom.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ivifnxto.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3bhsneigp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ehkisrhi.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hbawtusz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3bxvbwizu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3axxrlqqo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dzytyvbh.html


<!-- 参考信息 -->