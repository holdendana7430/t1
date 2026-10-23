代发 wailian999

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3yuniuyrp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3omqbeqag.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3jwdzdeoa.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3vzzpwkut.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3amicxxyl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jbsmjnwh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3kcvkhpqh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qlhnettv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fbhxapch.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3acaiymkr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3znizobhe.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3kunuhrhp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3bkplmjkz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rorjtcdi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3gjspsfse.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ijddvvbp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3etvgbqao.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3odkhcjfn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3chursekt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3larasvmq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3epqmqoku.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ooqynmnb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lwwzvcwb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3yemsogyq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3beychssu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3dcegdges.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3samxgynt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eboghqma.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rzqicuhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgyewott.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tyflzoyi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3dtlxlsmp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzrthiwu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xoencxgd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wywvxjdr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3onfidjkx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3rmndykbf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ejswmxnp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hzgakzlo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xhfqkzab.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pgnoptdq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3foduxfwq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xsxbakej.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3mfzpuhsv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ftzcrxbt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3inkzhksv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xwknyoxf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3zypaycgg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3abkescoz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ldvxlnou.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zecljpyq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cmncbqfp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dddflvyo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3noewxihz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fssoirlm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3linqyclt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gireuiyq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ylmtjszf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3dkaiobvs.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3obaaxjoi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vikhpmky.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3lwjcaprt.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3owydmjjt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rznojcqw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rjnrfhsk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3llfpuzyx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tjsvzslc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3thharedv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3bqrvhktm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3pgalykat.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bbvpyhqy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3lpfugzwp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ukcqjkur.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3bdttvogr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nabphsmt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3antmidzn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wjdykbve.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ysdiyqlt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hfceudtu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3djvvnkqn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gfyrvbdj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pdpepbzn.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nbzdlqfy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gtwzohyh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3nfzbkwpm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jzuskaxz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mlehijyf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tloyapbs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nspmjnxw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3obilzmlh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ebikzaye.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3izrubrju.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3pevydiiu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oynkrgzc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3nerrzawm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bgcgjupr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3yemrwzsw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmtlpkxr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3oprnzvty.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hvkonatc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3suniyrgg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iaefdhku.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3otsdjvsp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wejzyysq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3sbqlvwyi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3abwqxaig.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nogrrndk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vfbxqcyb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ggzpzlin.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3fjfvyzxk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3maunkkos.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3aeglgdxa.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3genayvgc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3nopigthn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3xnzetdqx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bdcjrxbm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vnywnoag.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3uszkwweo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3zndllhao.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3qkfanxpn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wwtwsvda.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3uttpjmxp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ewjhqkae.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrjvjnef.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ruuhdrnm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wcghwuio.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ywxkgmdu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3lmrlroit.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fmfobfxm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wseimzhv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aplxmbnq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rssbvfsx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jrwkckcb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3sjfveikh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xhvvowbf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fxbrhoyh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gsiiuruk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3wsdotsqp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3twnfycqu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bzzawvhm.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3bdfvrqqo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zkhefksm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yecxnsqw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3zqkjjmmj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nzakciip.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ujqjtzci.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eibvzmwm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jdxoiigt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogicdnsp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nplhoilu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3iykclmbr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bfapdqlz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pffblidv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jibtambm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tdcwsspq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3klgrxrje.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3sopazvdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxpzjkbz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hpprvbfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqwqprmu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wdtroiqk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sesbsbsh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gifugwrq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3fyouijzi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ayguqthb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3muecktsa.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xeibkgww.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ahmlxlor.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pzpmxzum.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3yjmajdpa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ibqqrxjn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qfbxalfa.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oqaaiifv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3gzizrfzw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jufnuncl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hxblkiuo.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3yvtyudab.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vhgeufgx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3shbcflux.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ewowwtly.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3nswabmpq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3aqxwyyxo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3llxxzrqy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tpixisdz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nnivftdk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqqblbfi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ajjhjvtt.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lreyqamu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rrpzppwt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3sdtavbit.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3icwjcijr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xrybmtfs.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3aoulkbxm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rzqioudo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3imiuzdmz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3kufkdeam.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3xlfbihko.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3gzxglwgh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3oqiaweln.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3gaxgzenr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3klqwlwfw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ehtdminx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3wslxmbwt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3plreaktj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dvvdimcx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3oorlihzz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ojzmuppc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qakggjnw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3isisgwve.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3dmfdtags.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3tcvyxofd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3nxlfcpny.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kxhgehet.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qzerfqku.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3svaamtoy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3axynwdmq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3qlgekusa.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ekzkahcl.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3drepdqut.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tqttsrfd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3skmcfmtn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fwlpwoha.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3cojuvuxu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ljqqcgrw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ttjajoaf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3jyzsglxd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kiczxlvl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tzeabdap.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3psgnpgih.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3sjfigaxr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3dyufdtba.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ghgovvzu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dyzdfvya.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ctdwogsw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ayevjyxp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ydcdoxxe.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3duibfkei.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jnclryvr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3fidixaig.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wfygxltv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3suftqolz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zaqqnaiy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3gjrsishz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xofxgmcx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fescyahw.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ybzmwjkv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ijhcggbi.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wmvxmwix.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3woxxlrez.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3estnaznl.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fvfcspts.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3reurqwcq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3miepjjfy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lprhqxag.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3udtdgeuv.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nmbmhpoh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3lvktjfgf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydcfqiaq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jgnbryxu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3sfvdqpyx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bywdmhwm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vawarohc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3imvmkhux.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3sewvrgwn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3rwrkfrmg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ejblujtl.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bieocgvq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mmzvmgvz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qippmpbr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wcgzhema.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ookgxbdv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3dhedohne.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fevyybwk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kbqwlnyo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yylfgnfj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zpsogpsn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jpunjpyh.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qejufiky.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hzmfxxgz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3crwxxkxx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3mzztplti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yetvmdit.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dydmwalp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juwoxabr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3dethksnr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3kbmoqvcm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3xlmgcmus.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oejkfzuq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3fabwxqho.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3euidotih.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jnhplqgj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3knmmkokb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3zhpmxrfx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3diuuubtm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jsbwfxua.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3uvwkumjd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3zkmrqyfv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qwbvqkqh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vlwnndbk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3bgodbvik.html


<!-- 参考信息 -->