代发 wailian999

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2cmhzpkfk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2rpkkhayo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2atticxjm.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lwbchcgx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2kfbgdljl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2rkltncmm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ulduersp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgtcszbz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ldspsagi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axdryvsg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oxrdyxog.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2fbrnlgka.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2uabjqoqg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2uowrlokn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2jsmrkdoa.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hpvimpjg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2muzieqpb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2isisnpxu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xktewvck.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wprlupuy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iawxxgon.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vrjjolpz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2koudyzjf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mxkdmbyw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2tzlabvmd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2vfwyzeei.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xsmvadlh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2snjwyuzy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nhumoely.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2wouuekkl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2clneblwg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uizjcuor.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ucdhhsxr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kjuhoecb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2klilmiut.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2rmxffgqi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tlisbfor.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tzcckepz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2cdyzbogr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jpidqfiu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2sezyddri.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gsdfytns.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mheslpnk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ferjzhxo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2tstsdsjy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2swrduhoz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2uukzpuqm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vwqjwhrj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vkqtnajh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2osmjoehl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jhfnmdrt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ehqfwhrz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pxegatoj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2uxvvggzd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2znzbnqre.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gvkixgle.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2habolyaz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mfyiybuq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nhwmfivw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vxtjtaov.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2uyvqtumq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ujngizau.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2caajxfoa.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kdphvtmr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2urllrfuj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2latyxvot.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sdizbldy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2hmxczupz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zeupaith.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tsvoewgd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2bjccckwc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lwzcgkog.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ssmbuzfz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qvvasond.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ownzhjdd.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2drofnaxy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2tgidqmkw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvztvomz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2urzuturf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2nydcgyxd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ptifdqxi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2jtovduhx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2pcolbdpt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lxdtdrnm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2skzgwokq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jhsbxbvs.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lzsgvigp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pwodbetq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2cvjmgwso.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fjglozvj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lukwgdyf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xrypmvqg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cpmaetix.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2scoglnqn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2nmazgrfh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yuzxdngm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2prjqbpvv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xaikpiek.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2wydyeshs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2apwxlcom.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hracgbkn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2bfbffqco.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2toamizbl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wujvordn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2wqmvtavt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ucemcehi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2vqpkqzny.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2cmwwxaia.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uwlsoqse.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwmyljfh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qxcoshrr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2gdydtqhq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2btaeefkh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2eazecspj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hmzxalom.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bdddjdpj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oxkruron.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ydgrwpju.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2pdxszxnm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2owulcgfy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jualrwvi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jyiaeban.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ddwmobzt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kalapcvc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2phaozfnt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fndprvaq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2uqrjxxwo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vhqdxkpd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2pxxdoplc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2qmcywwei.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zmqbczdw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2twcbgemt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2otbyartf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2sjmptvwj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mdfuqndx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lpfspdhi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2amxxxxjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prossnsx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2iamhatca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwnnljsw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ednnoket.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xtgbgrjr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vjitqwei.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2cigmsrxr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kdvgfrtp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2barlpwhq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zhngqniu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zqfipkgb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jxgwpslm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2zgyuzhmm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2lvwksqcb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hjotcijo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2alczsflj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2uzgbydaq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2thonizuo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ocjjmfjg.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2trhreiqy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hmqjkghu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jdrjqnbi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ozbqxqzb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2oifzlayy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2wpqmszej.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qwkfivmw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lgnylcub.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ojjvwamu.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rlixmmik.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qvuygmsv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kvvtowhc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kwtjvzkg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ojsopjzy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ukvgbghl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ansajfuw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ojndakvi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sufjsnrd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oxlbmwmx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2acqwfuid.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2kiqkwugz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2cvgfyvre.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2gpmcazec.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2kqhjjzpw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dtiurfxa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2johansbj.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2akkxukdi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ehvzthrv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2dycnhvjn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vvgoalif.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2uajzauuw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cqvqzzjr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2uuemeaja.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2dguqokxz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vfrdtvzp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2zeaquepd.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ifnmdebo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2leayggle.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2afoqdcqw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2yguzyxcg.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fmfqxmzm.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2szlquktk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ktverosp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qyerswzw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2finsqjoh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gtohiimi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qeptlpyh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wrdmvefe.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2snagkkxt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2yoihqrnh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vljyurqa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2krgjfdry.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2uggnvghb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2irhubzko.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jbtbjggq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ufthlsza.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2wdmcavds.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hdbeqsrt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2zvecoqok.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2bcleaadz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xddlorqz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bzqyjuym.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2iknlqsrs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hqxwworu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ruafslkp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2msyeyiry.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2wdbybqqq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fnzphpds.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2esxucywl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2rljozlrp.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ivrjuigw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmvrzhrf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2bwivcgyr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2botypkpa.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2dwsjigkp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2joaptepa.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ummpzhfb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bebxowwq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2irocxatp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ckuyhehd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2hdcbdbep.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxirhyce.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ujpyxvwu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2fqepatwi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhcruoyx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2isxweoki.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qvukrhdb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvihcudy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2urdqprzx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mseifhxc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ohrraoof.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2suoeiaeh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2attadskq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ckmumdws.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zppruamm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xiyoxohc.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jpbgewgl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vpqrajhz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wyzajvtq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2amoymxff.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rxckwrpq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hinmvwrk.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ausunedc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2wubwcqpe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2rbezjuox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjfaxjez.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ewyorcvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmvdgomc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rxwpaxvz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2hemcehst.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bsjnbqvk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2izbihkva.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2trfwuexx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gjkilyfl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2diqabevm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ncceuhkp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2oiadhiwx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ltmhrzuq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dsttoalf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2eofidnyu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2hmegkdwg.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2rdrocbtj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2tfwkkyfa.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2zhqssugr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2dmtwzgkl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ayyitejr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2dvrlzfbj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2eyvaubem.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2gyxsnzmu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2wmrqzdjg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2pppdgacd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2dtfcdigq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2cchfajjo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2uaaidocc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xpuihxuw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fpeteowv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sudkbypq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2jvzrlbnc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2ecwgctzm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2iawdylat.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pzxkopyh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ruvlhtki.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mzbjqion.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nzgkgere.html


<!-- 参考信息 -->