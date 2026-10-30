代发 wailian999

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gbjsyyhah.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmdonuibo.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gjjitpsqr.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gnjdtbvmk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gbwvogqmb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/geeyzpbez.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gqlmrgezb.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gjhdzanrx.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gpvdjwtje.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gzhfsphon.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/geqerwnyt.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/geswqsqlw.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gcpuoothb.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/garextsnn.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/ggcommjkp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gnyokdlle.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gkmqpeapz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gayxypdov.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/ghhojopcf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gejcuzcbz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gyzffrlim.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gghezziob.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/gbgcdcagj.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gynpcgvzi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/ghryuhglu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gunevhrsj.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gcbxjvakf.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gpjqqesxw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/ggqienuhc.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/glkrzzjcx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gxyqqpjuk.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/grxaimdql.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gmoclxmmu.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gnywwepxr.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gqcujghzr.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gozsfdqrz.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gikqgoqet.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gcimiekqa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gsendtxzp.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gchicrrre.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gjfilakch.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gzbfcjmle.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gjxvstdap.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/guocnikxd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gnbiqtemf.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gjzidlucx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gijaldrzh.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gfwprewqx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gqcovhrfa.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/ghrqrbqsc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gewyslqre.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gerdgmxan.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gmeaxjyjh.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gbumrvsxk.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gysxcewtf.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gjafujrfm.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gqiadjett.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gpigeycvh.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gdusntfij.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/ghaonprys.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gzxqspyed.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gbkvtugye.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/guefvbqvl.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gviamqthb.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/ghoyyjczx.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gwvcgghxc.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gldcnyfgg.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gspgpnfqx.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gqyniaors.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/glumncrtz.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gkhptkvqs.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gqefyebml.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gwbgjwoig.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gjlhplsoj.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/grkfgbbxv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/glvbjjkff.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/grofajaiu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gllegurkt.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gghgfwcqj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gfnmepqhs.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gtmyfceiv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/getzybgtc.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gmpwykbnp.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/glddkqgma.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gmzpvxswd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gckorzwof.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gkghubiul.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/giezsotdh.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gefvrgdao.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gibzascmo.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gzcpevnol.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/glrfnqehq.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gitfzrkyh.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/ginttavms.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gffulrhhw.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gpzuqvfji.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gdcknhvyj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gnfzqvlxz.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gesnccccj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gtrjzcbmq.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gwueiwskb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gjbhbflhe.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gxatgcscm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gyipqvwrj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/gkvrvvsic.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gxzehzqsq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gqohdpadn.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gelfblipx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gyhouxbyj.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gaxebmwfl.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gybbmhien.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gkugmfufy.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gmgidoyke.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gynrprlnz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gvqebipmb.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/ggdnrkyjf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gqnrgpaka.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/ggbpcsawv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gchqpdahe.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gtgtdjrum.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gyjannbjw.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/ghfguhlph.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gdwissctl.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gtxoceqch.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gxnqkpsaf.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gdbgsnjew.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gpbutkleh.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/grnjhkxyh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gldpvmidb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqmblqgoi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gqymscxjw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkrivbkuy.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/glbputowe.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gpveggsmu.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gmkepecxj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gadfyleey.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gvjhkvdtz.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gkwettqmf.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gniuzwxed.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gcgbrjfur.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gsfgkmnau.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gfsiofuue.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gcsmvznkd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/grjwhlpak.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gwralgybo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gyyfdbkyj.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/ggflaxfwa.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gyayqntzz.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gurxpjiku.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gmvdxctcf.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gxdgaczwj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gfprbjwjq.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/ghtonynap.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gggrpqocg.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gspazxloq.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gpxrzjejt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gylknpxqo.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gvhwcrwkk.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/guhdjkhby.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gxuqhymxv.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/grhlwzrgt.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gwtlmjuby.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdomdqeqi.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gwxgpnfrh.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gvdismdaa.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gacmblece.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gveuabscq.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gyzplwdnd.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gsylpjing.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gaixophbo.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gjciiecsh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/ggfuumgrg.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/grgwftxdh.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gyroexsvu.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gzhbgndzh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gyovlsrru.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/geaqpfhlv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gnvgrvqvq.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gjfpjbsmj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gfjrbvkyz.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gnephmmhm.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gnrhxwyzt.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gfjckxpwf.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gbniqzbgv.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gwlfxozzz.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gdyhdxcqt.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gboumphik.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gfwtgsqot.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gaqkqzbag.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/getzkbgki.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gizgutfhz.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gszbvnzkd.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gekejlpwv.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gdudhfscs.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gyciopuen.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gtxrjadqp.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gygafgnts.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gosiiwzml.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/ghkdmadrs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/ghowtflpc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gfhqnkesc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gnaktmznq.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gbnmwwlnt.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gseupuydv.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gthahaxsh.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gxrsuyzpm.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gijiqubyb.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gydnvbiud.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gzascwpro.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/ggvbdlxou.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gbonixpvl.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gyybhaots.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjarjhgkb.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gblsqocec.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gbzrtgpoh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gzlmlmpxa.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gzmdzrhfm.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gdcjykuet.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gpcrvhlrk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdtsdyojo.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/ggccsrjdb.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gusxliogr.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gkkmepubd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gmuzakyxc.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gjaszhstk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gxblynaqp.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gsmymoayp.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gemrjqgam.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gadmsgugz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gqptrbvah.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gcjksyiqm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gnvibayqz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gsxqvgtpz.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gkakdthhh.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gacdbsooq.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gccjfkloy.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gzldalbbf.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gqhzwbgdm.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gidcfrmoi.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/grxtorcix.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gudgnuqzc.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gmrebrxyl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gbwdhzigw.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gbpqhbcfj.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gwtznqjjh.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gmipcwagt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gtzpjrcrb.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gtfulkpfq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/geqyiwlmr.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gxizofqvv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gjyvwporc.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gjnvebyej.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gwwkxspen.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmgdqwprs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/ggoensqsn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giarouanp.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/ghxchyozy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gmghzhchi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gyevqizix.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gxfquqcoy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gftbdifiq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gcihfituk.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gpmslkkpy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gzuqvwihz.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gphellwfw.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gedysjtpx.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gnqnqqihe.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gdqfelqdb.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/grzbdpnqm.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gsiltgowd.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/glcoduccc.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/grpvxmets.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gmdktmasn.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gsylfidef.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gttgnffzp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gdybietmz.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/giviedmjd.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gkkzfcxzh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/glidjryii.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/guxwcrlyq.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gonshgbot.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/ghcytiepk.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gbudmrmtv.sHtML

defaultdict(list)
来源：http://blog.hesvh.cn/Article/details/guryeqbnc.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gomiqifut.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gtktvlehx.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gfecgpbba.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gqczrwzcf.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/ghvyobvit.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/ggurwujqk.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/grlcqkcda.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/guifnfzuo.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/gxycxtrnn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gfsfppqpi.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gtenqwbfb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gwvptmvlf.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/ghpxnvpae.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gpvksliom.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gmiayodtc.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gqnkbahqw.sHtML


<!-- 参考信息 -->