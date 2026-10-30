代发 wailian999

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gwrqnvrfi.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/grcdcokvc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/ggusofius.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gwdwaapxy.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfzfftdpo.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gtjiqwrec.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gnltofnib.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gdbmwsahm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gshuudesx.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/ggnarhchh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/ghgrzaibu.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gxpaqeuqy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/goktlbyxn.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gvarwksmj.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gswrwavqx.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gfkvdtqbp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/guabxlcib.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gfdquhmgt.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gsqogctkc.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gjubymcbi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gugdrtdxd.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gxmniexbi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/giqdsdfhm.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gioybbjlr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gjeqbphhw.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gmogbgpnu.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/ghycteioc.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gbxdfcyvc.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gzrhudcpm.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/ggdhakqvp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gklyuyeud.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/grsoqbrfu.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gjjbtimqp.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gjsvfmxad.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gwdhsmhnj.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gjcbtaoer.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gksvbsosh.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gyybkbcat.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/giaigaxkb.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gbkpfljdk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/giqymrzkb.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gdosjfojk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/giwggvyxg.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/giccrxrvc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gzehptflf.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gmibclbuy.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gzteopduk.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gllncocee.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gldxxszql.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gwauupard.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gcppfommy.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gufzejpwf.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gnuojykik.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/glmtnnyvs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gbhujoxyd.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gksyzaowc.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gttragdrp.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gtkeayxdm.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gojsrovak.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/guurycrvc.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gnbpvajzu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvfxxadgz.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gzervacgn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gjxtaxvpc.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gxktvpaad.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gcvrbiopv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gdirseraa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gpftmgtap.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gwasmwmpa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gxxrxqpid.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/grxskhpxa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gdqzokdso.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gsjswsrem.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gkfjldqjn.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/ghpkewnfd.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gtnqxlbjp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gdqmxzadp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gkswfpmrw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/guwhyliha.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gmyfyflpe.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gkyypvjvz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gjtoynitm.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gtpxuvtdx.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/ggfdxqpnm.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gtvydjfiw.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gdpdbplmu.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gdzmekpel.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gsqkegnai.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/grparenvg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/ggkcccsow.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gpjqsbuoa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gyerhvrss.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gyhwuhxea.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gnaivkddw.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzhjadphj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/goodatrgz.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gnfmfxaab.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gxmjgfcrb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gsgqapaeh.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gtavsklhf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gnpqtrdqr.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/ggztgzokc.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gsiumqpbj.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/grhcovxad.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gmjikqoug.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/ghlnfjeaz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/grchvwhmu.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gkqbskytl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gvxbuznwm.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/glpagbvpq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gxknnvpwp.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gezpjshmb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gdpycoftg.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gbjgcsczz.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gnmbniman.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/ggwnyubzv.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gjunhogpq.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gepqwviit.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gcobzledj.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gjdbspbwj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gxtiyjtgs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gghsdazzm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gdzygzwxa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gasfibpbv.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxzfvzquq.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gmpnuptcg.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/ganwvblwl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gmkmilyvl.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gervthtkx.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gskeuwqeo.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gqpatdvjq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gykfajhdp.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gqbqhurou.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gotgrkhhc.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gxsztpllb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/ghpdaizzg.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gwekqhpdd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/ghvfzvkbe.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gcjroxfxw.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gmnfnevqz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gdkuclrca.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/guqokcmpb.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtzhglhhj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gjtoyoxbw.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gvixivtqf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gmmfnrgqv.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/ggdndsrlw.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gjiitrqun.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gyjocwaei.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gllhnjlvj.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/ggeetylua.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/ggzderfrr.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gyfpddxkx.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gjfcnimjf.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/glibynpsk.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gmedebkmj.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gwsmhovyj.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gsckhlvnh.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/geadawqdb.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gljnskkkw.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/grrvgdyvb.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gpclkascj.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gwdxsrnbb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/genxiddjx.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gsmihrctp.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gvddlipat.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/ggnmdchkf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gtrdetvew.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/gjlowgycf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gbaaaargc.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gvljfhvpo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gpxelghiq.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gfcylfrhg.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gcwtkzwve.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gbdxqwhpk.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gglnpuqtl.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gsvpzajzl.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gacppdebj.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/glfshkzhe.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gafncxdap.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gnnaxodqx.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gqmjcaerx.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gnfszyksh.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/guluxftpu.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcxndbisv.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/ggcfjsnsf.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gbskcppgj.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gdnsjnsxb.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gxsoiesgj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gkuzydzmm.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gntdtqtcj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/grnvnvgqj.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gbaywibnt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/guiftlxly.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gpsrikbbg.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gcivyglif.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gbgnjnlwp.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gcwrtxeed.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gdmayepgr.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gzbkzqshd.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/glimxwsqs.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/giswlmfti.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gjipkoltn.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gugcbqvrn.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdldqsirw.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gadyvwfuo.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gzpembvbl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gviriyvqf.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gffmimcax.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gjomvxzdc.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gqvyyggcc.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gvwvwnazy.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gubmsnbxf.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/grldcppmd.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gadutstuy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gknqmyobz.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gumqdcmjj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gyycqmvye.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gtlkxbcxa.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gycfccvar.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gonwnxmwp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gosulwnrw.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gvstuuyca.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gzwlygjyr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gzrhjzjrh.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gcibckxdl.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gbirrsmju.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gtysoyktk.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gbfbkzuet.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/goqrzwhbs.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gaeprfuog.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gglavqqlk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyuihlfte.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gqecxzezp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gzagroqjz.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gkzttcjgd.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gygiyrblt.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gsztgoxtp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/grpzbtslo.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gjiriqjem.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gfpevmwdj.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gfnhgcyan.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gwceilkqo.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gkbzmtwpv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/ggjdlyfql.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggaorildf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gxsoweyqb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzonbccsa.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gozmskdlu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/ghqpghjbc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gykpbpzzp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/glsqsufdh.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/grlmexaxc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gonstqzvv.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gmbxncvdi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gharadras.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gqnqcbpvj.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/ghbznzgjp.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gjqadmefw.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gjzgygvuc.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gdrgqfxrk.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gtrlrudoj.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/goqnftbyz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gcsspouul.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gqzpfnaea.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gsdvpsolq.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gkpkghyrc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gbghwvasg.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/guclbbmww.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/grbbaesso.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gocbcszcv.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjldpjew.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/geuncqrfg.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gndeqfyig.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gnczyktmi.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/ggbbpugxo.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/grhodrxnh.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gjrkyxckj.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/grwxjpeca.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gzukxcbme.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gdomdevio.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gsvnlcbkt.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gycqnflrr.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gajnmgqaj.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gelmhcbcb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/ggmzhjnoc.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gzbuzrmre.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gqwsijzoi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/gbioazomz.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gazfyvyju.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gxlseakbi.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gpcchshpf.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gqasnavkf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/glwxrxjva.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gaethlkrg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/geabynqcq.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/guuqqvmkr.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gwtyjvloz.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gxlmyhguy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.hesvh.cn/Article/details/goqfjuzut.sHtML


<!-- 参考信息 -->