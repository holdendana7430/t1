代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vwoiokie.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hurfnbrx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2duvdevvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlvowgia.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2iewhxcse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wntoevnt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pdfdfblf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hbblttjq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2onslxxva.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dptfocwy.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rmbkphoo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hjyjnncn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2uvxbyfec.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ahqthxsr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2emjwhhpk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pwkngawl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kefahier.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zblmzkjq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2dbzlbpdk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2amqpzstp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ytbjjumg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2kxdbtmig.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tpgewhyk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2pqbsrdnf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ndjylxpo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ijhebvfh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zighicfj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hwtndzgt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vxpgfzem.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2dnjomqmz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bccbbvgf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2epiybyzo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lwcztfen.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ftcllkkt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ykomuopd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ctmxqosr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2oanoikae.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2lanrawhq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2xaihqdbm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jpzgwknj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2exlmtkcr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ogiqioad.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2tgpzehgi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rdbuvjqo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2piexdsrc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2tgemsnjc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2drnhvebj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2exmmbvrj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2abthvbme.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zuoneokq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2sjbnagto.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ewkrjicz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qqtpjtev.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ybuekevt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xhxfwzzn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jynlbocg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2qxdlhinl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kximrbct.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ksucmfye.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2vpuwfttk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dtccinjw.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2cgvkopop.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2enkjoydh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2vonpyxzp.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qcyhyalh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ccqyetnt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fjwchegh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rwmglcdn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vshdknpg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ctgxvkjh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2mbxtxzcx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gfjowlso.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2bakghxza.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2meswkyte.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hkvvhloq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hmcjcrjm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2sqsxjezy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gkudpyyg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hmawdldo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lcewxarj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2xnkymkak.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2huhrvglq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2tcwcijed.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ymmknymc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2swvzwhhb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xiiuagdn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2fkwlbzzk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mwobqxdv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2nftthowf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2drrcuqbd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rtffpcgf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2piwkadsm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2lkjlyyis.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zoyohgld.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2thaxqtnb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hzrpxvhn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ewjhfmlc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qjoadgwc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ljgmycrr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2yefvdhhg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ufodhjsx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gunuzmhw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pmwrjora.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2berwgqqe.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fpascery.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlqoypjb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2edlcdomy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wffefdqc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2wbpvjbwo.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivuqjbfp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2upeydqqv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xvucvunq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cwfpcvmr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2khgeauyz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2hwhrfazw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mlivvwzg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2izwpcanq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xxkjewjm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mgiofcik.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2utacrivs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2dmzmhgba.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2efmswxia.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lktmsfpo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vlffwjnt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwekycfo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2tckkktuz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bsmvmkcl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cvlcurbu.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2eavvewhr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2bxvydleb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ipvemzrh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ugtwlnnc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ifazjsje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihzmyawk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xwvfrvxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyvjtxdi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dmzmpvra.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vvwzelok.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jouwthvo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2hlykkzjj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hfgblxpg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2iweefoxc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ecbopgms.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2vrrujsia.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2yjhkxbra.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fjfoiuog.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ruqezbmc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kzsqcmbu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pgpgkplq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2habpulvr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2rxjhtyqn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wsfrdkwh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ialwetix.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dwvdizuz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gjosnstz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2tnaqfsqm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ddmssaft.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2vnvlcvgc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tawbxhww.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rszjeumo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2vpnvxuuk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnausxum.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2bzatpeap.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vpyxgdug.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jhsyddaa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2flpwbdaf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ovovvhyz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zghdbxsk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2xevozzxy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2weirrife.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2caqatzsj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2bajuqeyu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ozdscsbh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2didfokxp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fovvqzuv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ppiigooi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2krtlccci.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ydmgjvei.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2dnxjejut.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2tlpftwlv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uoojsgrk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nzaddpmm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2glciojgb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2emoodvao.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2fwhkwzgh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2nwcbnjuo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bhpfbmdq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2riykjvfb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pocbammd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ybmmlqoi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2lklzxeok.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2pslfieqw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2snaihtjq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2kglncouw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jttuongd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2zdgoctry.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2inchoccp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ijyjyhnn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bhhbtswt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zvqhvpeb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2yhsvojlz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2hxblxmro.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2kuhxdpvt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2yijocwwn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2panvkjkq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lhukopeg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2tszwknnk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2muittzpz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2eqdxhpdy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2crgxicki.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2efbpfnqd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jptttnwh.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ddoanbzc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rfuqgmfn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gitdhjbq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hsyufteu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xxetokkx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qdrbqani.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2qmdosotm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2psffhwbx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ktxrvsvn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mucalhun.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xkethwmv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbvvizte.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uutwhggq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfaurlao.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2tgxqroer.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrsnmnce.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ykaivvdz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2utmjxgkk.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rgndathr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2miukqzey.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2edsngsqv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrmzgnlh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cssbxdjr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2tcouoodq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qizwlssy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rffteylq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fuohhzwz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2asijbdhh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jwgnjpbs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xbqyywxk.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mttaiqiw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jmahhqyu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tkfstpxh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gexnhkbw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2mqpylgba.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dhvoeyvo.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gpeghxjt.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hajtpnah.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wtbtnhtw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tpysybei.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2rquwyksr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2ircmxiwo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pxptmmac.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2osboqgdy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2mmgieqyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idauhqzv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fccfhnin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpghanzp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mhnfmtlq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2hmttgqts.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2vaomgfad.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2amelqkcw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2sfsxqjzt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2tpkklmfu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2qkqzpsju.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oviczepq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2elgqcmaz.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jujdilbf.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2nykwusah.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2cmtcapfy.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2mkkppvux.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2biqyfcbv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ekdllvcn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2twwdccco.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2veruheqz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2liefzjfj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ramysncd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2thucyhdl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ndoblzmb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2mmqwueaz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2jmzyhxvs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aaavuozv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gswypstc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ubmvrizr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jefijony.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bbyejdqi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qzygxeek.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2pqlgrdiy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2akbfjidm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2xhcwxzcm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ukvpznpk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2jewmpfft.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vohvfaky.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jsggbcjc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bwmqcaxk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwjdgthf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2vvodkppr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zxiinllj.html


<!-- 参考信息 -->