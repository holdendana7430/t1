代发 wailian999

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3hdxzglmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nswuaetw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yvpkanbm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3pprqhhvv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hsbujolz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sfegzpkw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3aiqyzaew.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mvfayido.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3pvjoxlel.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3jgfejpof.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qhqobpdw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3oamtshcx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ftpobcfn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mswpimzy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cktdimcu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fvdglrmh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hpgnnkng.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3kbsjqeon.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3koopwbkm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3tcorubhx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3tufxrcoo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3oyfdxioj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kxqcdtsd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nngxkmmu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3cvtmifve.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3txkigcdb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zjsofouu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pljoywqg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3sbepitaz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3vxkdvcgr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3twttuxwn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ynejahog.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3drotjapn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3kvvztgrl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wtfmrnjy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3dqymimry.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3bkqazvww.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ronmkzyk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3wnvfxowe.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3oblknetk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ibitqdqw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3atekpusi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zdwayeim.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3drajehiw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rbyqnvbl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hrjigoex.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3uwxomaii.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3drmpmgvo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3knpparob.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mrhsxwte.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xgyguikk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qjisbdet.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qxjkjjsl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nexaumvw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ousxrrtj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3mriarszi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qlcfrang.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tuhmhdiu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vderfgur.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ivbaqboi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zckxyzep.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3thuzqpqh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vnfciwzy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3mjcnnali.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3cfudxopz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3olehzfuk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3jignniym.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rdqcjujo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3opvzbapj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3mkwieqsg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvjwtdws.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bzjipopy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xmpllbck.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mfnyfshw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3apcptlpm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlbukvhi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3eumdqudb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kxsbujry.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3umkfrmyw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jgegbtud.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ybrmmnnn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3sohgoafd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zsjdedrn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qogikdcn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3dxvelnjh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3cijgnkri.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zusxglrc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3otpddmse.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3gbfitfrm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3arwiwtig.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nfvjeoys.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3stzvtuap.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hlqhgkgs.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qlnkxiyq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hzaiczpb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hexthwky.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qpjyzpny.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3uafvqsjx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3gkjamtub.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkqlplti.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3blioszvs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3miariell.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xtnwypwp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3okwhzzqk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wdwizorl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uaelyrtf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qwtikgco.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vpjyuqlr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tucyblmj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jdqspmoj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ojdxlagq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3lskduonh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3pudrlrjw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3uxqepegn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3iacylgjg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wdptaqvq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3kskkpciq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lebfkfbs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pudtaztg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jqxrlrxg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3kyuvtaxc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3drhkrvqm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fktrhbxz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fpmibrqv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3oeyxxgll.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3tvunaltm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hdsqytrj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3scmlxqzs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jvvyqzay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qygqopep.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3oebmmwcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyswwvlx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gpiqwjvw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wlmdproe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fiimdtuu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ivcuuomb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jekqmiut.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3wytbuydg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3yyawxngt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3einuercm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pktriecf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tgtbtdmr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3iqgbfpcl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tdurkxqg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hpuumfft.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jigwcusj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3criksvvv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xaynzvxc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tizwscex.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ecukntrx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dechxerf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3uwbllhwf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3exbvkfog.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3uchrlyrz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mvwlwxlt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mxqmawmu.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3opzhskno.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qgeafhkf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3higbfdwo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vmvwsltq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rbuwffhz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kyxiedgk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3snrgtxjx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cwpjoubd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lossgvry.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3kngmebjg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bwratasw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3yyjxqimh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zbksgurf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vigmuofr.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3gkrcgxkz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lweygves.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3oddpybpm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bhkakqpy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qveydivg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uwompypf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjqzbxmf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uqzfbuao.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3gtpbgksw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xircgcio.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ffypuvfv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ucxshxdw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3rugrhalx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zkthtbkk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3siozzkxg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3dlieynoa.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zueyylmj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hpyrnwdx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zzgpgjgf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3krbkfmec.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zecjtkck.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gfvgdtcx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uypkuojk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jdurptvq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3eclwxwcb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nmqmiymi.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wlxcanyi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lunvqymm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3pphrbbnx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3qkzkfqbr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zbyfymzv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3romxuldw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wyxnflsq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3lrdlprbn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3osihzaot.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ucbryzdb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ktnxodcp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rqolqjsf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uiotflti.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wldeqevg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vweqproy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ynubrprb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ikoisifc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qhlbjqui.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3jqjchpxq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ljeelhli.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rqtcwjxe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3txnlgneg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3abxhmgll.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvopuckb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ucgdbggj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3egwjssvk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kzupufxn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhmoctey.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3czeocszf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkhtkfnl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ywlhxkgc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ynulcxic.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bwdrulbx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3leqgulfz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ldnnffqn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fiaguqoe.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3htqgrolq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jjtvfahr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xzsxrcjh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3sdmzkuhj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3emgbkert.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uurfscyq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jmdxguzm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ucvhlfll.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3awmuehue.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3djfsltgw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rkqqpfnu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bnmdttob.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3klovrmrn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ftnonerc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lyycsmjk.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hvixpubd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ekmfqvuy.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3gdjczknt.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3jjlcwogc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3gkmgnigq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3eoyixdgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ectxwvap.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gfdfjhad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcmepffq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3jowhgrlp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3kzuxjjnw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3zyiklsuc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fxpxrxqt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3igklgpah.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3llekrowh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3kjbmbkkj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3csfofhbe.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3hrrqujch.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bkkicawo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3impozzdl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3uelpravq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3eqpldgdt.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3llnfzhgd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3asdznolo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3bkjgfamd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3bmgurezo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3zppknzye.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3qztsuhhm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3fnvfzjhx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dlesnjob.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3xhakvqet.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3xypkjbbm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqaejtqw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3xcovtffw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3abcwrnhg.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xumaycxn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3hgmgsdtq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3agduwtzp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ofrpirsg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3heonhmlz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ombdebzk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vwydvovx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3rdvqwsqd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3rdiboacs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zsvfcykj.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3xqusdbyx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3fzaacrxr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3yahlgylg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3outggjvc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3dcfsaecq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wlbkwtzv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qbvzjplz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ayswruyq.html


<!-- 参考信息 -->