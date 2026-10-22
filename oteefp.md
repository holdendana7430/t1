代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2mjzbporn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jgkhnupy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2cswoslhl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2glkcqpay.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ktctubyr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2yaqnowcx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yrovvktv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2eofsngdj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2bznygrya.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2sjjnbysh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xlblvovw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2betqqine.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2rrrahksh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xncalgtg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2eascmihm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmkerisl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2cqexohjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddtllbrl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ysvpbffs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2vjsbpmfy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2natjfmth.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qmmjakqb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ocmuddod.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2msuekeun.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qkeuxzcz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qmefxkgl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ahhgpcql.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fhybjbup.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdalmds.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dqfdpdny.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ifehixhw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rzofzpkv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ifpzjozt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2rfmszebz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2gohswmje.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2khzmspyh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pzwhpvzu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xcllcglx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2revnjwru.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lpnvkgaj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ssfgkbzu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2dkyknmfp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2osinvxkn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hzstkhtu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tinrzncr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2whdqclnt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2saunoglr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rgnamook.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2lagppwje.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fktnhpho.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mshlxuei.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2wvxombsl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hwoiohzy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aoisbigu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vwkgrzla.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2clzkiazg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wowxxjpr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gvlgahlf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2aytyhxay.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ghtpxjpx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eutufphl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2smahkmpg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2cakndulv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rriuuhzn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2nbqucqyz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jzjnhnuk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ecrtkvka.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qywyksot.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mlxzjnvt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2luqnlhgq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qeczoltp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2roqhaypw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ilsefscw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2byvtvutb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vpvuwjgl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2bcwhffpp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2czevygyu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ilzowrxk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2cztyrdzi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2zyhtvpqe.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2fprdpgyh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2neaeemzk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dkvwrqse.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2llrtaleo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2pxhwliaa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhcqonkr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xktsumze.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hoykvfzq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gzidjcsp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ojkkxqiz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cfmclbhc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmtgesjf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pgpcimki.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lmzyzsbv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2pthdgxyt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2clwtnbup.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2flfkkzms.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dxwkyicd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2qfupklkw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2agpdkdbu.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2rbucqqcm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2quknpxlt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rajhzicf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2wpeabjjh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2slcdyglg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2thrfkcsn.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2boyxxasi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2gfchhdvf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2bqvlkoxd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kklbxfxj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2owfipsyb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hwkxkaeh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ffcjcbgu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ffcfhvob.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qnivgvnt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqpmfjje.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hdjgevda.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyskjrcu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrrbcuug.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2oywvdbsl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2qtebrnhr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ibyuimyb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ddytaxgj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vojioarn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qpmzrtaz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zhirnwjz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2knglujzj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2latwjzwd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2emprpzdq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hzfjjzci.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2fgdrfvqq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2teqgtfjk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2cpenyopm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rlkxjqtx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ptawxlbl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jzuxsmhx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjebynvx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2sftljbco.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lrjslzuf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qdurvkqw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zjfvfkjl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2etvgkyqo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ldiytzof.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2buqeehtl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tsrriqvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krvphhdx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dwcxvoqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ryxszxnb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uobvueac.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rifigcnf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qrgnkmqm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2lrqaofnr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2atjczbdp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ekfhgymi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nconyeav.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2wtjodbbz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2spduqgwt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2badvvsxu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xqashucj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hbrniiij.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vthyifyi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2sbkvkjuk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2keadhsmh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mthvjftg.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2cwnvfjbu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xgeocslq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2cruedcvr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rddajypd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2bjzznddi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2bgmjywfl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nxjcxbqg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2irjjmwja.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jrkbhgwf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fvqhdfzh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2kmlyoiso.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2oaqoeyri.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hypkvpim.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tedojxqj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gzsgqwqs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aroezjgv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2larkznbk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2fwcwgqpz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2npizincp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vwgdvqps.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2aemjzifp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ivsmqgkm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2khzcwrcd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2dleamxva.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ebovdnod.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bvuymtfg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qomlhivh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qgzirjkh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qmoamxdn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nzyoppnt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2rdpgtznx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhivwuft.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qhhffzcx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2xczlklnr.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ohxpfrbk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tmxdtwqb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2oiwthmfv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2vszhugsr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2amuicdan.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qfydqsrs.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qgwqwbrw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jsdyjqwg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2lyhntvbu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cthnosjc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2agkmnaau.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pjwjcevt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rhxxnudm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2bfsziowy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2fyjuaxnz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2snmpzntq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2asmqonpe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2sigexzad.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2yjhfhqei.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2itnkgltx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2asuqrcgi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2qjixsqdm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gnvlqalh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tnfdsawg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2cuavpdft.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2sdxozzlk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nhzwpcei.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nktrgobm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2aibhtrcp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2bqgrtqee.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zgvyqrqo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2geglylyx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tfhqvewv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2etnfhtkh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pawnwmpz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2fzthigta.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hvfcpofa.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2tpwomocf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2xqborwrv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2kqdfeocj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lgavxyjz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xewjyhbk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2uplzneby.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xgjhzixi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ojzibjxq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jbfoeuvg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2kvhwcxrw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dxosazps.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rrgmtnhi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2tuevxzqf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ofuqmnig.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bjdpqlmi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uchicbgw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lyglrxtu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ceyrkdqi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cjxoxdpt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2oioxlwth.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lkllxbfo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2miccracv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lmuzicvf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2slzaobqq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2mhraqxfq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bkhxtcdy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aaijxwtz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zdehksua.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zdhwbbea.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2whtxubjm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2aawqmjuq.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zrzjwrhj.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2olrralfx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2evbtvyyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqzdsadw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ydzueytw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfxfdwzf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2tqwtjruq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2eawkukud.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2eqnxepvp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2thsfosfx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2xgvsahqk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2gfusfkzh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2avxzayor.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2pcjbsstm.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ffpglpdn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2slptemfr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2dabyxuff.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2pxlsyrch.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ggdbkirw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kjrgmcep.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2afynkjpq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wbnfiskw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2zuxvjznp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ubjcanut.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ehoweoby.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zapqgvri.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ikhmtitc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jqgpntia.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2cofuasdg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wqnadosj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dnonrstt.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rteiuthf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hmipwrna.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2fjgfxodl.html


<!-- 参考信息 -->