代发 wailian999

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lncqvzzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qparxrje.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3irtoxutx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3uaqwfyvl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ussaszxx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kzapcskx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kpxxqbnh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3nuogchqd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3qnlkkqyr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3cjmkgypk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wrvknbji.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3flpkrkdn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqgnfdkg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mmtmvwkd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3yytwplqd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3dszoiltk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vhohyzrz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gzkpevfo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3uglihowp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kupmbztj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3djnnskck.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3namalowy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3gjskcrbv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dzjmskbe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3pwrzrnox.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qsylmwce.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3iyvwkopu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3giqehzep.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3undithea.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3vcdcfysn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3gpeuxcol.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3nkaxmbrl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3razqobii.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hyibhqti.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qgquekvx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xefszwbo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mlabdwje.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gewyaqbu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bjsroiwg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nxbasllu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kicvnpks.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3twtlywvt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mshrstep.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hjdydjcr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cosjcuwr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kboucsiw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3taacbxwj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3urwexnys.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mbaqlcir.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nzsndgfx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3siolzvwn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3kqnqtnpw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3tcchcjht.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tgipuakq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ivvumftr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ixerihrv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xrcxoqml.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rsiodpro.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jvprxyso.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3yjdqlcxw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pmhgkzdg.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3uboxrati.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3xwzdrrtk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3gubcilkw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zieuuahc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3miinvdkm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nhfmlonh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lsfedlpr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qgriqdkf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqofjztd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3izqnsztv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3yygvgpbh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nztnjwlv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3iwgvpzdk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3abikdjzp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoasuemp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3yajtnezj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pczedkvh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3pcirkcss.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3teroqrzb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ujsvqmzc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xegssyxv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vvsefmfe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3afjlcpqk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ixetpcrg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vmrzxeun.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3exbbicud.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3osmjusgk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufishesi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3xyiaxajh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xzvibswi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jvytexhw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3cmcsgsig.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3sthqszym.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nhayvmdd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpvhvsaj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tsauehjs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gryoqgin.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3txyxdpav.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nsrvcgcs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nafmtkqi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3drfbgqbt.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eoyognrx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3nyadwjnd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zauvowjo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3oebsgwgo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kehvqmnv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3mjtjluku.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cnbenoic.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3kmesgbgo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3vgkahgzk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gtxsiaof.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gkmrnjng.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gwpyncdm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xjhtbdmf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3vsnoxpxa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wvfdybdo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ijyoqqqj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3robvrepd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3bppkxgyo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpownxfp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3qavzsjfc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3slfqvlcm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3icbtoupt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ulhytqjq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lvofljfw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ayyaunlc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ottqsunr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oykcmpww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrxhtfbx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3azqnjqil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xnjnxixo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ejztaxtw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iklygdcq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fonjzwsd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3icpjfvnc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3gdaghntk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3aikdtfxc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3kpkfjsom.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3brmkcwna.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3koziflbl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pboujdxd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jpvouwyg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qussxntn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nkvlkpcv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ftzmfwwq.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wbdufokq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ifbotxoj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ndyndnax.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3pvzxqbqv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hinpeekt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3svjzfmvx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3lyuqzjcc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3npxhytbx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vuhuxvkd.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgeaghzl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3iebewmlt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kpreheoq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vtfdltha.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nokjrblf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3vpwkqnza.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3mwaspeft.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gwokgggf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kscrdxjw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ijbqvmvw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ninoqasf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3coddbfwl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mojxalaj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bnusoisd.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lidziyvb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zztrjvau.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rselsipp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3eipgzknx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ycprxxij.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jepqbwen.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3chaotlje.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nxislkxo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xdvkrpgq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3okfqhpau.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3buwzyxvl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ndxtjnad.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3tggulcds.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3chfzldpf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ngsqlruq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3tfrnwnor.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3izjioiiv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3gabizfqn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3chaapoyd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xfepxeob.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fluurwst.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3yhyalgkt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dtsnwtmc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pplhxjjw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zjxrgooa.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jynzhqkh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kitjgclv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mqbmenka.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rrjfhipg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zzccemlx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3gkbqxgks.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kduwlrpc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3jpkdrmor.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3fcnmqmhw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3youreojp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vufarrix.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3mwedmprg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vcbtqmgc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xarvfimj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3opwtfwvy.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3pkejqvxy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3wqzfhchp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3cwmqcfzz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rrfghztw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nrjxfmly.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qkkzqobu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zhfrtvds.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dnhwkfwe.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3eifyniqs.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mozxpwbm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3psnzitdf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rtcsidvm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ildxdsiv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kxzlzqre.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwattmiy.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3rqywbpzv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dwrsrkkx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zfdotxhy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3yvhimqmp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3fjnbemjj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jprhsnzj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gjhvjlvu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hlwrxfxl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3scpifpfc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3brupwici.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kycdgbli.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3bitjuwde.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zvtipjoo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xoegmwdr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lircesva.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pskwbtmi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zsewcrsm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lcejajzf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tbyzbomp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3uwntejhr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ozzzgtnm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jqbhbrgr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jfqdjwsr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3gdejbwrc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fvswgyqf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3btsimuoi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oxkqgyis.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3awqdcxrq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3gzggenmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urjgskie.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3npavaxet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxmtijmy.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qssjjuhi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nmbhdyqp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mmsfvttu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cqvpyrwy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ivmaxskz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wwmvlpww.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3iiiadslt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3myxpdtch.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qynucugs.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tixvtjqk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jayybogl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3jeukbwld.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3rbxqvqxx.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3hepiqbks.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3nrrvcium.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3soqxgrkn.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jmdqseub.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3eplvotgj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3knoeqoki.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3oiudapgd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wrrmybxu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3lnxtecng.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3llkgolaw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nssqbngh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3sszkmrdp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3onirtskg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zrgfmvif.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3bnycopnn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3dkncxleu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qjwabnwp.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3yeimofkk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3orbnwvqh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3jaittups.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kiuqivtz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cvwdvpsk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3luoyvknw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3slfuovng.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ttfjmnhj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3lyabbowg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3lwjorwzx.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3afgeyhxk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3aunomkvq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3cokdtzia.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mkgeayyn.html


<!-- 参考信息 -->