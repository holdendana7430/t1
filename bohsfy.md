代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2esbogxpc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwxubtdi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ufzojcya.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2hsnskwdz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ogiiooyc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qwjukquf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jhqlncea.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ixpfonch.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2iebgwgba.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2xpejlmyb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kuditwsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxedioem.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xkegespw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggsyfsby.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dvadreks.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2sofrtiyl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcsjqdmw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mhizldpn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ghxhsble.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xxexcaxe.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2okkcuzhq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mrsdadjo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eciyfynw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jfhmvyzh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ygbhwdmq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2foeldzne.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qvljfkow.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2chhecxko.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wocezxom.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2wbkvbdzp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pgtjbrar.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ygyompqk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2tlfcakjw.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ylgqmfbw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vldpkffb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fjnoaqat.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2raueixms.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rhyvrxaf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nhytwjeu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2mfildtcf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jtjpoxym.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2hndeniuq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zthkshsc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gstxcwoh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lwykloax.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2azkgowjh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xmjtplru.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2uaxmkbpd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2awukykca.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mcwkghno.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2knmcfvtr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2znhiqmjz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zqiseoux.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2aemhprxc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zpgdnhgq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ptgtbhmo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2indhtfmt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vlflsqel.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2srcgjqfc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cqqqqein.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2tmjstucf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2buajhjmj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bjzhzuzd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2oaerqpdq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2zkojodpu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ouphdxvh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2venfqzig.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2orslrrkc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xfjxzwjt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2opkiwtnq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xkioporc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2itigived.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zjmkktxq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2yvfxalmk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fnsttito.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2tdwvnhyl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kccwmjml.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wpwlyose.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2glvosbun.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xsdmfmxl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2sznysjef.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2hrmwwzxb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nmpopstp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2wzrxinkp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2roeojrns.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xqsssddr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ialqusap.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmzkunrt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2dpclxtom.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2girbxirk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fyuntjbn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kfjauksh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2nkghmeps.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2edhhsqgx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hpgxpdrn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2twouzfvy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tbwlpwvx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2cvhgxgja.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2fbxacvzc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yqysorci.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xuopmtst.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2uwbrxdse.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2cehkjioe.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jrmnxcdx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2neeoalsx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hdkvjpdw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gpusbveu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvyhejcg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wlxmjewd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2rtpkznce.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ioyjaaec.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2uxkqmpqy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kjbwkmta.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhrmpdak.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rrwvsmgx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xqiqajkk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nbppjirr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2itjukwsa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fmsmsvya.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2qpwzmyes.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2srbxxqkr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bwteyhfa.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2aqbjwfwq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wbbdzdph.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ryxnjado.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2iphbpwwf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2anumfnqy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wimeuicu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2isntmjbo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lgicxvmt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kfkjcyhc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2aauycdrd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2chnuqbmg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2asqobmol.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2fqwqcnas.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ssfcikem.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2clsdazid.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2nikrvyjf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2tvbaiakv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ydwqeyfb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ahptofiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixsiizja.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rscndqdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evemybdv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2relaaiir.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wejdaviq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tvfmzrdy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2chcnaxzc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2kezuperf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xkvotyxg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2blixaqaq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wubmdgrx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gmullndx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wvqfhptx.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hfkmfoxp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vdibtjzl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tbiiipph.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2akmnrcxo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jlexfsxi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkpjjpr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvfvflbf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yrqfuhsx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qnasqhug.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2sksucudx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wzpcrjmk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fcqyhxjo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2zcymklxp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jpqoufyj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2luempdfx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zkvddfhi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lkksnsdj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vvtsrxnw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2cblnrbbm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2efseunnd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xngvrrlz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yiqxrorr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lmzbxefz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2dmudhndi.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lcmxueca.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2mzbzdkqy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oroqnruv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qzgprhyh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2erkujhmz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2jzldcdjv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fgvfqahi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2nmglffpz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mclmslyi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mhftychm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2inrlgmfd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rkaaakyn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jeqvjvsb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dguxygoi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2vrehtheo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2gdzommod.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2dupkcpok.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2deentlkr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2xgeqtvvg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2oetkfjkb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2iwtxmabs.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2llmxygbo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2zkvjhzsq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2opoqvlkx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ctwcqhgl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dajjglyb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ecdxecxh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ankqitct.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kskdlqsy.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2lrczmwgb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lxlibwjc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2egwyhhzp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wpbylcdl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2wbyaaqzn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2pvjqrchv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fxvauwqh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2rgcdkrpv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2giwwbmer.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2oruqbndq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ztkrusdt.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2thczhezx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2fbiroyzc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ozyehjwp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ctcndpai.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jqgswlza.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2iqqdhkwi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qrgmbrrk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jjagwjbd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pzyabojq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pawmyaqi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oyclmavw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2uughgsxe.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2qhxhxfjz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2txtxkvnj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2byygdkwp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aegzwoyh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2scnvdzbb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2njfganql.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2aueazlqa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2szssaedo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2cblvmtmy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rkuqtdwg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nviggscq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cscjyzfk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2iewaxtif.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2yjyzertt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibzfmqbq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2phdoivsm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2khpfarbh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lhdofmtz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pgnwpvaq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ftbhxizg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2usnifkzz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zxpojeqr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hjbsqwto.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2shukbtxb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2msubdccz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2aebjtzaa.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jsvpxvax.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mysrwfks.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lkzyrrzb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wphslfjf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2vehcvcci.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2plgeysap.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kmqxsxsh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2wjyyhczq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ytesrwag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwhqzyzo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dwjgitnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fubscowd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2tqbkhwci.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xxihkwml.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fecenwyk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kgmtgmzi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2dibkmbup.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vzolmvqw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2fkxlumwy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2hnsiaxim.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2yyxkzhho.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fxdxnjdy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2wqshezgy.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2efzulhzw.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2paekwvfa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2kcaozagk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xvksdiss.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2rrbadxrs.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2tsbnudau.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2mtuzyesc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2zjcfbaqq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hfwxjgjf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mojzxnjf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2amtadcgz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jospvghh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2anskluir.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2tjaafkgq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zkzgrntd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2tbvdlcty.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2silpyqaa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2rniviplc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2wblfqufn.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hpddmwiw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vdogpobc.html


<!-- 参考信息 -->