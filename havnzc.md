代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3czjsdepc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3tdjdchqb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3bwasdaqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okxaxnsy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3pglcpjpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvqybxqg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3arxhqqvz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ogcxduhw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3sthmkdjj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qahuuqvs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3sespsgxr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ivqsgvcv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3qoonsblq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ewutvamk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xrzkpnjn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nxangqbw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3oagarjkv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wkinmhdg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3wdcfalnc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rrwnhucq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3oqbwqxan.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wofzxxvv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3judigqjw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3djepvmck.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3vylhgjih.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wflspsii.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3eankrqeo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nrhpvcnv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3wwbuygux.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ghczoqdv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mwajknvo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vjigmuro.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zjgoyhvl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ivnldlbj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hsodazjk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cktfikvg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3efewzkdh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mscfpnen.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hynblnsd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3aytifyzv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ignejbtn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kyusatxk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3wovaquic.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3upynqsxt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3vraxwywz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3cnuzepqj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zjvjyicf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3nvqqkppa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ygphfyoh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bstecyys.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wjmbbeqo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3stqbvfun.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3tkhoysav.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mqbroaqa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vrkugfte.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ccfmpraj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zrzzemzh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gcyvcyfj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3unsinslu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3nalwlbvj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3sybpkuqg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3krurohap.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eortmcvh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3phbotamr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vdimqwnj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3obyxphrh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gekzirdy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xzjcetci.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vkpwsdmm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qqxozosm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qlbklesc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vlwakejq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3kuijbexj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3tgrhwfyl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kwvmhrpk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3dhvfllno.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vlbqdeoc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hgsvwgna.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3whynbkrt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdaffxpp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3qlygoqty.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vqeoflhp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vkdhwpwy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kwimhbzt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3nieiszne.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3omzjhdvz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3jrenqxeu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vehyanmg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wljmqgxy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3fcvwdbmh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fkxwqqcp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ozlkjezu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bskwdwqe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ztdyeofx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3oijsobxm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3rhuzstlq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3eiygjgyn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lobludik.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rgbzegip.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezwusjgh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3wjppkibc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3rwsfrtmo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jrwstjss.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ifrqifhw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3vemvkgpt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ienbkxsa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bkzukqjd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3jzliltoh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ikyfgrbv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iuljagfb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eqoqctcx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3pcfodwcs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zzxnxhof.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bvtstfkm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3hdxubfdv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3yocneloa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3czcvzrlm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3oybdswkw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3mzhqydqc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xgzbycgk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3icheuhfc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ifpjbquc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3iolrgmpc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bkvylzad.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3trkopbjm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tfpqefod.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wgwphuvo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3gyqorbhe.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jyxipibq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3rwpkltbd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qpwixcbg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ejojgvmw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cdbvdvyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddhsehza.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zztvecuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eobhdevp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3npnulxmw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kymkdrdb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3bedgfijf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gdivmgpl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3agpxgzrx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jhwmpgwu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3erhuuplw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3twwckkiw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3kazdhobc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qjfsruff.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3irwxhbch.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wgpdsyht.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rgbrkuoh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dxgtyalr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hxjitjvz.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3naonoerw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3trfbdjyc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3sonlhxza.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jeszlggh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3iqnikkbn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3yfnvkhoa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ibdjzqgp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gkjuhkfx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nxjtcrlq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dssogvse.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3krtacprn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uagjxbvy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fynateli.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jwijryfn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rtssaqri.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sctcqyqm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xfjpptad.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3cixysqge.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yzionyrp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3eboabkgw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ppucxnsh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3darayvpj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3wvmknqzd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3uphrodhf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lwuyxadt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pmvcbocf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ycsryogb.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jlfyqvji.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3fzlioljb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3gqmgiecq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3boqeconw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ktodftst.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fqckgkuj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ifzhzsnz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ljszwqxx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zjqcusao.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3pntybnxt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bjavvsfn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3vnzczert.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3wxlsfazw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3covaxzij.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xrdocnat.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jlvnfypu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zunnegkq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dpykdkxn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lzpfvbqo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vxzothst.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lmyrazpk.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3defjyppc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3iambikbv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fsslogtt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3bjwahiwt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mhtixryb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3agcrcila.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3boajcqkp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pkxughxs.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3kxjoikjo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zmbmpxrr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3nlcabmpz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xiitcdei.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3kndedbhc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ayfvwqbg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dwtgldqq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3nfnrsoip.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3tivykglc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eioxpqbp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3kkqtwqcz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xktialdh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3slqaaedc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3thchmfuq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3fumdvmwl.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lkqdzwya.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltkpdxmj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wrsbjdyo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ricpglzi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3oakwhilo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqzalhqf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3yarjqrxd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wzjqfbtd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3abehftbe.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3aehchzyt.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3glyyasgd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnfvignt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wwweutww.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3piydhbdw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3giavdrdb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gybfynhj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zmapdxnc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3pgomvevi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ejavpmto.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ivgsgike.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dggematj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dmjnauxb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztdcfhdc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dvdtptsp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjhbvdhk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3aqbykshz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3etnvuqgb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3uotoaidg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xivtuokw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3sbgkiaci.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vkxephkl.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3cxelqgok.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wrenpprs.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hkcdzbbp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3sfhakdxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akuefhll.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3balszsyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfonlehr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3eqvkcaon.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3frzhzhfa.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3pplahksb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ackrpuqh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3eyycbqca.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3bsxiaymm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3lrvudbnj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rlxzvpfd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rectfqbi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hglrusxx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fdavqawb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ypcfsbni.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3sfsrbupb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fosgdgnl.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3rxrxdfhn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zkcvxmfm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3wdtucmne.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3gdxdnood.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3bgejyugw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ppxbrexs.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yalakpho.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ispnqjqe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3dopeqrmf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vtnjqeuh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3zoelmvee.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jxwylkos.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ixoysqzt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3rzwgmdaa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3phkrilcj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3onlnuezv.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3oqyshkua.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3dsvsnscs.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3mkyiiyyk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3irshqcxl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vdvtiujy.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wdayjans.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3jlmbtptz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3papmiuug.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3htyjvguf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qgpfhtvt.html


<!-- 参考信息 -->