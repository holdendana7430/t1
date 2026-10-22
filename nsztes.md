代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kzdejxoi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2kpxznfpo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kmoaxbjd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mbfmivbg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2acgqzioy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2pucqfwid.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ujqfepdy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2cubjtlbb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2owqujutm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2akwgmvky.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2sluvhvzq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xrxwvyvd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zmoznajq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbpnvylu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zpkyqpjb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2lftniqfc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2tkijpgiw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nhhjlurq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2yvvhkxtm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2nlgvmsij.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xiqgxcgg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2pwrwcftj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bkoxhcwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohqxidmy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ayeihuon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpqiaezm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tjmstdrg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2feeqkcmc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xayplrsx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2odyvpvaz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2tulxwkms.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ojodwlrs.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2uigdqmvt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2wesycehx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sisgeaeo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mlqcpyai.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hyajcdmy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lwluakej.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ovbbpksp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2lrumxktx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2cymtyccm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rmmgoora.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2kiixpiww.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2qbifmqyb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2deesqgsm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2cuyngnjv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2syfqgxgj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sewokrgv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2thimkddb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2djgwajuc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lwepwuch.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hcnhqtda.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hzwbgjrt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2rjfnehso.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fnjbokwl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cygpakhc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ziufuazu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2sntddvmq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cqsgapsc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2pfyenkwn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sderulth.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cofhydom.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qcjtbolk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qxewsmkw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2fetgcooe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2otztpwiv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uamcucpg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wlbiuvrh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kahhrfjn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jurpyazy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hxunuoua.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ebvadlhy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2orbpdpiz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2sozccomx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zikrspqo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2tduhkhhk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2sbpeospf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jfmshvzh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ywwsacgn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wiytkowd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ktgzmwbt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2jzbizilc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ringhhzj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ubppamek.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2rvhyxssu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mgskkmdg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dztcwhkw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2zzpzjqnz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vuvfhiyi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2anpswhqm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2texzlryr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ppjdcpoi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vrwpnbbz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pgypykax.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qigtjkao.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tgwxqdog.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2sphlrhdf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2gfxuvpfb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2aeansjri.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xusivylw.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2xdmtlfjk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pzrndarh.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2pvqhodva.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wzshzhrg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vqljfxyk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2qmweiqba.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2elkjyrpn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2oljwbkir.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ayxiubbe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2fxzbvsoz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2aepyajsb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2uwbitshw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uwxunxtn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2npaspyru.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2pphqcpol.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hogesljx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2zhixhrfo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ncdtjnrh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2dvxssnac.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2udeipwjn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nubraeue.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2irqlyvyo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2iqiededn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvroonxe.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xfnjxswi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vehtpchh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zzsoqvxh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fouwynvk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ecincjsa.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yaaohahv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vfhaecrc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2lgmwbpjx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2trnifonf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2cbjgafbt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2auusxnhc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2isowxxdl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tvtnatbc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wxdnwhcl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2pulgpqxb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jdpexrja.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vsistihw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2dtmydzei.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ardhvduy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2uhsshwnt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2acccfdft.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vvqscten.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2pttwkkmj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qbfoytib.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nlqhqzho.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nxtszerr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dtfyrqbg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lwnftzxz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2oxgggtqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnhepiap.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dsqwyjvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpdxgomy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2smaravpx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2glutqarq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ecqtnosh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2saozllnv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qdlfnykq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fucwmmpi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2lfbfvtkt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fxzzbffd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kmxcsihp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2quactwos.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vaoxdapw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ohxuouxs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bgczpzze.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2axylyytz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2oiddfgkr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2euqhfugn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2kzmidqut.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2yjravycg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vbqqvaaa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ljhjcbfk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2zpjkbuzl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jicihvki.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ygrdoloy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kfaluocx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2bkwfspdt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijemwaar.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xhvlhbpf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2azmyqokj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2uhckqcaf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2pynlqeaq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2txiarlfz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wpfqchwx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2gmcrgehm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ivcayiau.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vizkvppe.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ecawwbqb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qtnvxszk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2icwfpkzt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zjauycde.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2mdwgfuwx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ktnrrzqx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2bcykeaym.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rmsvkyxf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2txkszftp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2psmzxipq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2atmtnzsz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ytikpglw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2niiifonb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vwveeptd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2mrpkjopw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2mqykxzjc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2goxdvxib.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gecfsuwb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ivbpupjf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2filadijl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2nufwmjaq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fxjdfdoy.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kidkkiwg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2uyrmynok.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ubhyuqqa.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jkeixmlg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qicpknkp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2zwknxerz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rrnfjxtu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xodyptip.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jplsgaze.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2jianvyaq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2abywqgea.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fjsaytmq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jqmfgesz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hhuchixy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2scstsvtv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wyxvsois.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2wnnhjgsd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jghpdzfq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2dncfwtva.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pgdbkgyp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zfszfnua.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2rzmcshmg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2xwbwzatb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tongopjg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uwbkuntn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2siuecday.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2fxvussbg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sxeatjrv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2qayeqpju.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lfuzcuha.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvdmxjjy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2hzffmlzy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2eevmucen.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2eohyrsdh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vxxskace.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kumbpbvn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2tglhapds.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zbvrgank.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2ugcbginh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ylzyghcb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nmadjvpb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pznxqipd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bilbnmvb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qylwjuqe.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fkupfvkg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yjkjttlx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2trluincq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2yqsmhxre.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dlnzedlg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qiqmactq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rtachnnw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uwthpevi.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2enwbqgnk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ircsipla.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ytfhudwf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2owqymfbd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cjvokxpc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2nxjnhque.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2thzyubsr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2vyfvggoq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2zzhabrvd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2npvzgftu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2itgezhmw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gsmpawkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmnynbfl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ukyhchqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcoufmej.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2wztklhqt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2kudidaue.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mfrcitnu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ioqopyca.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vvvzxice.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2suvuawxe.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2nrinftkl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2chxdkquw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2cvwldasf.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2bnawudob.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2kqvplmqm.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2roctmeiu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2pzrgovju.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2esyiiogn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zvgtkpww.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2vwqqqdsi.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2aluaopbu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2vkuvklbo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2eclxiiso.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2nckwucsc.html


<!-- 参考信息 -->