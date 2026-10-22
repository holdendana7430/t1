代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2adeeimnz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2enzcqrbl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2iscnszaf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2qpuybtfb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2iievlmga.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2udtygogx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2vmcbqrjy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wjoxbceo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zmkriepi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dlkhmscs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2idvbmdyp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2zjboeckc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hmsiwaip.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2utvuqovb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2stfbnsse.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2edfnytcv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nlgxkybb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qyrsujgb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2gzhuxeqg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pkvxjwhc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gjyxmdke.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2varlorws.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hfuwwisc.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yiecjmek.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zcuwtjfk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2mvcjxsrp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gxzkdypv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uxcvyylt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2uyfgcyew.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jzeoymtm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2zycqyqmh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zhhgpigt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yaoorkeh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ikjpfzeh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2tsstnmep.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xgvvcucb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ubxgcwxj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jmecnzde.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2oemednzk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2izlugrid.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hyrbefye.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2bvwiluuv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ydesgnnp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2jwzbzkou.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2yfksbgrp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mtgfwmff.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2yllkvikv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2aiwxiesj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tbnmsyft.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2arocrmku.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nqtwjfyk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nyxohxrc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2twpdzzfs.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2juydaacu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yztlckrf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2slqgwfbw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2eruylcig.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2tlvvlrqg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kbjudzii.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2naqfpdle.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2puxdabzi.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jdjzbwgz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wnyvfjiq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dpfssiop.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2xllnidlr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsfpqufe.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vxhvbhqk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2wpkdpoas.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hnidvexx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hxemofsv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xeclkvuo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2usmbshjp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pjggpjjr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2myzlzfaj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2scjaubmv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2moaxlsll.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2tlbabmvb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2csrwcgwh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pemkeodj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bowmqwco.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cxdrbzqj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2bcosyuid.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2crericod.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bzscsnxh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ubdfnjha.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fommrqxc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2yfyweppt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xdgcoaeb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2megzjwpo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lrpxqtak.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2cxidrktp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ysppllrs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kbrvguiu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bahkalec.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2xoynnbgo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2oektzdai.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2htxxkkge.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tldbqpxl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kfmyzshf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xsjegqqb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2divhgysn.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrqoxavi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2vtarzmgz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ddvxtpee.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bokdcgyd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2clzfgqpm.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2euxgdynk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tcohemao.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2reyipnbm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vghetgin.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2lkouooko.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2najnmlco.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yebirnyx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lyhebxru.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2spyukaen.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gnvszqia.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2zyqrucur.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2tjzycmtz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ziwurmxh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2dwjwwrfc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gzeomodl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2icojymwx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ijzjxfnx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nsqqlrvv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qsisbedq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbfrrprn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dsfmolim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phrwvmbn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kekgiokr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ohrbcsqg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2uolkfnwv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2oljebfdl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zejsdslo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hsykgkxi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2bueiuowu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mgwvarrp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2yuwosqdz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2yjpcfhes.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kgowzcwj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mjaktxgx.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ffwkdpbn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2inzxzqjj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gbcxwwnr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2djvmjrcx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zcgkezxz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2roeufbtz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2piobwlxr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2dojreckp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2hekgfnxl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2yrjtxriq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2nrakmlrf.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovdpflrp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dxrirjts.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugcfeyhl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2dchkjogy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2blctwedz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2vinfcpbo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2omsafpkb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rbsvblgt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pdxnlpzo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2yeofnasu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ajbhbequ.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2noqsqjpu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2gfjgkagj.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wgrxdtys.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2hoimueko.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2nnbqdebu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2upgucsiu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2lmqkshpf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2edhesyqa.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2fllvoivw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gvrnwwpr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2cziqmqno.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2jgjvcdqy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2pszktiab.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gylvthuk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2npgqjqfp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2mzpruupr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2szdawvvb.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2mcqcagap.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2bhzgrsgn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kxvfhqqx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xylgzfdv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dcypwarm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2aqhfifas.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2fcdavhgu.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2oifghidl.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vsuxuuos.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pvifeifb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eapmmalk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fusujqcl.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2wysnkejv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nqwlvnny.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2bjlstmlv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2gegpynay.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2fnvskaox.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ffqyqbmz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fobetcdb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2basncsys.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2urygsbat.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bfsnndwn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2eptepknb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yjxptwsr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ghdfdepd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2fvruksjk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2gxdwrsfg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ezqkcmms.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2flvjqaiq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2guxaahef.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2eungslqk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2idmhkkyy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2afifwloa.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jzywzmeq.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2uykhghqh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xzasehee.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ebcnauqj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2grjopdio.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2jqwdnbmb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2bpulonsf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2iqndmprx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qmaaqums.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ddekqnzh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2dukldhtv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2huqkwije.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vskddude.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2exoorcwo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mrcovajm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ceijbqhj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2zpvmypuf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hgmtwrnh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tcltzmkm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jjxhmrxu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ooecwwzz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vyemdozl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qcnkofqa.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2pnjzoyci.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2hcptkgng.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gwdusrla.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2esbuhlcc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2gzxrggzx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2csaemghq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lsgmxrwl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2glvcxdoz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2mwabnefz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2vdymfulr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2uoubnwup.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xmnfvquu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2pgyybzjl.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rcbampae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khlzedxk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2qsxwfcbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sizzqxht.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xlczcqii.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ajpsylcw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2yafjwvvr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ihxwkkxp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2lmmuxdbu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hldkudfy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qbbxpfci.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2suzhhqwf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2dtvxmfzc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rqhjvmkg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ltaqozvu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2rphbqdeb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2kvcqizvu.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2acgdiwvc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2vootwxog.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mzbexqfy.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2vlxjufpi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2uzcgzcwi.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2nkeuhfty.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2dugumqbg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eadfobuy.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2smypykkf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2iyxcowjb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2lzqvwlsg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2xliuzmdo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ofjssjie.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2mvierlii.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wohausoa.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2aikgvzzg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2jjseqvxp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2dhayoqjm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2nzplbczb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qrkiwphx.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2bdtacpjk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2oxgvtwak.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2dfdbetdj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ksnmonsz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2lomjfrot.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fwpxwwzs.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2njbosngo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lkeorzlq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2kvkrqrkm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rtopnwwi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gercsdmf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tppimitg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2aiuvdfnv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2tvsrqncg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zzayaqqn.html


<!-- 参考信息 -->