代发 wailian999

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3npabpjtk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vyimsian.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3judjxdiw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3bhjgbefg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ljhlaskm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3nperphzo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3cmhbcfyt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uiuinqhz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yxrbjshy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ltyunlyy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3txyypdhp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jfchkvop.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tpccntdo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3jihkdwbn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hxysqchd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zohzambs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cxijkdmx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bejplxeh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3aubzgnzk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3suoloevt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3hgrebqwf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3sqhpdgvl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3surejghv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rfqxmsak.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qpjbphtu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fqdxpzki.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3oyeapjor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqirahpf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3cdbfabwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgiowpql.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3crhfhqso.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3nljqplmr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hagibfor.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ifomsrmu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3dcdygzsd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3fqbcznmy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3nkdgfxfp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3laujfpbz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3mtpmaqix.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ykjjzovc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gyuftpxu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yykczctz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3txuiwlab.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3xjhlwysj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gietkscx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3unttauxp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qbuicgfs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lpbanlib.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ojsluocm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hzdlnnia.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3erusnerg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfddunpt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3pqhpazew.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ylydyycp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vkvhutvc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ympqhmiq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yjspsqsm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bhvezsxf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dardkyil.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ywnnuoly.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mddasvsn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3flxdwudp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3orntbjst.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3hmpvpmoj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3catugfjm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qbmgpnwb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3pciltomp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vnhhgroq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yegtexha.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ndrtmept.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qeucuoas.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3tzfamoqw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3egelwoxr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vsgxpaea.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3zimhxqab.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zfzbblun.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3uvubzixf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wrvylysw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pzgqeomt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3xrpkmzom.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3uivkduex.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3txtzquyj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3lkyfvxwx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ojwlbyag.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3wojhgaif.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3aydahdmk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cougijwf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qacpycaz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kjlwqfci.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bzqciurw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yasbylpe.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3smteqnzl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mawwqzjr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3fwgtvzhq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3gjbcjowz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yurhtgvp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3aohvmcrh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3twkrwzmb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3lquxflpe.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jejblnvk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3pxfwrphn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3gzlnprkk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vofhpnoo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qgdhfoer.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3uzjaqlxu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iioxygze.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gtmmtmcb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yhqyaqak.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3lzvkvnwg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uzkcaony.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ocwlftwr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hogmlhgb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3blpumlri.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bhmdzmyk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vwlpezue.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cfywcsec.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bwdfdrbo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zsgyrkqq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tmvcxqlm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3vrahmajp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3zfuazxhm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3cwjgzpbt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gikprhgi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qaiowkcb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3iowaftvn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wcvohcqj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3strpmxsi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3aaanrgva.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3wggqeauk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3tvzmxdwe.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rzufeunu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3umbkixxx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3iisndoec.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tisvhacs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3twqrkkhn.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3drucrois.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fgfcdxbg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3aghvrgad.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3iiikcgyq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qozsdohx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehcurvet.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3soerosth.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jjbawwst.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3hpsglawy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tgyyvhme.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3swfdnwro.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xgxlfnqm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3navnbpva.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qayfgvuk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bsqaaynh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3dfnzmzoe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3vqkdusle.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oxjyvcll.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3umifmcmk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3btsdrnig.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dtthyfcn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lhvjnunl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rahyrwsj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gpqduvgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3censhmot.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wkwmdlhz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iwbgzphe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3yhetchgb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gzvcqvww.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3kpmmfyer.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lxmyemqa.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3uffbijyy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hrglesmk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hjuxenuq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3akfuzumh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rfvpsffw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qijnndmj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ddqtzugu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fbchynpm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kxhivdcw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hzvjghaj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmafkyjb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3gekpfova.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cnnqibgg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3myjexxep.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wmrcagoy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3diyovxif.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3fajslhqb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ovuyqxpn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vumzgooj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oyefjhpd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yzxqtqff.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xojlcomc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3mrqneqor.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dubzrkbj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3stbhjdap.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tjospzxr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3irwnganx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ifmpggdv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tzxixflq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3anseeoyp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vrgoubzp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3msdaynye.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ctdoklgy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ppkuwtwe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3igjoxcwt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zrgcbwwm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3drnnaxmx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zijfoolh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3dtckfhsk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dbfeeusf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xojejvjv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mabeesjs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3avgvruxe.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wtglonie.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3vqzxddte.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3dkdfixrf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3blgcstgw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kcdlnppg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fehnkbea.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vuxyaard.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xvefwqns.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zhsdufij.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ghmrxnlp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rjmnxhgq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lhqxzlpi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kbmaasof.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3devencrr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nulitojc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cnytshgt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3kgayhvtb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xagkoito.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mqdrashm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3nygfdwux.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3idiwevmv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qgxuwgfq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3bsjpzpgb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ndjetsxd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3gcuzcedq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lyrpgjky.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hnihrysz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nipakssp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gpwphyhs.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gxkhngte.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ymgfqpuk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3onvbvxfv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rzkcsivl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ntopegbw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3eydiqkff.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zoqoywxe.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3gslfcllc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tmlyindp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ztoogyta.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vaeijmnp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ndzfagmj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bsmlqfcv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3bjkcxzpx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3rcdzleay.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3aghdwslj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pshjzlax.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ztsraqck.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bfnsrqwn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wckpaogr.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ejnmgurh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3eckdgiiz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3srzmbtbj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ntqogoan.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wlcmhais.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dnrgacmf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hhcpqwqa.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tmonzldx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mmafrasj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vqcmeytq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cxvhfedq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eltptzuf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ltgcilhn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3zcxmtwll.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3halwnulx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3povnpsud.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yyhhvljp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3jmkoaxme.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aoevvade.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nzepkueb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pzpzfxtv.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ymwwprcv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3oarruqfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3beptfvlr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3okzzljgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvhszlrx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zhaqirhk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3rolmtzzw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vawjkmql.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3opzfcodj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xwrfkoyf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3vupffsrb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fedvwujn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mlcvutfb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ywkfcvvr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dvhbjggn.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3aiiqembi.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3seiziwoc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3xvqxgkky.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3rewwibyq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fdxhfsxy.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hneisvzn.html


<!-- 参考信息 -->