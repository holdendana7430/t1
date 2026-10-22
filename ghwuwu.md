代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2lmdamsfs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ilaykvcz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mmcugobe.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lfftjudv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2jdrsllgq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dxowxwjp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hmpfwytk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2gukupxuh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2fctfhrvh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wpgabwaj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ihzyknhn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2rgbqfqoy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2seqtexaw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucnfglju.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pylwhdzn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kcqtgrbp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2cevflzwc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cixqibeu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2rsrjtfqp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ilhwvwhn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2mabaurzp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2gubqbiqi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2foctbetl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xakpjrki.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2tjfklzbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntwnnkbu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bzyqrvfm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bowpebfz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsyvomld.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mbrqcyun.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fnnbyktr.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ehvywlih.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cslwxjfh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2akcwqxij.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fofymilb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ttmavxqa.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmfadtx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yhetyrti.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ydskywes.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2owdqcfwu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2vjugkmah.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ppdcnyrk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2nbzwguss.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wggwwczz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fnktehvi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fcslikmb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2bjqupqaf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oxokkith.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ozilovft.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2axlwwjdd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ipmmlfjo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kcoodjeu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2sriowgdi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ktsewwgj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2dusnvcok.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rinmxyql.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2sstbkqbf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2uwrkwkco.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xbqywuow.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2kqybenog.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bqzrxepy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jvadqdfh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2odwqbulx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2epxrlknu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lbopnuzm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jjbkwjmn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ycwvcler.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2cxpurrqk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zewrdwvu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dwpnlxvx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2herrdhut.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ttxqwghk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mbglbsnj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jtajupbs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bmgfvbyc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2srlbeoxd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gdklikxc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2yhcjuhxi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2lngljnkj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2tphjpclt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kxkygbkn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2nlvfbtpl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2isrbnomx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mazvyvsz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2uyfywekf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ksmvkggy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2iwwpjhih.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zvviqzjy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xkojljxb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2umdevybk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fwljpnyz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2smudsapy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2txhkljcl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2zjegtxgl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jtzuqsug.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2irtzjhse.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lxtpcgnw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aoyrxqil.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gamjyxxd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rshgopti.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cnzjtdyl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ofiqpbgp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ymxjvpme.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ickhbspz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2odbswgqo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qutysegh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ifhpguda.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rjsbaony.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wcgsnzwg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2xguvjpcz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2fesefmvo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qtbdhfdf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ngfhguit.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2napypjln.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2rxgmphji.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ghtmzlfk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2sncdmjle.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2brbnrxyk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qwoobfdk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2sswzutxi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ameoaonw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lmxctplk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2qyctkocv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ytbdtonq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vcnmxjce.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzhlzxok.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yjcnksyl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wztfszal.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mdzispmp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2heihiltc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ditszhcw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2cnitpzjo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mqqnetfm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2hpsdptxc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2muijtsmr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mbzkxvka.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcvbpvic.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2uehplhzo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2nitcxhwx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2knzddktx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hywfnbrx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2apobdvhr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2djsagnpu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xjmsvdld.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2vqyrtduv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2czmjwzhy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tlfinloy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2adnfeedh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ndepyiko.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2fcrhqayg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2eyzunkmp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hxqjndgl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xshlqbci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuddfcel.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2izcsunaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgmebtck.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qnfctucf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gsuvczhp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2nyvmkyjs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2bkykubmu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2tfydzkej.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pcmnvrzu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2fqtqlxcr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2oaagqjqp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ybldaeeo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ikukblah.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cbcdsiod.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ptqnftfx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tffjjynu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ubcnllif.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2vurapukq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tuozumnp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2scdkrcaj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ulvhhblg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gnfufomo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2vrzirnut.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2qvnzxxqn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ncyehcoh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xkbhexgg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ftcgoubu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gfdrbtjv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zsxrabyw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2koblsvvs.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jisprqgf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2srdqpwgw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xtfpdnxt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2azrxohea.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gyujrgai.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2aeqamwjo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hksjgjog.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qjdhwgpp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jzazzfww.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2hjdsdwey.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2cubdsiiu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cxjymyrf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gaychsmf.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tkecagne.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2qlkddvgt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vqlvsmhf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2glphobjf.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qqaxomth.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wrxkhxwi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dbxcvhpk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ksvmuseg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ikrqyqqq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2emtbuplp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2jjqyeyzc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kzotzfzl.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ydswymyd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2goqbegaq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kgrjnrkl.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ckcwkfle.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2olesxxja.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2supkkuuw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2oolyhwwc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2apndtunv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jqsfifnt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lykatkud.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2kmxbqesk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2sysuagnl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tybypzsp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2oefwrjgb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2exdfvqru.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2thqkhlow.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2asmydvab.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lovwceqr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qrxgkdcq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2sfkxzcxg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2drrgfhqj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ybbdhvox.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ybpzbvoc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2mqlsnyaj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nehdeamo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ybccxcle.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2fnlvbodw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ptzrweqt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jyauobxz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bsqseahw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ffumbrwf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2zdrfptkm.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ucxztzst.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2djweovzu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2yiyclrfe.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hidckljc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2uihfuwdf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfmbvwsb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fdjxjhwo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wktlvmdd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ypelonlr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppylrnbs.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ajlljzvo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2vzdgnyao.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2sljemdvc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwrhgyns.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tzjegedn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2xvbyhrpi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbprbucl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wmgtqtdw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zvkkdiib.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2cuonejed.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dqjlcyfn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nxuxacej.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dbifuojv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2frlmztxd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2huddzipi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pjxadtoz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qvuquyta.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nxqneurz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2tivtzqzz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2focxhxib.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2duiusxcb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zcuxqjgv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2owpnqrgn.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rrcmnjci.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lsbwswxr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2hwslpitj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2xhpjunmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsirbjwb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2sygavudw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krmcxvdv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rcmlepfm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gjghozdc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2dwhfaomc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kswefsqv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ioelhflv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2vmpnxnhp.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2prpylxdi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2elbkxnlc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2pmsiztwe.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ncmymnfh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ktougfqc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2bynllygr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hhwkzkcy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2cxujvygp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pxszgfys.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2kggpuipy.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2himtqcna.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2vlnpkucg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2oltodnwj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2pinkfohw.html


<!-- 参考信息 -->