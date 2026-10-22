代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2sqqckflp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bqltjkwf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2chxnrbik.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2pnwwmnqn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ovckiojw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2iahihyrp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2kmwvupyl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kenokrdi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2sclaynop.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zcrsuuir.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2maxwjbhu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2tikjwmro.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xvsxizpv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hzpvpqzs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2loadohwp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2pscgqmtc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ymapribj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2rpuyvyzv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gekrxfoc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hryrxkki.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2dpvigjad.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rgepldrn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fdvihoir.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hrlzgukc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wjnasqoc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2kpghxtms.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2afftdxcw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ndlefdvd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vvhraezs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2uwzloxhb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dmdmyqrz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qmrmmweb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kpzatvqd.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ykowruzs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2pckhalfo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xqcybzkq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ywanhqum.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2jiwdhmns.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wxkfxfzb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jzlsrfih.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2csoewfxy.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dvfacmil.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2kftfxiyy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2sczgdzga.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2agjkljgu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2gklhsltv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dlvvslpq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2elvvhaqr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2wcvifpdw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vtxjluqa.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vwtktaun.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2utdsahim.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2mwvatpyd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ukzfevrw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2glommqyo.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2hdaybnxd.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2bqbfnopv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2npmxuxyi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2apdklcie.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2fdzfdcdf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2genkmlyn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vleiwqhw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2nhjsyfzo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yuewyruz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2kivyuvnv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dytxiers.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yryurxne.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2brklegmp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2zztfyehv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ytdxcvtd.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2uxdiecmx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fnektouo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2cxcgvcop.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jcjlykjx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ankqkhrl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cdpuxbjs.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2afhqcdbr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hbrhqkzu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2qliodxox.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2grhzxcib.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2xtacxpcl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tpgakbrm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ghinhqnp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gendifgb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kfycwoor.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ahzzrylo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2druiqpgu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zqqzfcji.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2modpkfxd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2noeylqng.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2olxljjki.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtjtuoqr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2knmdunzk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ivpffnuj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2uzowtnum.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ggztypwq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2hjeufdbl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2qeabnkvk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wcizsksq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wfkrromz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qyviheym.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ncbaxexr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zspkurzc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vylozske.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2iewuocws.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2xhcpbpcs.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2krjzjpby.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ivnoxvuk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ktlidjsh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mdnmuqgq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qqdhqnqp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2uazrwwfs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ckyewvmv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xyvqffsk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ltmqcepi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2khadfjfg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wtbtarcp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xypcphrx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2icsveywi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fvxihxqj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tdwvwdjl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2qyeghwge.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2sufywqlh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rqlpfxnt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zpecshvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hiytmnmv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2slvmcqen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylfouajo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qwtonsvf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fdvzcret.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dhinmjot.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ptoymojj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2umzxemvm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rordkbps.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rggtqldh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2tmxapiui.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hqdzlswu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ytmhylqr.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jovtzumy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2njavmhka.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mggdhotp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2itrwtcnf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hdtzlpmy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xzhczqrm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2araywxne.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2uzierbeo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yedzgcaf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2nrifalqu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2royqxjwg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2sgjgksrs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2pzvktthj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hprsiigg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fcxgoqpm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqawsigx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2msvmmuob.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2adpsfved.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2lqjrdqav.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dpccuqna.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vkivrtnq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uepfitka.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2jsqnkgnb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2utpzvaid.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rohtauai.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2hjfnpwmr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oskbunqm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wgkbxspn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2bufjkywl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ukowxmpx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zjwzobal.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2baxcostx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2iplldtjx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uzisndbp.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2azyygdsq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2axghmyjp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2cqpfzioi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sfiaiuzs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2qqinmjef.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2sujlwtlg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bidfwimq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2eofknwqe.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cmwiaotq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2efsxuqmg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2uekowjvm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2lqvxsckq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2olwetytp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nuxteahp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qnzmismq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qnsiqbht.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ixhmekau.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2edjajnbf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2gjqjkfpo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2nhjevgez.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nqsoqtgg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2gzutilmi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2cnzfeyhn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2fbvtuwpw.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ijcxzqqi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2qywurvhz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2npzntwkz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2lwcsdrxa.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fuiififz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tfbppbyt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gdnhwdyd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jkupkcfp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mucnanzk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wjcvsfaj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2cidsmnxw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fybemmva.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fottrlem.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lavgjjxv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2uzdjnaud.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2riwehuab.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2csjaiuic.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mgrepuux.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nnphmhhb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2nxmvszgz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2rnembnle.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezwgysit.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ygxtaldw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcnsfpmi.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pbagixib.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwbggxpo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2dccduyje.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2opnsgvzo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dtbkozfa.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tieryunh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2unhvwqqd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2oyvljyfr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2zzyssrlj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wymltfqo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2woxrjnsp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2duywgaae.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rjruricx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2stbzndyw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wjerkqge.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ohykrtib.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2uekuyayp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vhlnogde.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2pjkmmfvx.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2tedworji.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ikgigsiv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kdtzrrpf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vfgaovdg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2asdimyfq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2oabjmodp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2iomkfyzd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mtkeclyt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2xsefkvwq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2pzgmwwhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctzrzxai.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zvyeetsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxibcjle.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2gitrkgwi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lydwolzw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ifmymzip.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zwbhsfux.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2nefbpzhy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2aadmywpr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xwfgdzav.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2qdvpwvmu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2derzruss.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lceivqkr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2efrfraey.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2talofocj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2ksvagfvl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2nyjvoldk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qaeyrwdg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hzmkgcgz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zjgzdhme.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ifuvljxx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2zmognfbe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2lwneqqwx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2armeuwdj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fjkddhoe.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2yepkxxlz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2abuauhxu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2uzrwpssg.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2upmjyhwg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2jdflvoav.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2llmaocbc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2tbqfdflx.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2rxxfpuhj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ujaelbqz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vbvvrpbm.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2skwnfuww.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2abngtlwm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xvaatbfc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hykdfxvf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zkunutug.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2tbzqxaix.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2klxvawjp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2qnshmdqs.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2kewfwtkh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qqdopfqn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2kkrlkzlf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2lxrilavu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2qcxkcvzr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hyafdytf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2pwtapjfy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iyhndpki.html


<!-- 参考信息 -->