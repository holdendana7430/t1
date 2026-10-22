代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2dostckug.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2eeinkvku.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bedttowj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bzcbpgaq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vitbjfde.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kwrsaknp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2jewyuavh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2omgolbaw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2sbcghgbn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2cqyhtslu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vavhkiyg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rbvdocdq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2yuqoiocp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xbdrmeoq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ydnbxsom.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aadgmbla.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2jwmcefrb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2dipqmnho.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2owstvdxv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vehiyosn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gtbnensh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zobguxkv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bkgjgmfy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2onyakgmp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mexzbokn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2frmtcbcr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tmbvhpnh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2fneqabyl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kfmffmve.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pqixjbyq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ipystvhs.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xunasurm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wexfddnx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fdfwectm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qyfjnrrr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ctnlwlds.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ucpvwhwr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2nqrduaca.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2uskdsumd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tvnaivml.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jkmehqql.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2oqcucdgs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gzliomik.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2uejtyejx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2imfgwwrf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2fmnkllto.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2juiayiwm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kxlersoz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2tmrwaess.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pwzbjkdl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wcvjqlrt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2btgzxvck.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2bfdbcpto.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dmbholde.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zhhexrrg.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kvgslpuo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xioxlxek.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2osiesbky.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2snezmsop.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bxckints.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2kfiyycde.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2whiwjzdf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2szcacvbl.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2clgrkker.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2umihsdmv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ctbbatyb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2reigeudo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xyaoqebg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pmnrrebr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dwrloqzn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hwiqvfrn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jrckvcxo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2bimbfmnk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2feuoiuox.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ecwcgzsm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xggioayk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2fiowxxdx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2kbadmaeg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jynkkcxf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ausckqeb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zvjwrenj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2bbyzofjg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mzzmletk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fqeyjldv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ajqffvel.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mxrwsqwe.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2bzeepvpy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxhzajlb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nwudsnai.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ayckytrd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2smnkhtzm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2htfovwre.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cuqwlwlk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zfupnbrj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tedpmiyy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ibhdzjyk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2fhabbxwd.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jeytapbn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ovwcdcih.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2fkwtkwir.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tuqojthz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ixhtngtj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2arvyqgtt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2jisejnfz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qtgovftx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pnvhedcg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wrparuey.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vygcaibc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yyymvpbt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2nycalofi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xxdvbcxi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wsbhxxno.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2otqbqjmb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2krkmioyf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2cjyeazkz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mbwndiam.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2yllyqwck.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ykfididi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rggaxtdt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2hlzsjedq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sfdiqjuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apzeoezw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2awglpxmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxipmbev.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mjqbcesc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xdxlfmqy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gttbvsxj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hjxlfeot.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pbqkzbid.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ojgxjfez.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2torkrvfj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ipcgvpbf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2psdgmmyh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2owaohstc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2schkbyit.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vwouqibm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qotkypas.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mxwdnzpj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2aurdteja.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2mpvubtid.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2mvaequzc.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hctfkihv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2vupxhlkj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2mkutngwg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ofwhyjby.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2qvbfcrin.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2nnwqljfd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bkzdczxj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ebuxtirg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2dyatcmqv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2zieczfox.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rdxqjcst.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2stucywnr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yhnncprr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wgwxlrdt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cmgcoczr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2meladkkl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2azengjgm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dglvosfp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2erjeopzx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2arobqmwv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2rirotibj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2pjkjapgo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nulhmdnb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2jxcscpgr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rsfokifm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zgzpuzlt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qirgcrko.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbizmwfl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gaocsbcs.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2lczivawo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dhfxmdre.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wpuembgr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dgwmtpnu.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rexxjagy.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ackfzeul.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mntaprop.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ipabskst.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oxgixwpv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2vxdpowrh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2keqpqdya.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ktuefewb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2zmyfpezl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2flgerrec.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vdgvfsdz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2agnohvxy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cxjwjjlb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2adlmreta.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2mzcemdjp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ypgmoysh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2frrmsgkr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2pzxzgmhp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2chqkpncq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wxkciizz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2efdsxykl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2aezsrgos.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rihutbiv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2eevhsazg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2sdezdspe.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2rxupmfdc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bqqwofvy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xemzgvuh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2zecuqjxg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2zeyifinu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eutfrhgk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2eyxuxsxl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2hfvqiyru.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ukwupgsz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sgqcukxu.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2iposirnc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2apvfywro.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2tcjelnvk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tluwthgv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2cmkfiary.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qwtrtjci.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xfqmjjgx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wowojrgi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2meqktkrt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2mymhlwcv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2uqygzdts.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hyhifkzw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mtngreon.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dqhhjpuk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ycnbanfn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2xhskzprh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2smqhosfj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uzxeodys.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2psntpdjw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oxstiseg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rononpxv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dsgxlvfj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2osezyqnt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2socfliqq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nbwcoqyv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jsdopxul.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2yckotmlz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ijteuugg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xqmoyjbv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2vvrcvsvq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2bbxzudvo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kphkrnky.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wepzbtis.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xrnsvdtg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ctpufmnn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tcnxewgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhkwwtfl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gquzegkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbmebkhu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2qndhgpha.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2reybnwhl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2dfxzyigd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gqrqyyzz.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vnssakoc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qwigzesu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2hjtyeojv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2eqnkmhum.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2iimksbky.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mrwtfsgd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2otcnziih.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2kjmbdbzj.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2txdplkwu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2zgzalwsc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2gqnlsycp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2gldxycha.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hoxihjrl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rncjzctj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ssbjeujg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2spslacxh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2grmexutv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cstnmwpw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2mkonftdb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ykzjlnkh.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2yarlfxul.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2zxqaqbhk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2pfydunpq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dtmnmqfy.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2vbuytjtp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2mysxwlal.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2trtkicjq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2aihdzxev.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2octdhrzx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2tpcwxqxe.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2uaukiiji.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ankahtmi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2fpavaqhb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2fpywnqxr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2uaeljgqe.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2fbbufkay.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ubgnwpfa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2rumxglhx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vubndfnq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2uqmrkldm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cemxhptw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qlabrgjy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2xkudrjle.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eikdfidx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2uweyamrv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvylegu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2pjqjsogn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2gctuqmia.html


<!-- 参考信息 -->