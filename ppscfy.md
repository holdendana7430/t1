代发 wailian999

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zarizzuy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2oqhajzja.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jmosngdc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mevezpoq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2uhvdwvin.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2swkhohyj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2fywkknch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oimqibgc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uesvhwwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acukdkfy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uwfxdxen.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2wonfytln.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptzgqqep.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ejkajdci.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ejowkxdx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2rnffhbeu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2teskotmt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2agkvtciw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2wqipkohl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2owizlmgk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2glfxhswg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2licmlfyy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xswjqkhf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2leubwent.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lovrjprl.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qexauhod.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qxduzkmr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fldkqivb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zhtfdddx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bnnholox.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ixsmylsb.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kcmgcfxo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vziamzok.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gkwwcjxx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uzlfhosk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2eqolxipo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ktbsdmkz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gbvlzzli.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2bnxvdctm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nzivfqof.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2hdlnaseh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fkazotra.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hrjzsesx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2amhidssv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iiiauqzv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2reitnnbt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vvqunzhe.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gbniiiay.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2sfgctydc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lqerokxx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tgmbrvpv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vkvdvjxf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ogxrsznl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mbgitqyt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mbgdotgk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fnjaylpp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dcgxrerb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ysqfijse.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qyefsznt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2fydhnimu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2gzxxgfwo.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rsaydgdl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wccnsexb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2frnebgbu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rhxpzakm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wychmfgv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2odpyyvqt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2yoyccalh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fpflfnar.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2rdmlpvnw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2cwjiglwa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ledqniyz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jxftkpqk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2yxweguof.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2cgrevzet.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dxpricjf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2iffkczmu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2spjzpdfo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ccpgxntc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ebpodmto.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2bgdvwusm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wdbupdis.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xluoewey.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2rkiywfbg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2yqsykifn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dyciacbn.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xnmuhmpi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ipwmcqpz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rejdnpao.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sneaedcq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2cbuhvlyu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2acdfvdej.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2gdsjdigh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2stipymjy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ajhlnqdg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ouenhwow.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukjaroyj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2tussnafw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2cgphdxza.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2swzisdwl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jrfjdgfd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xymjshht.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jkoncszz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dkeidutm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ivranhbd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2awuirlnb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2anhmoojt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2veplqrmm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qjwbhqgt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuzijfdm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jdxrwpco.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2swrpoirv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2hqijbzjz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2samzicbu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2llfcaxvu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ryvudime.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2khkuzhrx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2udrjrjsx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2oqylmiwu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ugxnaxbl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2szfkjjtf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2shtymuqt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2shwjnukf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2onvutbca.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2nhvkdxvt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2nvgybwgn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dsxuszhi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fcftegkn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfywjkie.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hkknnqyy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2txokdumw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xsdlprhf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qvwsnnax.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mnsjakqw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rfvazxoa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2oiqydmwp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2orvzfkxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egxizruc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jykajukm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqszxpgm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xvczbljx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2anmlvowt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ppmcuupl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2dvtjefuy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2zoahjtje.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mzgqeacp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2oyrylrvf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hyxnuknk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ozzbuanc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jhfbtemn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2cekanwvz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tobqorfi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hjhjsybg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2obetbenu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hobqonch.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2aphnphsd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfvcfpng.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mhrgwgby.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2oeiuyrgc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yibdoyqw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2kadrlvxs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2cqcmumoe.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cgdnjfaj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qqakpvpb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ylfssbqn.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zaypoevx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vqgfjxbe.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2olnfqyev.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qxswyjdx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qiybvqzn.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aepgibuw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yogaqyij.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rosejxbh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rgopuzdm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hqeonxhn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2fpwcvwsl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2fpaismdw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2mxbihzdb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2izgthgbr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tyuadrfz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zuvlgdgd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kmryvuef.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2bhfjhypd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2uuwcjmal.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vmbxyuzj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bflcxvvm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kexkhiss.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qtdwwtll.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ecgvsrbi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qywqkexw.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2aspqdnuq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2cekpnxxw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wnreosct.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2gjgnxurc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xcwcobez.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ntgorclq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rwsslftt.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lzanqitm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2steikymn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vwpadilg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wjtffeph.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kmajykyj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2dovcvtqv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2laduregc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uldnndhm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2uwigowzp.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qbotyhag.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2mbiciyxn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2epeyuiwk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2jzbcxsdw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2yduzszjs.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2atbwuqvi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fuoqcwhv.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2fehqjhxe.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2xxdpnivc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2lebrpeqd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ghvpfqbn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lnsbytqv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2dkqszdmh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2tkfoagef.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qcmpjami.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2imiifggt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2uoyypcgc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nwtmpjxi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ksiheyhm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lwclmstr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pglokqib.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2snrjgple.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mtintdqx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2butcpdzo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qgtszmwe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2epnrebek.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zpifaxtm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2iupfdcfj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ivyuivxf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2yoflzuum.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hgktsrzr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wyxiqvsw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwghxfhd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ywantizq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2siyryoil.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xsfwxqrd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nxgnwuzc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pbrzsbxh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jfenswvs.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tgmekfpz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jagfvtew.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vfgscycy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2rcnlkgat.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nilxpugl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2hpjdcqbb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2qmdwlbrw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2oypnxxua.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2cnsrgggl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2suyavkpn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2fynbqplq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sklutbvo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ghexzcor.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tguxyenh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2opskurze.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2efngtqhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjxjncvm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2swyxvqkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwclxczb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2sdwgdddq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2kdmfxxrd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2rgqnyqhu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vwwonxcn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2kfprmnwc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2nndzywno.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vugwlruc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2suoqjxfy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2dejpomca.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kdpqmngl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2nkyyezaa.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2znhgzqla.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kialjcqz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ryyctats.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mdvkzuwq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2onwntdjq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2giqrbxzt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kumszzia.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2fcgyutka.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lianaxug.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2losjwncb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2afntxcgj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2dwhtassg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2iyulvtlw.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2pbqfpjgh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2orjqvqui.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2anmwbjjq.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2uyuqzzfr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2eitpxrbn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2jfhowyak.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2sdskgegf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2lsmsxuhy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2wakxmrav.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vnwiuehd.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2schbsfsk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2myynafba.html


<!-- 参考信息 -->