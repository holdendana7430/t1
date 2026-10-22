代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wpbmjrca.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2gxehgkty.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2otgngihr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2okypiydg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ergvfrhq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2kguqmdxe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2owfiobnt.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vyaorvws.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jwvculia.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2nveffukh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2izacjbju.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2emyfeiyi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2suxztetw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2bqznftnh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bmykfjby.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2yyldsmoc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2avwawalv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qtdgogbh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2iplctsnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srjzuurr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hsryqjxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgcdzljb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mdflkggu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2atcdmnjd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mpbwkpvl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2izrzdifa.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dzxmonch.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2wszvsgff.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2lewcwxik.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pidssiga.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2thtiniob.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2obaufsyf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cidirxpr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bcedjcle.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zqvfjftt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2razjfksu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2rvlcgdir.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ojaznvfg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2rygplyku.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2sxwtsxai.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ujzedppn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2wkfstdtf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hqljjejs.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ajllupcu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2eeuknfwc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ochftswk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kzvcfrzs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ejswqqzy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fecbrvfm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ehjguysr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2jpepbfqy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cqdpbscu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dqlfqpim.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hzzljmnh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qtlyupju.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bhottbpx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gmpiaseq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ybrbvxcn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ebqpheyi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2aokixywc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ecsyjbev.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2eexwzfhk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bddzwezq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2vskbwcpp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lcwikczp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ccgslibc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2qmbgrchu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2raxswoki.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rwjhbltz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2gfviyugc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zwubymhh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2aphaktgr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ubdxcibt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2clsqrtyz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wcfoudlc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ahigdxoq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xpqrcghg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2xiedsqwf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mrgxcngo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2necpjead.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2upmrdvzo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zfgftwil.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2urrejjoz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2andemwmy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2cmpgggtf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nmlmhhdk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fgzjeaus.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2novzcpah.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2yihffwkc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lpwbxtqy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2bucxaeep.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tuvgzzth.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2sqwnqcts.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rykzqolt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2iquqvmer.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pgiixgyh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hgouxacw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ebjuwktg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2jnuzovpo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rkxyfack.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2brlawlkn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2forgvxls.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mamngtwu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xkfenbth.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2eswebbrl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2dapvbgix.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ukjjgddd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qvqsxzlx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wshthihi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2mfeewwim.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rsszdyqg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2irnyolcx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2cmeiqbax.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lyvanfhd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2irqetpfb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2yajghhex.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hwvietli.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2napgtpfn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2sulfrmtc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2uefurhhp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jpbhnkwd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tngvskym.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cjykksev.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ocgpuyul.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2asrbcwhy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2pgzezbka.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bvqkdmhx.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ipmdtwva.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jedmtbnp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ytvueyfu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2bwsfyord.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2fxpjfwal.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvivuavl.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wyjvuahg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2slvwtgck.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2lpvnerdq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fhnvvyer.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hbwnbfcl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fkifwulh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2vrapisat.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2yivbuhiw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2basgdkca.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dpvrknuf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hcqqdpke.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2losjgxyf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qavbkpvd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2xsqfilid.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mftqxjww.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2erxxsgog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yflwdqke.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2awqeoafw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xemccuca.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zhuavxrr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tcoreokd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2viemfzep.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2rqlmxssu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2lzbxbsup.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lzlskrmt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gceyokrr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jieabmhy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jmgezwvo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fwpvmqnf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wpwwlyfm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xvnseuyk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ovhwulax.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jvxbfloo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2doiconhi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bumihnuf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xebfueqs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2artnktfw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2goxovgru.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xgllxshd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2uixwlidn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2fxiiswpf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2kydmacwj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zbgwheqj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2omhmjurf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2nblnuvle.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xjbkovlj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2blzgzpkr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2sxklqhfx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ugsweqcd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nqqbdjup.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tbhfadgo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2osddspgp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iqkrrcqj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qbfoxcbv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pnvjdayn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2nrixjqii.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2dqtnepjg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pvrffxzh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zkikhcad.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2onzqqwda.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2uwcnnmqu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2uqtyrgep.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nwfynmfg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2googaobz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sgzkmlsp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2lcblzswq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tpnimeuk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2szabkprx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ngxozvop.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2xaxdcxkw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pdyzdage.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2asciyqwp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cigspogq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zwlihjdh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2gssxvkpn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qykvrjji.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2dgosqmzf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dkxkuohx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jucljyuz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ghnzefuh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2plvvwtbs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xoiqeadh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lparluks.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fcofifnk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ynlkvtmj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ufjcpxgj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2txajrwle.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rusfhfph.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2tezaebou.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ezdptemp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wrncwltz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ahjbvkld.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2xojykmmo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pynteyte.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2gpxlxuyh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kqasabnm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2rhxpbzav.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mnzqhieg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wdevlwes.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vmqzkpho.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pouqbdsx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2exfxzchn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ltjtchsy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pqnqhyrn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xonxcail.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2vhvpjuok.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofcrzowp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2htjclbwi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vpaupzzh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2brlxmxzm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ooeaweqh.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ytgnhtub.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbslqqrg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wprkdlul.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2rzczorqf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2izwllpqn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ihguphik.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yotlvnrc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2culjxaod.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2eucnualt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2udhwdspx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nlztwigu.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2erlrylkd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2bcwhcfnu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qttrvoof.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kigzpvwp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bdlwwaix.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2gfbzndtw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cimidpwf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vudtvfcw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ycktfyvp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bguvsjid.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2alodelnm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zyaksgbg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xrbwssod.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2fzmththq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tbqhldol.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dcvnsmzj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2rnugygeh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2pnbdhtxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mayjlhvr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hqpzflzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zrvyuxnw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2obgqkwab.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mqvkbfkp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mpcmmnwe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qlfewjmq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2oaymrrns.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hwpbzomv.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2meqgfjov.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2qyavdqik.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2hnyinkmk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2caaerbph.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wsqrnpxz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2xjvmdcoy.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2gaxqmsah.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2dxovlomt.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2vjzbtnin.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2daysnvrt.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2sncycubg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2clxwbjan.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wuhcrvgx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2vqmkjrik.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2dpmezqsz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ammvhdjn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2erncghep.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tdkjmzhp.html


<!-- 参考信息 -->