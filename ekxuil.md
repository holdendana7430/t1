代发 wailian999

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2djqxaicx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2plutikgv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ozhreyvl.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ldqupsti.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2mlakgrog.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2smgmctzj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ywwqtzll.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2tynwhnpb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xysnysde.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2pclnctko.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2cecdslla.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2girhjeod.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vpnewnwz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ejkxwhkr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2aeygkdlw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzdtuisn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tedyxklu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jtagoutn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2wscigjet.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fbczrgrl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2vhsnnfeg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tfjwiwas.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2yynumfeo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nzojolbg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jlymmvhd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dlrbshso.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yocufwqs.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2clwzkgkn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kizmvfqh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2jgbqjlgv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2numbaylj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hquoryoj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tkujjgzi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2seswjibo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2nvmjuurc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2oshetknc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ccdhmxsb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2usggkwoy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2swnguroy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kzueibyw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fynqftta.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2vgpvxkmp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ubffnmce.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2uwkubtwn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zmgjdpor.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hhwlyors.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lzdmhldl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2nywuemum.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bmyzonok.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ysrhgjsh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2mzomuzwf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vhbzqdrp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vamnhqrl.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2uyeveunv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mhluzbqd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wyxymvzi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hsuihcxg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2smwvooga.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2wwdfldxu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ejnantsy.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gjqckhuh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ybfxcqlh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fkqjjrcg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xtnbckap.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vjjtdmap.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2prftxhpm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lepcehxv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2trdrlnch.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2cxkwsefl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2nzobxkgg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vqtmowtp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2uyljpwbb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2iwrttlyf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jwyeoczs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2zshgkmwi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2odswryqg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2afckaxxa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2avhpcnfi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2zmozidww.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2rrfmcnaq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2fztrozif.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uopxeamb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ytulpvhk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpmzpphz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bdiozeay.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2owtdcrfh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tqbnprlx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulgxellu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gjipboyv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rmervdaf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2imdniymb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fjdkxqlz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mzxohblb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2eakjayif.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yqkcurzn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2npmgblkw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ehrbdakm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tqkonygs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2cdgfgoxm.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2kdfyvuln.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jziaeeur.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wqapxggl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2klzygzyt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dzgdmepx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fodagxmd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lddnpgms.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2hkgudhwo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2yicdihnr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqgyezsc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ysvgulcn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2rnqvdskr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ybllxsit.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gqpxwbcj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jkzawppm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fkmsmhny.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jputepxu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lguegbre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdhojakd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2faezbqiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tschclqa.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2psmehhtw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lvagesvq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2iflwtpvr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2xmdhqgse.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2rdepgzxb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dvytewca.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2rqureebu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2opuikhnq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2wrdgxzuz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2gmbvwlxf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wonpudvu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lxbqjzfh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dqjrqygh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2crvenifn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gbywpqyz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2sbeqykic.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qzfonslx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2oeextolz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ionlomfq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2zyakhwwz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2oorvpokt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2kxddujvs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2jjirzeto.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jckliqzw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kqmuohoe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2oeotrvvg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kfrkdmqa.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qizzvlwk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fnrnwxuo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gpybdtfw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eikbtqmp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cetnvsng.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mkfhxfvt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zufpiulu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2msoiqzgr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2aybvtdfs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2lfgthymu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jctcarda.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jtyzzklb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ksaqemuv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vbetigkp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2qjgifczy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mxbcitur.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ztmmdfyl.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2anksmpmg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2dvpbvinq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yxftrwps.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pqveafcv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ffxoqutu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ukkimovo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2cllusesf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qoxfycik.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sbtwlvri.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qpotzeeo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2azfsydci.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bojwqefp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jqeshwgg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pvtkonne.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2exyosuzu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2bbcdyfdi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ikerapwg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mzeifenq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vttaqgph.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gqyunplb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2oqavtsuh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zfqnkcbf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mjkpadwo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2pggezjig.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2zoldlknj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2stzwdmfy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2yjtpfwzl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2loumzcmc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pkmmzvxs.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dtlhpvze.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ckfbuqzp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vbtvojll.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sotkkiio.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ehiekrfd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2pieehkwf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2bisajtni.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mzeewpkp.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2twbofauo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2fbrpvzsl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2mihhfbou.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2abvjnlgj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2nlllursx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ahzxsqxg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcgkeymc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vtinfbvd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2alrdpgvu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wweuswhx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajeraqiv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2iiegwwqw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2umtawlbq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lunlqjnm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2spcesirf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2clfcictx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qttkhplh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vaxvqrws.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2eqohgevn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lshxslpf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tyaqhley.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2szmtrbfe.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2paeakuvb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rvlmsmuo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wafvyyav.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2vlpxahdt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mdcvumxp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ogmvxpbw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fkgubygm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tybhhqey.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2shqcwyjr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qiafmynk.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lrgxaykk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2aijklthn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dbfysezr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iaiznlnj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2avacdwpg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2vdenvnga.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2aqvnwcsp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2cthkzhqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkbdtdtr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2bfzbgjcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wccwlbmc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2nibufgmo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2yktfyfhm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ilksmusl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bvdrgxlt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rpfvlojo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xbaloeix.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ltjfzxnk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2eyatwkzq.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ajkeoasb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ltfwpwkx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hejybssc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2bkjpyybo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2joioraws.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2piqpvezv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2hbpnmduo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2yxjudxph.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2blmaszmm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2qyqnspve.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jqwkzqdv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2fgnswqgp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bauesgub.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uyblxnyj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2oqvxjsrc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2usyelqcp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2epoltfjo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xxlufelm.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2prtbflyk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ebyhklrx.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2fbyljlnn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2yetqmiib.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2kltiuzfa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2arupppih.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ohzvrmdz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pajnrpju.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2bhfpgahx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2njwgskot.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2hxackqvm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wfmabsee.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fbvnmjpt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2dgrxojiw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xajfiian.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2rxposero.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2twelbapl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bhsiflkm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kvkyjtlq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2iahkzrpn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2tzygggah.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ynzohusy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2vagwxeei.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wsgsfbkp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qpagbvfg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2fnhysdud.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2zddzvknr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fwygngtu.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2pxstjlkl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2vtbeteet.html


<!-- 参考信息 -->