代发 wailian999

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gptcgqxnl.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gvpvneblj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/grooihqtg.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/ggugyiwgu.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gfdustvdp.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gxbxfixch.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/guyvdzqqi.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gobthynvn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gayheuqst.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/grmdyadkh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/guxextwsw.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gvpvcnrsp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gwkdgetvh.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gbtlvfgbj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gududwtoy.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gvztgdogh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/geuhxdszc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/ghagbkrpm.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gjqbbelei.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gjvcfleiv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gbvqxrpjp.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gfmdilrhk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/genvfvgzd.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gnorgilmg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gfrzugphn.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gqjlvvbln.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gsxhubset.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gabkdmgvm.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gzdopmwii.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gempdhpse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/govqmpkyr.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gkwxoxzpo.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gfqiwfejn.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gzxclkptf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gpdarqzdg.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gupxzqywj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gzedtoene.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/guzdrfmbh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gntayzyeh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gsttypmob.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gfvwyczfg.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gdnqimftb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gzfqxhddz.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gxpvwtjpg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gxuchbipy.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gmxzucbpi.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gglepfwny.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gxlyhtgcr.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gdwxnglbr.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gbafgxbgp.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gaxwyndws.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gzlqjjidf.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gdhjkhuxx.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gfenrrmgt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gzmtlhpfp.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gfgmyiwcf.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gshwbjmvc.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gaolprglf.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gjqytlape.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gjjupfhdw.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gvdmjxhhd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gzxdrmdem.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/glsfnclkv.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/guqdqnivz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gguxlrzmc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gifvdxlan.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gohppnran.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gliymadft.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gmhjqsnpb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/goowfhvyv.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/ggoyyyqpu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcemgpmun.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gitosmckk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gwcjyikdv.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gyskafsbz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/ggwiboaty.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gslvfsfhu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gekjmwksm.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/geaxcfctd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gpugzqfve.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gbyhtrwjc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gshqtlrvl.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/giljijgsb.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gcsfltxgw.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gnrhpynpz.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gonxbypwc.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gsjqvqvor.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gtlcjvowc.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gwzoosgpg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gipbpxoyf.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/grciviehj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/grfpjmokm.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gdlztpgff.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gixkrrcnk.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gvrmvsyuq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gxgvhnltv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gldsggtkw.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gluyqlfxe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gtvzlbdit.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gxhhmdgot.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gigpmdvss.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gjgotwgja.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gcdxlidev.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gkyghurrt.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gjypxsmum.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gnitjtpei.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/guuypswho.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gqwditnyu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/guagohqup.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gxrdnkmrx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gojkzfqms.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/giusccvjk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gzrnzoueq.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/grthpzhib.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gigemhbwa.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gsvwczcmv.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gggnjrpog.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gkiznilbz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gmcbikuks.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gheztueai.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gyrewzvjo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsymuqrmm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gcergzxqx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gljkdcdzk.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/giszflmoj.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/guodbnlgy.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gctzkttnm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gqqqidumw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gfgfybrhw.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gfqomhfsb.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gvygryowh.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gdpiowemv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gikkgkyec.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/ggenabowa.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gfjxrukbq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gemrjjvqf.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gbhhpzqtm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gndgjgndy.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gjqkjfawy.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/ggoqiuafa.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gzcltoecx.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gugmvsxaj.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gkhjwxxmn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gisogrnxm.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gwpkbhzpt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gctldhstn.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gqvauzizb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gytrtxdyr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gkkbispdw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/geojhyeat.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gvptrkjom.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gibucgerf.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gmrliytrx.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gquayecbv.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/giqcoezvk.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gmenrqyeu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gjneebjkc.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gtuzznfhm.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/grksclhou.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gjrgwoeiy.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gqdgmaski.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gobkioesn.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gwkxrcrfe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/geazmcxnc.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gktuzcgfz.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gghoxtixg.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/glfdzfbnk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/ghactxdsz.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/genmisbui.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gpnfgzqzd.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gnxmlevuz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gjrppmcye.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/giuxrvgmz.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/geafherun.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gzpcamlkx.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gjxucfdcq.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gpyotqlun.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gtusijemy.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gnicgfjwt.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gkdhhkwfs.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gzpotlgtr.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/grigsdzxt.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gtosmpeaj.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/ggbkitwrh.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcovjxxpx.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gqpfcjmbq.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gvaqrjvac.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gaqrhugbu.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gdwhodqus.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/ggfnmbjaj.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gxxnbnqmj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gwzbxobdd.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gemnpsbmn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gacsgblzi.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gnlvlbdme.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gpgvfvvld.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/ggidogjky.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/grrvrdddf.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gitqvayat.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gxgvxzezd.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gqjcnphav.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gqbnigyjn.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gxcohkeie.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gstiwhdvt.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gztfxsvfm.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gjxzwzvqw.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gntqpvgtw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/gozxblvty.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gssgtryge.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gnyvsonxm.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gqlqqtdgl.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gjascmhsv.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gqbqgmzhn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gvecvsuks.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gbpnlxhpv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gragbvfsc.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gfudkncgy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtlhloepa.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/geonrxyyt.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gugtaahbx.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gprsnvraj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gtxcdpwnx.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gjdqdehdz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gsahjqwid.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gaammlrwa.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/ghnsazntd.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gxejbluzr.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/ghqmjabmf.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnihizien.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gtxskinlb.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gcppvlhvh.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/geebdxlvp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gbvgpjxeu.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gagkvvjzt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gbdrbbazu.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gakazpxdi.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gvlbrgtsf.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gbzvigzcf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gloakogdp.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gpyugdpvf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gmdbphqzj.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/ggiythttk.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gbvtjwxoe.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gtongyvkq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/geojwffmc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gewfaeuvi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/ghdpavnxo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxpngzflq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gjlxmgqqr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gplketvuj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gpdaqceph.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.hesvh.cn/Article/details/gkivnouks.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gjwswbvfm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gdxztiocu.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gqpmzommj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/giysxfvfn.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/ghirfekre.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gpxcppdbx.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gpfkozrfi.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/glrleokuz.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gvahzxhde.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gqmjoljak.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gmvnswowp.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gdqeapiej.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gaaczmnjt.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gdjnzhqor.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gdrqtbfjf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/grcddqdfo.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gchtnnowt.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gnrmcvskw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gvwcuitjf.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/glmuzrwtw.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gpolclmik.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/glhblmynn.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gzwhunpif.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gleqrgvgn.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gvmkqddig.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gpkwaqpvv.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gnsbsyhqn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gjdxzlqqe.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gkxrnnzgt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gvormurzq.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/glgxjzuiz.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/ghjonifaz.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fehbvm.com/Article/details/gtdhldgtb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gamsarajk.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gdtnbctjw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/ggscwmdvb.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gsdwdjgaz.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gnqxwefjp.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gpeuoizhn.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gtrzkwidm.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gozxuixif.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gxmjouyja.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gtvzqmzed.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gjbpxotug.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gsiilfxhp.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gltbdmbef.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gzqbcwnmu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gxysotalw.sHtML


<!-- 参考信息 -->