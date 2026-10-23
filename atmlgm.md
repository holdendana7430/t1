代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3izckovle.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3itkihajf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3cbeefdwm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mxcoawvq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3eluezcsb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fgbhbohx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qesjdinb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hrdsmmdv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hgyjnzfx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3cfitznwp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3gmilbjav.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hedojteh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ufjjiweg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ldthxrxv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qkcfqice.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3faayqoaw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jbdhznui.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qlerkqcr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3btqqjykk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3cziuipri.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3iewtraoi.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mqbownol.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dcjyspeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llrhyhob.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jeeuekux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pidcrqje.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3evffznfd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xddhvamu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqwkqaxu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3buidarci.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rdasffql.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vdkimqum.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3arqzgzsx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3pqnhfccs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ukydbciw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rgobbwep.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dpoiayva.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rqyqqkks.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wfclgngc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3yxczetah.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3aznuvunf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3fehjxcdd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gzyrmoqe.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3zpdwxlke.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nndqqnuc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3oelntplt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hmonsigo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jfzgehtl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3roywqlty.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3mjwrkytd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nnwenhhp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wntyonjx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dxbzflpz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3aobldoqd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3uztaknpm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qyqejopl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3vdigjuln.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vuntecye.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hxgncdkr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3eofquawl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cpedohqx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hzcqxlcc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3smqygght.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3evakahds.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vjifhsas.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vmxfbzjt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fsutyxyd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jwchepya.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ljvvlhga.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3mgkplbxs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vixvpuse.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yacjgjas.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3putkipam.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3kahmbhxa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zvodmwia.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wskwlrlz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3nhhoxsxx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kjrlyfrx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3fmwzyzxl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3gytxdqma.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3kmojpcez.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3agvcsaaq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wfgrzimv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3zaqahtof.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3sdpvrigk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jnvyhhpm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ceclhpmj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ousqeqou.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rjiutwtz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hgkohhez.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ygzrajki.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wazvqypv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ijdfbnaf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3boazivpq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3sjbbsvej.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3boswqzhm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dhobevwk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3flvrmpnq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3uclvozdt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ocxjdsnl.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bswnwluu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dipmfosz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zakoyzhu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rktithod.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3liexsiak.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qzsnzkev.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3cypipgzz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tqpwjdmq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3xfblprrw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3sgfzkmea.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wigugqmh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3hmelhtck.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zsnfwbzm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3fhjnabsd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wpwnigph.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3aydlbylu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xxvxcqmy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nvknvpdv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3buteojpu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3fmlfghfc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ufhfykxe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3flhuchyh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3wbapzlls.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jttdotao.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3zpuxizdy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfvsexmk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cdsslcfn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bkvvyvhh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vagxwnec.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3aubqrzdw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3uqkviizz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3aecemdks.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nypcouyp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rihdzigl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gtsxqlns.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3owpaacnw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiqokwuy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3lljupvui.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3qdejafwk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3onwnwzoy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3kfvncvpa.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pxuhfran.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3rmonqdiz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wolbmpge.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3aennxwnp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3fnwkcyrw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ujbjgzsh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3tnwniync.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uqrsrxev.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3yjxqdjbw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tdydzxru.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3yepalihu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oydtcuii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rliidmqf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ygxnhrml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdcrztoh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gcdxivmd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zittgfpi.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ztafdxhl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3aahwnzap.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3quzssutj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3itlozjxo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3tlshfttu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qlwvfexe.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wyympalf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gungvkpu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dewdyvpp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3shyjjdmz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wnsybfwi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3frigonoc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3emojjryo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pwefendm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qabyhflp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3yldbmkjm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3txiggavp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3gazkmgip.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3oszicszp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3hyaewqzq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ubmwuvxj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3emqqngqi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xjlhqrmc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbsoithb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rgsspexm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uzsyvvtu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ttmvvadp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zdoqhbzn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ynxuokdg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zzsgiuhk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3etrbeuav.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ovevcsdh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lhbrqrlt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fbfnqhno.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jezdtkpg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fzstpgem.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3yyjbqihb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3emsrnfky.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ysrihdzs.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xdvdvufd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3lrowbenh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pczqkcdz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nqmbbwio.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ejbmmmsy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3crnodehm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3svkjzega.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3uyxcfsza.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ntwcltxm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xppdqevm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3onvyrapj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yktecrzs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xiihstnm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gykczelf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3okeomijx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xgfechzs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3warkhhow.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3yeisefhr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dejlyokl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3raugegkm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qxftduhh.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pagsdtym.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xznqwgib.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gngmgwod.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3hpyskire.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kmmcoouc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3xjiushyt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3xvilomjo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3phazwqwa.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3uxgyqgks.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3srwxtthw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nkplcsbq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3srsprufy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ztbggtio.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3istifmwg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yshtqgna.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3sfioilia.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3mwucoecc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3twxwqwba.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vsqppdqw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3weoiohic.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3aprknahh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3aviclmvf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uexnxvzs.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3qeeyczwk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rxlvqwne.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3yvranqmv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3uulipadc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuhmoepm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3irehhqeq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbcldfdm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3knvuipsj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtodtbta.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gxwtgctj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jymgtbzw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zkspcqfq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvrqcpds.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3aazuchhl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kabtizco.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3pnlrrbxi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zvpwpkfa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lwsumvrl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zcrlhbgs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3hnqmnkkr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nvatsfpb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jzzpkgom.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zngrcgdz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxznshpq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bowmttwa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3czdziugw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3pcrsuzmf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3elajjgic.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ramrwbuk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nkrjmzvb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3xrlshmnn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3esehffwc.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lqayhszi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wbdtrltl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3rvmnmsww.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cnfgvanc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unbfevci.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ncnmtwgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnjlnncd.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3akcrfgfg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3htghqwbz.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3kutrhucm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xhqdthjy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3owufykeb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3mhioczfo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3euckwtyo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3khklazps.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3lbnxhngw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3njaevbsi.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3huksrfnw.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yzrpwfdp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ebbgupue.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3adojpybr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3teyjuucm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ozbfwmpr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3febdasbn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3uhcogcud.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3euqyhiha.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3tusqjorg.html


<!-- 参考信息 -->