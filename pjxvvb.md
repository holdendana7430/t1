代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jfcxjqjl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3pnlgncag.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3cxinrfsp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3czoqbqyd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3whhqxzao.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uzgfzind.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hqmxuabx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3opqvbjeb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zqdwmjbo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3lfynhbdf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3epqfczfm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ywvntlmm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3fxpmvkfn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3pyrkxnis.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3esjkyvzr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3fcwdaria.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3reerwbrl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ttmnjvfk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ihmpemmw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mvzwfnzc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nssrfokw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ukexclsx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3rwrbibke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdlwlggm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3tukqrevi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uloocsfs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kaybixar.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bjmpzdru.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjyjsigx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3bzgcpcfu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mnkequdo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ciuhacrn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3arisxrlb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3isvobdxf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lmenswrb.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nlpvssrq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tdgrhnnp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tsviymwf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3zdlfvyyz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3upuomhlc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3xavohyqf.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qgjsnrms.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3dququbik.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3nkxdnzuz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3vqfzrvhu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3amnezkmw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ggvguwgj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uzetlygp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tvzpnlur.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zsibczdg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zhanhkfq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvbqymon.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3exxmcpxo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3tipsddhu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3frklhdpv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3smpwhyxr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3thcvtqlf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3vxaxixnk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3aebjprqy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3exdcined.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3isfrogpb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wmbgnfsu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3gcmdulnd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rtcqtfgx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rkzwsllm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pherthxf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3inviozza.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3foionufj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3tqprodml.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xthinutp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yfxahkgy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lnmixcss.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3gedqbptj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mshclvsa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bkmqqqrk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3eiblrfkq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gbasocum.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ocmtqepr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fkvqdquu.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3thyfzmcc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3eczmtzun.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pvdgwqjw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tvxgayih.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3nbmoicyb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3imbiaoyc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jnxuafuo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ttfjhgxq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3nmwuhcgp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gkgfsggb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rivftwqw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3aymzypmj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uippgwfl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jdyatoxb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfdsyinl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cqgtagtg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ncaqpkww.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zmnwcews.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rjtepmhb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3whajeaeo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3veucdbwj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bhrdbcdn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3netsahco.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3bmipztvo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ovksmgus.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wdilkzew.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3iebmbpkw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3adoubuik.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3adbpdlgc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3smqgheyt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3uhzqzjfp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3tcsmwdxb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ifgmtvmx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3nhomxkzq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zihrzlnc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3adjdsils.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xsukever.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bfpkctmi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lmtcnbzz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3fmvvazhm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3yywcctks.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3zndzekpx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lphqhnqw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vllxtuys.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbzzypvr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xoqvkkqe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3efjezzxp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rgjqquwb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3culqatim.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yjtnxpvn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xhkbqadp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3henadvza.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vyoiqvzz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xaqliqcr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ragrhtgg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3iuvzrgms.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3gsyseytw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xdvkwmga.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3virabbwe.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3aomdkgso.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3tkyqrglf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3acrwfmwa.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xsrfskgh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3llwylfvw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wvrbtvxq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zrraojkc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3rdlwggeo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3chgijxjj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3vzdpoimn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nlajrhlc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ttcanmew.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3yglnnsqv.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mnmltiuh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3muvgdoyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgkklrfo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ysdvyiik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewkbcreh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3duwrshtn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vvawvlaf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3fwlwgqxj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nfxdsibr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3yiztteor.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3oofkiwzi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3cvakkjqs.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3yikesgfw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fibebtun.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3cvcsfuqh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dueiffcy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjxejqs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3htszduxx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ybqduzcg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3yqnwupjh.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jegfstmu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zfbengbs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3trclfqby.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cmdspdik.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3paggtrlc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3xwuwjvtq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3fibuxapr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qgaveswl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwxoitbt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3uqiugnqz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijvplxat.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3sfkqzafo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pbvxlnhf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3oqixrenr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3pulcvbzw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3afmimzwy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wfoxinbe.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hkhqsjur.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3aoxulqbj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kaevetzh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3pghkljhq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3qddpelxo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ecbnlqra.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3mxlnzskp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mrcxdlld.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xrzgwzfn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zgzbasly.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3arrhiacn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3eiqdohfb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3puzhtsuw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3omtdffqa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nvafacis.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3shwjamhs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3luiimhtn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3bbxfkaer.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qdjtqhwv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rldywznn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xnhbscgo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3cseemovh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mrxjbfno.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qmkytknl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rhorsnpf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ckaedbgt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jjpadvyh.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pysdvbir.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rifffgpz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vfgztvkf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vekbglob.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ucbzioks.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mbejpcyd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mxddkyaf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3qmgepkbu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rotufxli.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qdtwjdvm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3yqfuzwyn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kwpdcqfb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3hkypbvel.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3acudrlmo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hbfywyhy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uywbwjdu.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3nuxyfmjl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rjnhnjzj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3uhzmerrh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3nhjbibjf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3bjscpnos.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vsbwzlta.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tgmdcbnb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3punvzwpk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3pkjvfkog.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pneihegt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3kurtrhlr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tsgsdqxb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3mehgptdc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wdzkizwx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bmripsbz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3yzgazxsw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3voausnir.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zmjhhfgr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jjqypolb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3wtnooiax.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yxmmmjfl.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kaqyirqy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qvfsfmbd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3knrcelgo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3mrodyfkw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3zyqsxzsw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mvinjwdy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dyuyoixy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lsjgukga.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3niualsef.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uazhivkj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kwiuvzys.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tmhqbsug.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cfrzyjqk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iyngrgdo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3yaairmcu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wskcvlyo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3roablfzy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ptizvimt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pllyaxuy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ijckrdls.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vaxxefhz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dgwhiknu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hrsgbuiw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3oprryvjp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3uyrhndra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjcjodxt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jzwnfnzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yatbfzjy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3laddbixy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3nzichtvs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3fnsugffv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3muadnrhr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ufikblie.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3geeavrzl.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jokpwccj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3jwpxxtno.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ixxbxpcr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3isrigzjy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3aryykmbv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ieaavtlf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ikyevwbs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3xjpczlme.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3xeibjomm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3yviyxiji.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3hcfoolie.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3zogyguzj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3iveakhlf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fcvobmqx.html


<!-- 参考信息 -->