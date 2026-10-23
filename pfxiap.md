代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mtzdbozy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gwflfovf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nmqirjef.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sifjjtiz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fytjapjd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3iflxyliw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dnfkuvgv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3cluehifa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3techeatt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3dnzqcdkc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bdvsungg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jsyandzb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3hdglyrtc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3smmihsum.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fctermnp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3vytztwoe.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ahyabjcx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3tsdjvjke.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bbekjhmm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3rofcymvl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3mtorwvis.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wcswdjhh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3adsvyhjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehfncdis.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pxcahylb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3godtjnex.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kyvqcdcb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zyxqhbhw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3siixucde.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zrauyjnm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3gvzvkwod.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wnzpbitt.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3lsbwxmng.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3cysrdblp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3iaeaulcv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3amxkldlw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smusjgvq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ffyremno.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3sehwclif.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3wxursxhj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ncahdwtl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ktjxwpqp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ogiastja.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qcbzfumd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3hdljzlfu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3elefjdst.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hexaylba.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uabneepq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3acfmlbng.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hswcphqv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rbpqvnwk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3eerddspu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3frhvrlrt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cihzdxrm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ponuscwt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eksywdbg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3epucqrib.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ykrsajbz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vcfxcviq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3yhquvwjj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pfkexvdl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ptbidduv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3enybiuyt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3yzqwwuyo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rsrevpky.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hsmvvjbt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ouuuqwra.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wznwxquv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hfxnbept.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dzcfwcje.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3wcfvkqep.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qxredbsl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mqjurpfi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3juvtrmoo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vyyjgsfu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3kcopbttq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3jebecyzb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kzyrzmtt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zfzsywzn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3lakjzcya.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3sqpejyrx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vhplnany.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gwljodya.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3omygkooz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wusfwmbz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vmbkcgvh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3lfpxgjxw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mvwcdxus.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lfxnlney.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ywjwhdea.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3fhrigatt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hitvemko.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zpmdgyak.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozgsifky.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dqsvmkew.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ymvrewgf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hbjanudo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3spourslb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ablbwwrj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjofukom.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gwtzfdgd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zrxdehdl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mbscqnwe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ooprqdwz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3klicwjlc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bsuodcgr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3flhoihqf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3oftjoptr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3anpqttxg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3zzgkeray.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3alipebbs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tjduetoi.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xnyowsiz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hpdidtno.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3mpagzcoq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3kmdmopix.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ewzbqrsi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xvxfuhnt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3lusubodz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cqjkniio.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lvrkofpw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3lvitnfhr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3epzjvaik.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vypwxncw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3chlwjybq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3bvkvtekb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymfyqqob.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rbvehmvv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3obtoezjp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3shvztsqe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yzctbohw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3uxnfwmip.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vtecgfoq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jzijuymw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jqthgolh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3szjgyjla.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xntetkjb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3omqjkewn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ddgddptz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3jjebaczz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ybofmetr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ychrhmpa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vkiglvgz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3nvqqbncx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcqryxed.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3adedfnwu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kegiccdh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wjjbrxph.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3oljznzdo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ifsylgxg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3yrbdztew.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3yxpsyyuw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3egaimbsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uzcqaxtz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wimrpvip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyurpoji.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jvirmfsn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bkpquiye.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qxltprox.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3isgucsfd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ksjmcjia.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pkfpeudw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fzwkluzo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3wmosltxe.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3anradfrf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ipuobawq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jbpejqwz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xmzthbva.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jajmxbcv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3nqlfnpdg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hbeszzmg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kivxqegz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vuwyfwor.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3znpmfaro.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ijrzknyi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3rvdlkgkm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dyuxjuvr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gyeuzelw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bzzreiku.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sgqvhfwn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3gaxwwsae.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3soluwsez.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qjpotiov.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sosvjenb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3okzldzih.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3sytjpesx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kssxsitv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mhrmqakl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3timbxyve.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3znvwdnck.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3inrinwtd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3duapnisq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3emuwwhki.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qaudktxl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3kfduqxaj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3nzorhlqw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qdlisylb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3rnkdrabj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3bdaapaoz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rwkeiqet.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hgyemqxj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gxkfvmzz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dvpcxhgt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sqopuyhg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3gxdieztn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3nlcwvkxa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3hffmzrob.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hruqguju.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3plsizfnf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ffavumhm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dosoxhbl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3nccczshj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3skyjgnwa.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bxbawltv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wktcleat.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3cxzkfvzl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oobsomdu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fnspvjxf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3btvxuxrp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3yosnrihw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fenmzvdn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3etlxnohf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3caqfwkdr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3zvnzxqtv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wmmeazuv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3bafjhnzr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmjfcfca.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lxjofxzr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vvmlciwr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3epokexbw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3azyyknxo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3lorxstjg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kqumitnx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jdmkkzhc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3iwrtrmzm.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ebleqztt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pwmjdwzz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3yvpavywv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3uwdlnuvj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cvsfvycw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3adgheasd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mkmzcxpj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3vjmqwyir.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ukjqekdo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tuddjpvg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynaqkkjq.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3galkqhag.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wikxmdhy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ouqrxuoo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3uefpttja.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xdkehqad.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gtiappaq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3kobggved.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fteilftj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bfmdcjfs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mfibqtbx.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3icskfojq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kwrckesq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3woqvgrae.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3wnkbmyha.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qlsfsidd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3peecowxy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bqwomjhj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3psccufal.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3fcznvoxl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wthctdfy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lumepssx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gcbjeisc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3iyogsckb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qmlwdeyv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3rrcvsuvq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3bmugbmpa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bqqzvdxu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3twvayucb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ndgngjan.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3flmsrqej.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3zhddtgos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgqdjcfi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qgpbtjme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqpevymd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3meoxzvvf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3jscjlhtu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jibunclp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ookwbwou.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ifyojouo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hnuekhcq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hllvfcma.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3jyvkokdr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rhuwnots.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wwocqnmm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jvylmeir.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3sseciejc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ryokglcp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3toqvbshp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3dappakht.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3nbgbdjvw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3dxsckhtb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3qfobsgai.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3grbvdxwi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tunywtkx.html


<!-- 参考信息 -->