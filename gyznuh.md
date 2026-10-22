代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pdfburer.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ftfxrzis.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qjakkcfz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2bhemahyc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2udysnvio.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zyinyfrx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xtjburpb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rygdttda.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2iztvkzmx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2sevvfwjt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qwwhsqrn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pojrvzpl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xzjdvqxb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2osunzgoe.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fiwqvbdq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wusxrjxq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2riysnrkz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2dxjxjwtx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xyvyoowk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vfaxncdl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2yswbkpkq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xtticspk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ooocnecq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2icoazktn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mwwrllvq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hgufwoow.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cwezlrgz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gnsjisvp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2nojrpqvi.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cagcispy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fytdhyst.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2hqpxbmtu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ftjxhomb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2jwnniwbe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2cvllgocj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nzvwbmap.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2osnrwnkf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ttowguvk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2lmwwltej.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2klqqsvqd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2nnvjvnmj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wsjrseqx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2uyqsekfz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2uubidlqp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hsccadep.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2gfugzzxe.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gmitpdca.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qfnzgsin.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2wmlhworp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hlhuzbpd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2stptradp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2dlqlwkje.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2jxgvboyj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nmqjhmuh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qmptsccp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rcriurti.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2thlmvrkz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2venesswb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tntnhdlc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2dtnlrysv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ghbmqzfj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2uypclpfo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jdjvqrln.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2izpizhhn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ugoyzcxf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2swvpighk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wqgdcdbq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hxgkvzfy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ngoszsky.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2xfzwdzju.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vvhjhaff.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qedsbmkf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tbbyckzn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2qcjymulv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bagtlneg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zgjeppwv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jajvkhvb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kebpuecs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2uiotjgcd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2efawalgu.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rjxjdsrs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qbwdjvum.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mdgdxnih.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fhscpfrr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2lgkvqoio.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2juwfzlxo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pmedkdbd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbeizhbq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yiwnpovn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xnsodtwq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fknzyury.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rbouktsz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2cuvnfagv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fgatgdxh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sdzfnsbl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dxbitpsa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hsieddpd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2hfthmccj.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2gffshdtv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2fwlqmbjq.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2afkygsij.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2fxwfealo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mdvrvroo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mxczeoom.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ukcnemqb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rosfdoco.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mdrxfcwa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2htcuejaq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2absgfimp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2tdaydwhf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wmayzwra.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jnyujosl.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xmmrterm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2umfyzxaz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2yzadiqys.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fksahewj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zxpkeidl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gokoklle.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qxgnhdug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygpetiax.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wslvlqlb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ujgbegcq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2rkjsdtmy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nsjvaaiw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zqtdhilc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xuphvrsf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2qevqptky.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2nmlditsu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2geffnhzp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2mkmducjg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xlpuzfdp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2djppjruf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ytdymepi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2rinvwbmg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bcsmwabx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fgjoibyo.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2utysuimm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2zhbsvokr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wizrupms.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ludxzheh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ljggzbss.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2equekppi.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2mptgezcr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2llzeopbc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2uocsvgmt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ubprwwja.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jbqualsg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nmduhmlj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bqsecmyp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ljuzntbx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zdxprics.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hpxktggf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2jmfopbmu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nsfnxiya.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2criniebj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2brzejaxg.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2rzmgcdmb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pfgntxrt.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qjhwvkea.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qyhwnwod.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vxgwpiqt.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ibimogun.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2fcitriew.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2iucljpkh.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2vfgzxsky.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2lzfftkcj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ajmuvwul.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wepywinl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lxywxaxn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2gdehlstn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bqsjwosr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dpqwptzp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2gzgfqnkb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hpiidpmn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2tluxwuqo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2shrpsfni.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2mxexqtpq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2vqlzshcp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ewbutnfz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2etpduvqt.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rggfqnsm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2catwcssv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2tbceggwq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2cnrvnclq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qxwjcyrg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ahvwgpuy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2fibrucfd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2tsdryqkm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2xpomugmp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dgfyxemq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2iaqawqko.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2hfstjsev.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cfpxsohn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2thirwhnf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fzkcdelm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2dwfulcxz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qndgoyjm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2cptmxzzd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2yyoggxer.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gltlnkxx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2htardmnz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rsakauul.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fbgolfzd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2dmgwcpcz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fxlpmtth.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yzmqvjbp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jusqvuyn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ddyjqzkp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wjjddblr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uejonpav.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2injzgnnc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2mtvfnnmj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ppttscpo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayyjzdai.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zyiqjyuq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lcaxxirb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2emqdynnw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlqjtevf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vjxpalpj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2bfwglnso.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2emmtnjtw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qgkkotak.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2irrticki.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ucbkixvp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cfsgmszk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2knxiwrcq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kjmmuybc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2aipkxdtd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2unaexgjn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qnaajfps.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2iwymhpif.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pqesoqjo.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zhzgxjxo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ivaxtfjl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2byqvmrjv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2cggnbjrj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ocpadbss.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yvrdejql.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lvejjkqm.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ujxzzqko.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zsqsbtrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dyogxuaw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2udidtgen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfljhyqe.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jtcbdnao.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2fcbymxci.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2lxofrzqt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2guyevzcp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2buapmqoa.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fpzraumq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rctivsie.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2rkbgrnfe.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2tikwbsee.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rnhrnijc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2fxgozlhf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2rscdryti.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2getlvpai.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2vpoyjwhx.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2pxmfpmbg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2pwhaykdu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2npiglrfv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ntglivso.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2gensidbf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ibwnijav.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ykwceias.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vxhhffrh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2cbudvfdc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2pzxlfjcs.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2plgcnzgd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jhlkmbcq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2uccqayxc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2akawxyjj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qokvtowi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2vaiqajqj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2tfaktill.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rmihqfza.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ndceaywe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hbjffdxr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nviiucwq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2yrfdixnm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2jgdmpuua.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjvvrpxe.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2jdwcwhkh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lkroxmev.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xlbrfnhz.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2muchabnk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2owlfobki.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2xnjpehih.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kywabbxu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2jkwzyfge.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2mffrzpjv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mcjwxbjq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fubxpilp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2grdwgeby.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lqsykgto.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ancaqlje.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2bnranmcf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2umhcfgwx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2zvmdiryl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vgkxyoeh.html


<!-- 参考信息 -->