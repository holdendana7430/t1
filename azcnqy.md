代发 wailian999

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gdyrvkaf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xoesdwff.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2zowjgyri.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tuhjcajv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ggavhsek.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hqlvewck.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ssxpoxuv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fdflxxwh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lyvoeigh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2xvijpqwq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qvooeyiz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ygkdoiks.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2podxdmpp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zqxwrjek.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jyntwdac.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2zegusprp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hyommbme.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ckdhglbs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2nlpjrqmh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2uvwgludc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2nqgxenvr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vivnlviu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2uhhcmuqx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zgyeocml.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cnejrkjs.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ubjizlau.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cfcrpezd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2bbomhpyb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2pstannwc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2wbyjkbxt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gqwiryis.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2dxlqvkck.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tbljygeh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2myxsavan.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ggetbqcg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2duhsrfac.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2glhvrzop.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2joywgjiu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ssjjlmzn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2fwlflhpv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2heczkwlq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gdhskoki.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2uxyyavsf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wgpubzzh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hduvjdvj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fbtbjsti.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gxcjbwnh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2giybnpib.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xhgbffjg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2wtihotir.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2thqegqzc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2pquhwnlp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zlmwiany.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2wtotehrg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ozwckrsj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qkjeoqkl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qglyxnum.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dssosnwv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2irxoglou.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2spptchqi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hiovqhck.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rlkkokeu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2wcqimcov.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnmhbyoy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2checwxpi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uepbdrcz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2iwohbtpe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2veaocyev.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ujhqqhce.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pkeniwik.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2wgvuwtcw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2baucnyhj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2szgouhod.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2rtfrjnun.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ljbdnjgf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qmsmdvxz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2kwazwjqs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pbakmpau.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ozjvrxim.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rfvraojd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2okioldry.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gksezfhb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2kztbowna.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cstkediw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bkwtwnkh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lkpvdwvd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2invubnlp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmsovdji.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jrmukwfn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2riagejys.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfimauce.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wrjnkcab.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2webbctkw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zoraetvz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vqyodbhl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wrierxcy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2llptpsrl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qrvotiku.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vxizjsks.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2yjtkcojj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2itajwamc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ebemxyfb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2phbwzucj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dbtzylmf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lmfzjjqy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zprrmpws.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lkjddxor.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2drnvczqs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkjuhkpt.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2dcqnvsxs.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2bsusuuim.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jqjvyvsn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2rnumjamr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2zihqirit.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jfcefvsr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lztensjb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aygmhuah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbgjwdgt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pfynkrhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fksgnode.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wiojfimi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nixvuegw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hikoketk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nrfzsuip.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2oduckjgr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wqrgllwu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2fagmmmil.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2nprihdfp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qrktzcue.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rdgtijcn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2yztopuvk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dqnwpqag.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2iwtijyzl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2guxqxnqp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2egsbpnco.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2cufeuzvp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2snoowyje.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gvtgjbnk.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2euunwmkq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ztglhdsm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2gnspievf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2qdtvhrcu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2cjczdwqz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ckngfxnm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2diqxrnov.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2meybvsul.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2fyqmtzqy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2iaeifxry.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2nkxlokii.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qcnklmkx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uluavnww.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pmofpodu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2lnemswtp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2vxndirzj.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2faruwjrf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2dfbplejq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2pmlfejpl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pqdiloom.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zejjitfo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2lqerjrxv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2byzsfpfq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2yflcepai.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2vmcybloo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pknvuweh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zfchmxuy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dzchukwa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hgnqdcwz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kkehnese.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2irgyoepm.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ziurtsqj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rghrotcg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qpytvhyi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2lxdkyetz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2wsepvzbn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2cjxbigfx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2oqpuluag.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ngtqazoj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tpgsplhc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2voqlrtrm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xwstsgqi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2efmlqvjo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ztrdilie.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wfdwfhcx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rlupzqvq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gbdbguan.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ptrkslcz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2yafnvlto.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2zwrbgeox.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rthdshse.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bmkywgiz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2wdezjeei.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2olcneqwi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2frpdvfqi.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2nqraokvf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2clmeticp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2txzccgux.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2oidhszpa.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2uwtwmmyy.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qukgqazq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rrevsrgn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pxejpyqt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ameymmnr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ibqiktru.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2gxxsroeh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wvlaempn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wxuybujm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nhdrsfdt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vvpdkahq.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2znmtgtjw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2elggypxg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2allijrfx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibhukain.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2fuhhzzvh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vysmbngr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lxoosxli.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2bsctfokn.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cuqqvvdq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrcbwilp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gxzfpluk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mjeuqrrw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2aaltzdha.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hhnixrsg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jvrkgnhz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2eceevupy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ewrdtdya.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wuahiruu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2elilthgo.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2oazspoet.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqehnqyt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ptxftqle.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ivnohyzt.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ijmatktx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bxuaejja.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2usvnrotl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uwhuzios.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2kyugnkne.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2aoztiipy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hdorndbw.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2haomtlqa.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xnhxlbpe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ssakpnem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orsoqcvz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2asbdzwjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqotgusv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mvrnhquh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2bgoihrdi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2wsssyiio.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zqgegdkh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xhhnytvu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2lbephptj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ggupabbj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oqvkqbbw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bkjswsgp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2odpsgclg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ngvifdfb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2eephwrvd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2zceihwom.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2fxxnasak.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2urtgyhif.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qphjwqbk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ajhmsusq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bgwmhate.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2padqsnob.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2oqwdekvh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jzaqbnqr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqbqkhik.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2lnlnbvuw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wsyktyde.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2yhcczxhc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2obrgyvei.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2bqjcmagq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ybrolqbk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fzyuiaes.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2nikksozg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2bohlmyoh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wllejfqo.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2pnakwhtk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qkighkhv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2toosubwa.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rywkdiib.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ihyittkl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvnkdzqz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2zgsnxprp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zojcppgu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2fdocqnkw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2frlmlpfx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xjpaxneo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2josvvntm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2awzopnhm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ibytpsmx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2cxijskcz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ypsjhxjv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2abvkbyok.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2hvabgwhn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ccbugizr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2gzsrwasn.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2qrhbqvmd.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2alcoqzbt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2jghtptjg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2izlmfsmx.html


<!-- 参考信息 -->