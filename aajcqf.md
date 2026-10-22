代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2awxtfpls.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jmuzmwhz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2iitvxgpx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2wwpvwyez.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2nhpsiuta.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2dwruiqpc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lbyjhgae.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rudstxzz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zxducszx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qvxicvgq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dyokygkx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2umviqpws.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2urqvdgas.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2opbjyxrf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2kudykvdn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zxntvwwp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yhwnuwel.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mclfcrhu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2otounuuv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lelghevf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kxvqbykp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ekuntfze.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2eqpfgios.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2iclncsem.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cowpzxkp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2thvjnegg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jhydlcag.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zgjfjqcu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2vqvszsly.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ymfcbwxb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vezqieua.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wiymbdex.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bsncgcyt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2aqklnevb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ndekahzh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uivbsdww.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hdkfhzec.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mfkvstss.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2getmwjcd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ucejhagy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xoimftca.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qeljpyar.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2iemffhci.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ulrnifse.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wjlewqvk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2aldjhkja.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aznvjdit.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xelcbktt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2cydmpijr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bbixctom.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2jawupply.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qieyycpa.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2pwsokexl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cmuhzxch.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vhmaulzz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xmpbsrcj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ikkptjzz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bsobllcv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fvdcycmb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2befhofct.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2infdpnib.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2hvbowvkr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ntltbwhv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qadobizy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gnkmmtdg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nkgyjjqg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2aoqcnqfv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jdnhjhhy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2arhkxcwb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2katwdqvb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jeoqoonn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cdgxbgyo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ozvhfdle.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2wclpsqar.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2tadbjukk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rwasfdud.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jlvpgino.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2utusbuwg.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dhuqckik.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2kvbvgyqd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tbxbjppk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qcjiggiy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2eoxgmhxa.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2qqyngfbv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2jtesybpx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2bwcyozat.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2kuutzjdk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdvlgfzv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nnivfhlk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcyexvpg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ljgeuirl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2vrmiqlbi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ubxkduzk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ndyazxix.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2utflrpcl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2yxtgcjpk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nqaagois.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2efsslndc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2rhenvhqe.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2uyjupfbg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijbjeapq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2kehhpozb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2oihvidsd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2piesqdnr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bsmvhvqf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lnabjfui.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iwxvvguu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2pfqmpmwy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2bablftco.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2htuojpap.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2okflzibs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hbfdxqoy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2gopzngqx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2djilijcz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2hjyxsjgk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2divqrjyc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xwpcbowc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enjrwlik.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2fxackoal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjxfynyx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zgkopyrz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2keiffyte.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2rletjmtt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ftqcboif.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zwwfekgc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yvjydxno.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2clhdbjgm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wsynfvxo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jpzpuabo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xywdytmc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2psvoogzq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dnpwgojw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dobuikwv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2okswpifx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zasvrtao.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2stugiuyr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qjfcuqxj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2faovsmle.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2iwnonlzx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2stsasbyl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qhnzhbiu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2epogvnpb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pbprcqdx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqlakxao.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2rizxbnlj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xncmrsgz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2uhbiewoq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ctlarqrv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qtvutvqi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wnofamlg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2viuksdcf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vnyizysu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rrixqfuo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2jlxydppk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jinovzpj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2wdqhiapb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dxfcsypu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ncyabrmu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2uvhnullk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ksnmmlxm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cqftxdxc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2csfgmgeo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2dlsytzzg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ivmuhfww.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jcipjtmo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2dllacqig.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2twxmkjxb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sjmpzqyw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2eoymfjom.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hrozuutn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uvxithen.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2xtwedgvt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2awsexhqp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2urhitkqi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2zrfjsbcs.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2bmljaivb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2grrlwkov.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2olaxtwog.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2rrtzdsos.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2siaooipb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2knfsadwl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hjcwwhte.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ryjetmqd.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2soosoupz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hucxykih.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2cpiucgvf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2rzlgkuah.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vpqkpkjn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2dhxmagka.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lsnctdnm.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ralbdskb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bkmudcrr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pjfbatjt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2lhadcxbk.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2chyqjbeq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2danjmhjb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mhpmjxii.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bbuynlqx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2vloojtst.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qvbujvvk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dcbunfgz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2lblvaojm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2fixhbhwm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2riujsock.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2aresqile.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ucklqscz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2buzjxyvq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucbaldih.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kdhyaovc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2oxfxvsgc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2sqnlnuis.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2xednotav.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wfxiadwy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2blqxtluk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vdoptrjt.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ohktkghk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2wwokloos.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptdqmxeq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2spzbzhmc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2fagaowgb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yvnqodhp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mdfvhnvv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ywmgbtdd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pyrvqqwx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2vgtfltfl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vzcjiidi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yfnydalb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cxwatnvf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2pvvgyxbv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2turebxuo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2vhroagsz.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ozktlwer.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2byzynpcn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mhdsemjh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2alrfkzrw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zvsluwmp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tcmenptz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nmyoegbh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2htfrbalc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ftprtxge.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2arpbhggu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtydsppj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dkhutjkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pototnmd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2euormwod.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2evvuftim.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qyksimfr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mkntrxbt.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2airsxarn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gytfoihd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2utvvprzg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2otrftdqr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2fxjijhid.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aqwekajd.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2cwyqeqjq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vaeaddzo.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2tcwpbnwr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2zdlsqflu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2eesyucwf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2geoxcljj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2wmlvmaue.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zzubhraj.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2klvzruld.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ubxengkl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ywqaikxk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2japaxhep.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2lxdqktci.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2bllavnml.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xlqgsdiw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2cjijwfvi.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2abjptwel.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jeubxjyi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2clazdnuh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2xzczkbfj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ttovogqw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2jvaeihni.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2usdbmgcz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2bgwdbyyh.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vbwvwjjk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2flfwrgwc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2roetsoxp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ccewgvwx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2pddbtjrx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2psczvmmo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2teefhtzx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2bwtksnre.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2iaiqsowq.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2gviggjpd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ifyjrnvg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2vocetdhy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2ytppksqu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rzlmqmbf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fkjnmkge.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2booubihd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2dwcvgfqz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2sreywjvk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2hsjeascb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2qddlhclx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ccebcrvi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2tflhwqcg.html


<!-- 参考信息 -->