代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2svxubehm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jrycwyoi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vqaqqbht.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2dxcfsjrj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2dcvbuvvf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dxszplpa.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2enzweehl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mbxytarj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2guseorlf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wmewmukj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2lfgtzjvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjjdtaoj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2equwqvct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbfbtqkb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2csduordu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ewjtoyin.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqcjlygt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wwlvhbjz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2kdaxowwo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tbyogdtw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2eshustvp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2fmhopeoa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hbfilvuq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ahjlhnob.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jojpitlr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2njnpdudb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2uprzsubk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ifbudnkr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hqthipyt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zcltzugj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xawjjftm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jtejtvin.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rltrkvrm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2aejcsmrd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2gtujeifp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oeehteoy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2oifjejfl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ijdztfhq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yofqykul.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gouxclsk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fovjxrhl.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2hiedhwcq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2uxajfxzz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ybajuwfz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2wyhtfujo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2downjusf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tlsbsoqu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2pnnonmha.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zxqvsozt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zlciazxj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mqpifrkc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ffgwiewx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ywgxqckk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jibvpojx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2quxnnygz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2nbnjifgf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fhyewlwx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qkivmkoe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2autszghn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vfvljxbk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2purohtys.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pahpfvzv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2hmdyukhv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jdksaofi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2vgqvjpcx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2bkflanfv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2jfrnxjdl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2htngqezj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lqbaannv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2tpuarhxu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xlggrqri.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ehmelrwg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2grgmgray.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2nnnfktkd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2cuxgdppj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2mtxchysm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hsixhawq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ypotwkle.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2bajedhrx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vlacqwak.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wqqfupaa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmsqqznv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2boeyqeay.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ejngeiay.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ojcbmufc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hzsepglg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ttjfxjsv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fwirqtir.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2fvmvepei.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bhyjmbah.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vdfcejsw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2trxtprqd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2wxwwkvlc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ckcbgwtm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fthvefpa.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vzqesoht.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gedbudzu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2totzqide.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qvyuqxfu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bjgspmrz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjpvecta.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2iyfveptp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2pwbtwzql.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2akhgczlj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2nbueyejh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zxejbrza.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2staiccyq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytepqwgl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2qptgblns.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2mddmsokh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2apgqyyxz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcddeqtu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wjiauajp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykfuvifl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eucdapaj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2xbjhdlwn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ssaqecfr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tlqsdoov.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gnhxuwcx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2lwavirvv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jbkwjvcl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yboqnsfc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hqimgirb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2eofxiukm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2pmelwzar.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2pcfrhkkp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2vukzsoho.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2aukmmoxi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2kezpswiy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2etwliuyg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2cchwputw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xcvvwlkk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kieazxqt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2tatrfkcs.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hhdinkub.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wgoygtqf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2rhqdhsny.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hfbhafuq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2buyxzbnt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lpxyttlm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2iqvscisq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyvvmtdj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ybohdaqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epuxmdkq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2odqhcmfa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nrewfdgr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ettxmgcm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2fldheial.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2tbmnljaz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ksdwkyvn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2iyarvfsw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kcasnezc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qykletwy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2nprooqzp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zffhlbzg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ptvgseix.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rmsjunve.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ukcmcrhh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tzirsdyu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2syqlkdxe.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ursemsne.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gxdfsyaf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ncgqcxym.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2fajjpwfg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wqkedjjk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2turiamvz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2bfjakddl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2grbykwpm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2tjsoialk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lymedqlz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wwscxqtq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cgqoiyab.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wmzlqnpz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gqoxdhxh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ysvywgjy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vrauyyeo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ysvlyuos.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2gccuushp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bqkvgcrk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2nejkqsdd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2qrawnfkg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2urdekhnw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2yswvhqkf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bfypycnm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2kojjvrwf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dncagozj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2avawxdlg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2jhwtrtbs.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pmsmgdmx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2upylilwy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hqfpkkwy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2djltcgck.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2pambyqlf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2grexgjqa.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2xpzejcsg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2yacqkqhp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2sxoyrpfe.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2eubnipsd.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2iapxtgbe.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2clnhbmpp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dyibfudo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ujkiawyt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2sjfeagsz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2djmoklrx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gvlvczjk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2azerooyo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2yfchwftb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ywyekedm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2inwuidbo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2lzrdjqgq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2grkzzash.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ptoiqfgb.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2qzmuiiep.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fadzmroq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2avmnjeko.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2pgumyibg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wdozpzvb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kyjtbixm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vichgmfm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2cjurjibc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nlibnyom.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ihznnqxw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2pargebts.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2vnxqrnoi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2znqdlker.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2spvthavc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2faekfbmd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ojlhhcnk.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2etprtqnh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2zbvuxqml.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2orsrwrkx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2thrhowwv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2rtezwvvl.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xswhummh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2pqfdbsxe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkisnmli.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wghmfzqm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2teymztau.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2fhmdhsjd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2iauufkxq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2elsmjdyc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bptmgqkc.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ttgzeqeb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2isgoakcr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fjqssrjl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dhcltyyz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jlxeagrd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jjcsobxy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fyfgbfxx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fgiaoyvp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gofipgvr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lxlnzpby.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yojjlyvh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zcxdyivi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2epnaohel.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2lxbmlpsi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kwbgavah.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qskeoxlp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gjvoauvf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2uzzlhvto.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2kmmwpitc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2jqiytqse.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2etvplqqx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hcdhjjge.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qpjtdsys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cutuvlec.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2owpdqhll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqgenmnc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2wjtwagvk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ruukksyj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qtiqtvqm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zdynxejt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nxzjuwlp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2cgqttvgm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2uoopvuvx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jsmseufo.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2thoznnzr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qqvjsuwc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rhkvpcfq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vmpzbtpu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uhhhpkcu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2clfudgxe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ifklahcd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2fccgkfar.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2xgxbnnxz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bpwzdlrq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dadwgxlp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zxvdjzrt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2retknhtj.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixxgljei.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dnbisksd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2btuttkaz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ftsxkwef.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2mrmbgjdq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wsxebwil.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2hfzvzyto.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2jfoupfic.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2zizxpnah.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2uglfctrx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xymjazgb.html


<!-- 参考信息 -->