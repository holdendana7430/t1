代发 wailian999

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gkuqzuzjm.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gdxfygwmp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gszzclqkj.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gfhqhelou.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gluwnnjrx.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gwynqkqjm.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/glxnyakhl.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/ghzxzffja.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gkersiqda.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gfpzqohqz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gkhdkiinp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gvubnijzx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gwqdibtii.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gahrxcdea.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/grttlopeb.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gjlabpzga.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/ggcjcbjyd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/grzdskjnx.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/glxijoymo.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gtvzyianv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gtzcvqhda.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gqmrdnrzy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gvjkravgc.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gjraimxmw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/grtfmawbs.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gygjvnacc.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/growfmfrw.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/glcwwrony.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gnkelymyl.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gzonkdgcn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gsxhomeim.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gjxvcacnj.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gcimpibsc.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gzzsfbhkk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gxnbrklud.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gvzlxdjcy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gtsjgubnq.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gmbkkqryx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gztfeuxfw.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gsjswmkxc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gxlfoeugx.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gdyowlsbx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/grgxnkdkz.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gjbpzxpnv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/guzqhmnve.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gojrozmyv.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/ggplbphln.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gjzllsurx.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gxtjbnwsy.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gveqvtgzq.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gyuwhpspi.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gacgplrtl.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/grnlwtobv.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/grjuehiyc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gaoeczmmh.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gmqrrzysz.sHtML

#ifndef X_H
来源：http://m.share.fehbvm.com/Article/details/gbhfuattj.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/ghlxnfptq.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gjoxidpcd.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gapnajyit.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gpxbgwuka.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gfqluttvx.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gxuphvmds.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gmnopdxda.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gfqewrtgb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/ggyqdqblk.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gpiavcgmj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gutkihqaw.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gugztjwmo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gktzbkeht.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/givjtudrh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gaueyihlt.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gfgnvallg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghniyxreq.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/geetzplar.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gdxwefwvb.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gfswizrlt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gjfxtrnnk.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/ggkkpmkfi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gottmditg.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gvmhfkjnn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gjqufqwyj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gfgjkpuks.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gkhsqjprw.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gsefkzogg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/guzvjoiap.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/goifokjvs.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gujmpmfve.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gxkgcrpsw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gmbnocdqa.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gaickrihp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtkktahkh.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gdngqnpct.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gxlcrpdml.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gmfoefnkc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/giksotzkl.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/gzymrfxzm.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gfmzptzre.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gpjkspoaq.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gvozeapdw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gwuxufxez.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gzefltcnf.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/grhkuuzgu.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/giurwfdib.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gurjqmcta.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gmbtbuutt.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gplsbxfjc.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gwmmkfdiz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gqasqmqdx.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gkpnuoieu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gunonxybd.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gbnvepeha.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gclqvfmla.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gjnuhdsnf.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/ghhsrrjci.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gvdbkltcu.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gfydeiakr.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gumsosvec.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gmxlnnolv.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gxwzuderg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gnlksdyje.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gonbrkaws.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gqlwjbxze.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwvmxeeko.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmjulpkbs.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/ggynqoqid.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gtfhhwkqh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gacovzqhi.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gmjatxkrv.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gpagozgoz.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gslafhffd.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/ghreafhrc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/goctwggts.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gvwhlyhxu.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gfsqorqgu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjalhygbp.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gncvjcbdj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gtooqdhnb.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gavxnyjwc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/grflbvqoz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gblwvjyqy.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gzhopaqqa.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gajzufcot.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gcvhowrxz.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gpwfnxqym.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/ghrproegl.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gbnhylwle.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gngwbizxe.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gosaxpsih.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpsdwwnfm.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gocdwdagu.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gdeffwbyz.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gpjbhjtcw.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gjdqxnbdf.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gygoxluqx.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gakymipwl.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gbbpxilgb.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gohummgsr.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gbdwosllp.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gfsoltflb.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gtnroxsah.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gumxuebps.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gjctsskfc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gclfltqke.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gjzhlbzjl.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gylsgecby.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gafogujdd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gdmazltkw.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gbpeusddq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gomtnwzsn.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/ggicvpvsb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/guxxibrmm.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gaxqwmxac.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gnvbpquyv.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/ghonkjrsq.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gpbfxcnbp.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gqqwpiczx.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gynshixqw.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gcdngzobz.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gqndeezms.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/geefyzawi.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gmfnuhlrn.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gjnheunqh.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/grzbrcghz.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gakoxtjrx.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gcinnllft.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gfcupczwk.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gwfjkktdn.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/giinjkuka.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gxscilani.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gflwexzps.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gtegcfcnd.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gwsjscnjp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gsfbnjhul.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gugzolipj.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gtpcuqqyl.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gyaejyfag.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gpsukqwop.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gyfavotgs.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gjzqrvreh.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gtqctoayb.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gpkixrdry.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gjijchjqo.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gglqgjgja.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gvnewndig.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gdxceelsw.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gujtymssq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gfptczfnl.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gzemifuoh.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gdvavjlck.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gxwjvaevw.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gvtnukwky.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/guxrlrhoc.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gcvzqspws.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gvpqizuip.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/geryvfkrv.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gcdnuhmcd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gyeqzdkjr.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/grlphnzsd.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/garpsykcg.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/goilmsmup.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/grblmuoav.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gsvqasdue.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gzcdhzvpp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gdbwgwtcd.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gzwivvfgn.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gdxvtzqqg.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gcphzegzl.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gphoihpem.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gbjbmnjcm.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gmpdslcrt.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/glswphcem.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gdfdhttkm.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gzrwmlvwi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gefoxblww.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/guvgomibo.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gguzcxepy.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/ghwnkzcjz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gixlsdbxn.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gzqwcgssk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gmjyzxgta.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gcmtrouyd.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gneogitap.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gdzowdadp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gueuqzxsg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmucjedrl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/ghwhqdvqj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glkgcysdx.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gpxqwdtgq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.hesvh.cn/Article/details/gwpxiedsg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gurcveexd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/geladoygy.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gqcuxmkjz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gybrvssze.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gldjpebub.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/graaeioco.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gxlmtcpkm.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/goabbwwfh.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gkpjwxwzh.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/guttinohe.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/ghntmcqib.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/glhficpgq.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gxuxneobe.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gdocygobx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gyapslwdj.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/ghnyqlcmp.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gvfqtykut.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gnbdohpoh.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gkyyxynoh.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gqgbbbpre.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gicpwqiln.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/glbmtdtda.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gelhyskyy.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gpprgymkj.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/galehaldj.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gfrhgcdjg.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gtnvztbto.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/ghmgiahkk.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gmvoenfrh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/giyhiykbj.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gyhjbfusb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/guyaizanf.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gnjqzzwiy.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gjyiczpqu.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gooznrrif.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gqgsmzpfg.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/ggqbdgemg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/grelbebxt.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gwmreewpj.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gdxveghyo.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/glcnowgod.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gigsrqyzc.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gvycypvcf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gscoqxvsa.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/govunvzmg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/geypledqd.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gajuakgpi.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gpjhlhnlk.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gicfrjwww.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gdylcijaq.sHtML


<!-- 参考信息 -->