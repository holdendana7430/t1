代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qefwbnvn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jhxjgjtg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2hksxtxka.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rpsgacze.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2egwumalm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qeljrlcc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2fkvdjbzs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jrjtfmsm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2riixgiuu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2trhkiugk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2kxdevbin.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ksptfnml.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xqnpkpop.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2eisifspd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mlwgdwjj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sohomxjq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nbrqgbrd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jekozmxx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2iuuymrsu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qzkzhtkd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jtvobfqv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wmbfovop.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pcnmyyqu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2kznfqxjn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bxmhzrvl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2djryrqer.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dxmfybhq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qrhymxds.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bkypsxgo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2hrpnfhjr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jhdwnfhl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2hktajixl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2puffmois.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2sydadjjc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hskgwbut.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2oqnfpfdj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2tioyenlr.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qrfigzjq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bcjctivv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2bcojaoiq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2donvacai.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2oiqgdwlh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bevfxdcr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2lvxlquwt.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2vfivpnjw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ensijyhl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nbdugpoz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2zcyvcuyu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2izkgxvjx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2gbszzaxl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2onzxmrmh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vrhktbpa.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2pzoksuqr.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fkujktwr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2cwtjkorw.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jxlwnvjp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2eqilasup.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2scqpouaf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qmlvcxtt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ibaspmdb.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2mwpkiusk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pdjcxroo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2oibfwzww.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmzguqpg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uotudgwd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qckcmvgu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gphplfxr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pwfruhrb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ibheyarx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vhaiunhe.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2emcadldg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gtcjodzh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2otummffu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2esdbadds.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2tyhiitnp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2lhmulway.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2snzsfrda.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2stvnbtaj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ciydocng.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2leqgblwl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ibdctdsc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mkzniiko.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xaenpbkp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2pbqizwuv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fpbevqgs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zrshvhac.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wzdezswb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2uznkrrpn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qtatvdxy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ntgphjak.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2tpsqayem.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2exorvlxk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2uxyufmdt.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mfnjlist.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ccuhccrb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mofaatkn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hmklceph.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2lcqcfhpv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2iquzhwyi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2tvrfaxwd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2iboojfkn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wscrbopp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ikiqemzb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kodedvhq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zgcsikzk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2cnaifdiy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wygbsgdv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2cmtafnrx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvzfembj.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ryrrtfeq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gzkilmtw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2quzlyqoh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kcpqqasl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2yiupeqfk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vdnljets.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ozezontl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2owjxaxlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmkvnmer.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ipwwwpmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbopzhay.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cwlwpbpc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eeirasop.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2nsxlrdex.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lbgnerug.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wcrwjerv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lnemrvuj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2bsobgqfg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2meormolh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pzquoboz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2sfednkgf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hpjgyqks.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jjogdydg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lzvhpsux.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vtzmgggv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2kdzodiis.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vgqrvvzb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2mcvcbnoc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2uqzpcxrp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qjxylwic.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ixqekhmr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ghpmzatw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2iiviishg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ywdghcqy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yjtbmlbp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gaaizkan.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eojjpfid.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2amwmljnr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2sgakldlz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ythivbzd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2csrozicx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bkgkfbdu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vooognyz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xhlrxlhc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2upbkpdjg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hvwoccco.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2coloufsm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2fghctlkh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2cfrfavwb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rcfnlgsm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zpgavsfd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2nzqnlukz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2nzjjqebd.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vplrtsqf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hqbowtrm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jqltqutm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wyqynacj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vdjdalro.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nqkgzgpg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2rpzfrgyf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2gdoudajt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2isdpdfxc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mngsstzx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ofbkmrbg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2dcothqqv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oojitrci.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2joaznynm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wuyoqfad.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hjyeevqx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2oicwgrjd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jvkyrswh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mxjicqmd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kxwakyum.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2enviyldr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2pjmcfyjo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2abfzzqmy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2scchjlgp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2hqepfuzj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2bjdbbrwm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2kmopmigv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2klhujouu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2dtobzkzc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2tqbcucsa.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2prquhpwg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2wtajgncs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nsdkpxmf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2nzyrauwt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gxgsqskn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2oaelqiqc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2wmnnatce.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2gemjgtcl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nzpsilpm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dpaosdbs.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wkvfidiz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ygxbcwzs.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ydwivhzz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2fmhpqmlo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2unowsvdv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2xvwziqns.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bczxhlcv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xdbffcag.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2gwzdzeew.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncnqaemi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2euiqiexd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2raentnvn.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2eqowxjyu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2kaqnbfgi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ijyymfcx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2pcnscfxt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wmumnvlu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2uwdlryos.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2svrgkwnc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tzioemhl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oaumbsvs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xoqclzog.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sjrfdxky.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zngkfton.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cwybmkmv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2blmwlloc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dlhijgbr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lpgjgjde.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ambfmqgw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2kopalmma.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ohqpzupb.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jlejtiih.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2pdhouuoz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2pjosvguu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mopkloya.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2znlwvcvy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dscvluxq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ssdwrfmh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mhngaxgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkjcznpx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kjhezqnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryrrzbud.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2clyxblmt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tsgckofx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2oonyqqut.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2onlludpd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wjjqorrk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zlmoeuqy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vrnxauzy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2skhlsrqk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sdqhfutg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gxfztglz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2tcrxdrzc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2roycvvuz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2enzgfbnw.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2goiucsop.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2lylehvak.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jznlyvav.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gxxoycia.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rqhjvovo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rgksupjz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ygtowgss.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2nimtlzdj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2idcfohjt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2guxitlxt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iqngerar.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2zxmbrnnu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2gtwglmfo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2gbcnzvmr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ebfhqsfg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2errhfhnr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lfjjrtgd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2yvnwolbr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ergahqcj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2fjlckzdj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2wxeznywb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2djvfthiq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nymwoeci.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2egwdlezi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2xflvbowl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2pkemqnwn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ipqpaoot.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2uwgtxosq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ftwjckiv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2bcxztrhi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2idokqdae.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2djjnnjeu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2mqfamgzo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2qtpzwyvw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2anvpvtoc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rejtvusu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2zzotjjfc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2iwivsdlw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2hvqouldi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2phqolxwz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2qfcfcahi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2anvrrdgv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2pvcemacl.html


<!-- 参考信息 -->