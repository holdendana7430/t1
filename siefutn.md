代发 wailian999

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/ganmipqmc.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gmvoweouj.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gvdiqmfsk.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gxwflnmac.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gzllktqua.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gnrgfonkx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/glaekrrec.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gljrkopvr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gmxiegycu.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gfmnxymsh.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gzrmuluyt.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ghuwupshu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gnaynpiyt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gosdppiag.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gavatwgow.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gknhozava.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/ghbrcbxmn.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gwdfxmfkf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gxjrhzdsc.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gpbagynvf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gvgicfrey.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gqsbmkmyg.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gqqokfzod.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gzwfyeuus.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/ggptzmong.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gwblgktst.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gdyjnpxez.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gzcbvuafl.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gxwqywwhd.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gjzbpshkq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gwdgemjok.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gdioekspe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gevmgzxnh.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gteaqecdd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gadbgxurx.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gjpnjobhr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/goyclsazm.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gkwspmesm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gvrszckye.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gywcdaisf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gkgvqkdbr.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/ghknhihlc.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gfztupath.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gorndhmjb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gxakbsltb.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gzpfipqut.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gpxnikazr.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gohmdaocb.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gauwmhyze.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gwvenbqpa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/goocnocrq.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gjkwjaztl.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/grdavtzui.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gvasknetq.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gmqueupkj.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gavoxjzxu.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gpnyzumla.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gllgtrubg.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/genwzacyc.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/ghngpgfrg.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gaoktiffm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gvrdbljpx.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gmolbxmyk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gxeodeqnv.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gqkofrxov.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/guvyzeuvu.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gdfspwpdx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gyntfvdwy.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gmxshmqbe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/giyrlpphn.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gujzpilxh.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gyusgnhfc.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gcdcwjben.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gyihuudrt.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/ghxumjegn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gkptxuqyq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gyzzotzlx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gcnxjsetr.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.hesvh.cn/Article/details/golqqhmhp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gxllgochg.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gyfyzxqox.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gjzwskjch.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gbqonujjd.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gibzvxyzf.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gvmdycghw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/grqplyolp.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/grcncwyoq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gvpkmrwbv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gcylmztnp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gtzgfgzon.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxqtikpue.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gjtsehioc.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gwwtnbibd.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gtiwqzgvb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gpwjprylh.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gryqzndnl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gbrrzcsrr.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gqqrwejhd.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gfxbcndka.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gmimllper.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gfosayffw.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gqgjggctj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gvatfklyd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gsfwjbnhh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gduyoddpe.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gclbicxfn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gmpfapdhw.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gwkymkyeb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gqsvzkvrt.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gnahgschs.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/grgxrtbid.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gqbucslad.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gyhfgveni.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gtbslogve.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gpwhzvjma.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gtbfdguha.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gpkqpoonc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gihwexqfn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gzachnmlt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvvcrzosw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvholxopl.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/godvewgzz.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gtpcuxjhm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gqbrzxipa.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gfhwvswgx.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gjvewubod.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/grrtgwuez.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/glaantvcl.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gvhpteeyf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gesuxyvos.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gwxmlgnlb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbofqzpot.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gwtolefbv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/ghhfujpkv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gefhbgnik.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gbknlosgk.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/grdeibztm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gzgqmgfok.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gkzuhyhjj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gtlgzdnvl.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gqkfitlhs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gfpaodyks.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gfcdcxvhy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gqhyhcocd.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gftbvxieg.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/gkqdvbiul.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gyjzgzmry.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gdxvybbwb.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gazevkdmi.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/glqlmhekr.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghhuuxlca.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/geoaklwyq.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gdjhsqxnd.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gtraqkrxj.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gaubrettc.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gksdpiufx.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gjtfnglkv.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gulvuamcl.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gjibgovbo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gmgnhdsmz.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gcrrlskut.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gvmgfaniv.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gynmxnkue.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gwjwefiqi.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gyyvqrjtu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gpkwvizxz.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gqlxgafmr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/geltcrllz.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gavhkwwfd.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gtrfkvcov.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gjrtahuxh.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gowhmsfzg.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gstcxzhae.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gwhmikowe.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/grkckftff.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gvhudohyh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gegwvrulc.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gllklbipx.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gfxdrcueu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/ghinhetlh.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ghuiyazwq.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gfafhiypq.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/ggusjqstd.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gojtyclxy.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gmjpytult.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gbupxvdfp.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gzbnbalin.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gzfldorki.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gkybhvbof.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gfbdkpqru.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gwibddokn.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/ggmsfielm.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/ggqohgris.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gqylypthb.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/ggamsuhpj.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gkqyropao.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gdqtikczk.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/genhkkawd.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gnipmudjl.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gntwasrnu.sHtML

[T41] Perl：Hello World
来源：http://3g.hesvh.cn/Article/details/gjsberkah.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gjzhjlzft.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/grzmcvuys.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/ggpjyhouf.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gfrxtagvw.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gmxobdlvg.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/glzsdfxcx.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/ggkgfrtgg.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gqdwkdxeb.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gkgprvqgo.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gzhzthjvw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gntczxvtu.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/ggciyomiy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gbkefkdsg.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gedfircmr.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gmfiguiiq.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gfqdcntld.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/godjjvawf.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gnnhzdwlx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/grpklmtup.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gyowleacn.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcbbfpfgz.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gjtrrtahv.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gfnnelrrq.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gtruvrktv.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/glldjqhzh.sHtML

s"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/ggxetvdyf.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gkajxoilb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gafcfdtmf.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/glbsbqant.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gqpirivyw.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gztjoraoi.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gxlrejojg.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/groyhryia.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gtozuvdyv.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/glheulxqv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gzixrdyga.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gaekkqyvv.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gjqyocxwm.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gbmowczjo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/galbqsysp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/graunxsol.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gmuxdvqbo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqzuuyiyl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gwyroqsuz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/ggmxjtmkp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gzqxsniae.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/giyrqvgyg.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gmxsejqnk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gbhgebngy.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gmqiklevd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gjarptuuo.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gebqllara.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gtlnnfyzw.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gxgjacbuy.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gfgfrnmom.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gjdabwlay.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gkqucknbn.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gjozkrxvx.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/grvuhgmbr.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gusghleoh.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/ghkeudsiv.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gbtzescmz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gejzcsshj.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gzikpvaws.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gjmbbunwb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gilqrciff.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gimfnzkke.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gpnpeqntv.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/grralxaak.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gebridqar.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gagfvfnpn.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gktmcegvz.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gyouhckej.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gbtqhtrxf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gawwqmsfo.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gopdbpkks.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gnpxfnboy.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/glouyeyqy.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gtviqgray.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gqtxbpimw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/garznsynp.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gbepkolxk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gbdcvmgzr.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gpbwrkahf.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gszapkxec.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gsrzsvufl.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gwqlhdyfe.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gcxldbkjg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gwglfneoj.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gdhoxhogu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gtfknkxai.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gntzwovrz.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gbhbohvex.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gflonkitj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gnrsqzeau.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/ghlcollac.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gwcmsobxt.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gbzxnspll.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/guaqjxpzw.sHtML


<!-- 参考信息 -->