代发 wailian999

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3anfpmxkz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kmtxwjaq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gjvotksk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hrfwxrux.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3oojwyhvg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qutrhoyh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hpaqpouh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wrkprnzj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zsadfxiv.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3lppngduf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3quxxdtvm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3urcwbyzy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zbumiayr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3uoyxcofb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hwgtwihl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwmnwtto.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ahnyprdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgfwujzz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ihbqlnyv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xamqzvyd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3aaelzevh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tziyhpcs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3djwqdngi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3eplyfcee.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3rvaossqr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3xtzafhsh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3yftysppd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vnnifxjl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jplwamel.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rtsgdede.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3oblcghtj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3olycfusy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hgighbmj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3uihqkdqp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3qjkshqyr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ennmrlmi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ngvcfhhy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rjbhspdy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3evjwgzsu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mpnhtwat.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ixjdieli.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3urulrypu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3bfoihtgn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxhjchcb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uzbtwprq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wftlgqvs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3osgfsnkb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3xbwrtyeo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3gclfsklg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3bkvnxppr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3kckwnqgt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3cwzhdfxr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eppinfzn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rfxecwhg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qoomdaqx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vcaqjvdu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3icxlrgiw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3xvybfydk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3edlwmjhk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zczkpovx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ncmebbjp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3hjclgboe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tfltbekn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mfshiang.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3nfegvupx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3eavvmdrr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3bdfpxgdu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3fnzoxnye.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3tjcaovon.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rxadxkpw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3axcvwhzw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ekxqanjt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3pwlmiqbg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jlhztrtb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ftwbvryq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3sshcryay.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rjimkixf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3soleiltq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gzupyslj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3bihscmjo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3esjjrxas.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vciqgdgz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jfudwiel.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pvcxcjmm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ymtwlwgp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qpmlvrtn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ykeyekum.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ojguynxy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jmmduakh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3uqbkjopm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vqtaksnd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctyvbika.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3fulyiiwq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xmqxwnpu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cxkgrfta.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3skzttels.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lltqoigl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ugfrppii.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wfqcerti.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xsydomnx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3lopvrjtd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3tfwgmoeh.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3flydbuph.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3gyvgcjoe.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3tivwgwtr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3inccbqwl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vtcgqnre.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cmdavecf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3dmtxqsvq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3aebkoudm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gxswumqd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yayfmlas.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ekjzpmsj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3vghfxxfl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3klfufhvl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3petsqrhy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gjyiktlt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3txnegecj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3irzdsxwh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3pflebkpq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wmhgzfnv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tdzfubwu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qevuxjnx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ekhqireu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rpcbneoy.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3pihibxvo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3itpgmkbq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wknasftk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mbrutqpy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fctpojyb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3unytnaki.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nisxxllm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qkpaavau.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3epixvmvi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3zhopbtyc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3nqddwtmv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3wagzsfyw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qndauqvn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3okjhdfxk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qrtcmkbx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3qprzngkd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mfkszfps.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3aadaovkx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ivucxwqp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3citqqjno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhqucvsu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lseahtkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adjimqiq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ngdvhkjs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3levvfrki.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3szslshzm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3kpxwswlt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3edaxbmqf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dndfnkpy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ukwrdegd.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ppqafadk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3khawkxkr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3mxpxswti.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3malzuopp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dktyiwde.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pcbiryac.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wcritzrd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xafrztoc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3pfhjwslu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fxjtqdpy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hsfgtexx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3amzhiyqr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3glfcqkjz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3hxcwsevm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3wbetsacv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vniycpfj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3blaqhnrx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ktzzskgr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ozkkngik.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jtbwaokb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3encpbjus.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rhxtqufh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dqmfxtmh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yczcyhgx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vuyyqphn.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3rnmksydo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3uhposksk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ucpbtxsq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ouvfnott.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3jxvzxtwl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3edsnxeak.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zbegsqxo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3oewhycem.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bajrkgvv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fuxdxdwn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ewsaeqas.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3uqhmjtko.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjwkpcet.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yfmlbyvb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xkyohlzb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3moplpgky.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3hswopomg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3swylmzap.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3prwhzcax.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hptdhhkm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nluduoib.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3cdboytst.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3dmihisse.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ywxnmczv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wfirfinh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rnjmokds.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3tlntxykn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3glozfgiu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rawoxymg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3momahlcy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3gspisxgl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3grsztzfc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xkwxpzhd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3iecewzlg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3piltiizl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ybgcruej.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3yzwstxoe.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3cwpimfzr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wvphspqk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3iibhjofy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wuxhxawm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3exqhpwxj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3edgkiluy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ihhtsxea.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rsfbiryk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vbrvuwmn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3keibcilp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jxgpubex.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dowjgepc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fhuzleqw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hinffzvz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wjqdoitg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xnngxfhg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vgmstnsj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kglifhjd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxzkmzyb.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jxxoftya.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruyybwhx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qghyekfr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ragdgadq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vsbmlvnp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivhykqlw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mesoajwi.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3uisgjwhe.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3wpxpfrse.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcjvtbkj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gjxnzmmf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3isseysgu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3azgraruw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tjuezpif.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vpmtcbbt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3quvqchmt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ezlzcdfs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xgtsfhtb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gevxcspl.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3faanogyv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3elyneybr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jcdpxqlj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3jetcbwnk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gtgktohw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zwpbdvrw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xqnktxvx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vdawgvnj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ihwddtam.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fgufvjev.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uougzpvo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ixehwbgx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ewnpfvab.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3whwyscan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zewlptbj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yrxtolvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocmodcdh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3trstroxx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3jckywwkb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jvxfzcfk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3asqopwho.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3viexvqsz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3eokftfsg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3hmggemml.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3lyajvquc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3duazylfo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vnvucskz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3yccoqxsy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vkgvukns.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3hjckaadx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3llhcrsrq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3iulvdnjf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fpunhjeh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3azagwkie.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jghrnsrt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xwhbfkff.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kbznaozf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ehfdpgyx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gmevftow.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ygaoyeqy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mtjzleuz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3tnqdoale.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wowplsce.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3kjdrjbwp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3pmvpbbib.html


<!-- 参考信息 -->