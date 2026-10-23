代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3eoofhnzi.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rcnswilc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xqoplgao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3foqkvpsu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rqqhiplh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wynfwqtu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3knrdxlfp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vvasiaez.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpjhmzbl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3krvdavyi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fegmzfwc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tbhvtllb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3gshoiett.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3nqyupkyq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3dznwnpxk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pjvuiznw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gkltyhxb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nfxmwzjn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nuywfhnc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mcrwhezb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lotnfocn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qhmkjgfl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tetbdtig.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jgygmqxf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ntxikwrh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3fesecfbq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qtdmhlcl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eenazebo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ahattdcn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3tabmsqtd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lqokrxvt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lodcvjna.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ossluglf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qggqpuku.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rnovagsc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ddocvwta.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3nyfwrbhm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tvvdehgp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3nzmdhvjm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cohxnicm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3blxuxdtl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eygelgat.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zezdvpxk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dawbuybe.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vktkeyrp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3oyuwqsst.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3omfihwsc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gbyetcwv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dhwmtjcl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nownlhge.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ahchpwlx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ryyzuurf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3nduvuldm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vrwgexam.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vlvuoltl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lgxgmmbz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3eyclrhse.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rrsnyjjk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3yiwlopbo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3knnmjvgc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3frxdglim.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3afhvajou.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3itqrawls.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3dorofmgo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cgzlcace.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jsjsjfzb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vnwjurjs.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3lgwopvjs.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3iuczqtqr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qfmkonba.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mopxmgpn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3irukesca.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3slgsyfah.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3vqxdndod.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dbqylhvw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3durnzzcc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3uhhnageh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xpyogmpi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tpdtjhek.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pktntbsg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vcykqtta.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uglseadn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3artklong.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hpywfhuc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3zfuljsui.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3jkhrrnbm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vtredbbq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oprgvbtn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ltdaiymj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3llphafhe.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tbceckfp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3uwakaydo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3svsuafoc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rtcnsgoj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ofagngxp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3smnkwqev.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3egxfjcsz.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kraihchu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3kuvbupvz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ylxaqtlv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mvzfggyr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ycxamngr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3eqjqjsga.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jjdfylqw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lefyfzec.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zumgnxsn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xbuviier.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hfwlcxom.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3uapldefb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xlzudtpv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tjzeogzh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3cdvxdwwk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rrdrghcs.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3snbltaxw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ubygiarv.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bnzltuth.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3smeuydic.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qcofhsal.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kptllznh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jqzmkopa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3imooeinw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mfzqbggb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vsoowfae.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3dfyxybla.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrtykhdc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3oezdstsu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jzzusees.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3isztdfmq.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3thvdvthp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fonhdgbr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3kdogsspg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mfmfpvdn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ebmjtaer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3poclcoiv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3nfomzytk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsdfxfee.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uhdgyyci.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wfyoudlm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3chfuttbp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hixcnukf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3qblkvifh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hcqvrpml.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3cgzcqziq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3hzbunzjq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3kidhxzov.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3paacjxii.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3czhfjove.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zfooowvh.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3toemefdq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vadpyndw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zyedtexj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ztftowcf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3gzbkxzho.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3cjlcwjky.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zwkxnmgr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wnbvcpzo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3yitzbniu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3rppqbgql.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3uzepjsuu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vlyhqxio.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fjjdmuwh.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rxglkrba.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lhskqitp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3eflwpjjh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jcvnjrva.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3uhemhxqk.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rvqrdvwk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fmghofoy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3abnfgsig.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ppuxzaok.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dmfshsyx.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3otzyfuyd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ameuzled.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3qrbgbmfz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3revxfwlo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3szckwjds.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3vhwmkell.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3hqyknmga.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3yfnxedqc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3miivbsnz.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xwluihjx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3jzgrogdl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gqbtqnem.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vqvqybbk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3heskcbcp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3dxlqezko.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ztxakvtm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3dzrjoxkw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rvoetevn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3lpwrcofw.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3egjcbcvn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3adyztwer.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3duuoapaj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3uxpfcpkw.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nghpaibk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3cjqabxey.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gtrrgmyb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kblmauwf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3krkhkxfz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bpztfkos.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fdhtbutm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wygbplnu.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xpilvgzx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3aqhgfaiq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3kvgponcq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bbllemcy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3exuzaqik.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3wybytfgb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fkzggioc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3geoegpbt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ldkhgmxw.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3lmhhumcv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uftkiuok.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3mpcbrjzu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3tdwqwiwp.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3xdbpubji.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tijhdtrq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3sktqkwob.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vmdgqitg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fmnsucmi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3juvbmamf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3teffjhdt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3segnvtam.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlqbwovy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zvoixfql.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdyizzdp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3bnggsfhe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3vswlucxx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ocswyoin.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrxopofw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3mzgibedd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3umzlmycf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iqwkbxfm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zevfwggx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3iwwlgzdf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3yttyskie.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wstghtvf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wetgqqck.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tfyrzufd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cblhivhi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3pdyoxpbu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3obzibdbk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ukdiobzm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tumhdkpw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qlqsikvu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mysmetgq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3lqgkdkon.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3kdfhedij.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dpmanlyg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ljkfbbqr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ihyggfzs.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mtrsqqmy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3uzxrevkv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zbnlychy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tjxdomxr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3csjmcetg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3edhruhiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3davbfaem.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3weiwttoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzmgigib.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3vuksauyl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3orqkaleq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3uqslwowp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tctnqwlk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xeroctcs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3eudqndnm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ydwonkpb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3agscrxnc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3clgonabi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hiiffgmv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qhrgrzba.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vsmnhexp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wcfqhlzl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3cbycbrtq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3pdmgpzqw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ubpqgtkl.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3gfaizwhz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3xjtojaun.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3cplvqecy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wtwkogrb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3exotynfj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mviecltl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dysgvbib.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yeerrvvs.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3gdeemeks.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3vhaqjnee.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wxvpdprd.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qwqlqitw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3gmpzltiw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3dfwebkax.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3rtieztkp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3uwwuyotf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3szphvktg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3stakqncu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3byjunpce.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3oseybcps.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3dndcpfpb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3eunvkgfz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3jvjlvttf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wqdrlvif.html


<!-- 参考信息 -->