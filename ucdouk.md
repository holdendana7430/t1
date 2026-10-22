代发 wailian999

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2edyqlmyb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ozuvtlfj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2lgvpqdlr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vuhvwjwn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2cmhqutrd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2mobusvtw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hxvviwiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejpesdyh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2igkkaimw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fepcahqo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cqwkhymi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2nborrzxz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2eyaltgaf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2rrfzwolj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xoaimrot.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2gpdgdsuq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vdjhuqro.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zpjhmrkw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ljitevcw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xtzhhuvs.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2icbadwqd.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ntzhtvtm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qrcxieoy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hatpywga.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2psirkevm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fncdvpmh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2hrfhsckq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2dyzaibyv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rwfsgavg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2asfvbslr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2stqaifqq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sbtghsvj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2cyssrffv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2agwgawwy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dkdsxana.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bzeczoqq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jdgwwjkm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2amyatobn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2tkqkeobq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2kkopqhld.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ksldpeac.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2kyvuiczd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ymgvvdjj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jownhkip.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cghkjfkl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zozsmmjc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ahdiedvk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2flwzfxzl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2vpswzewl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gajzvwbj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2itofeyye.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2qwhzmqiv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kyipaaij.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ubdcldzb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2nriubpdw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2umnfkixx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ynxohduu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2sqztixfg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zlofopbn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ngernohd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2djowcqav.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hwuwkqty.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dmbksnmd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mhaudpqu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2exatafyf.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2dbxfajdx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xnlbfgfd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fxywfsrr.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2tsrlieun.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ckcndclf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2rajshsuf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2clsvmxgd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2uuvvimdt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2maeshpbp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hzqxpeyk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bdswvrms.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vwgqwfbl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xscmflrx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xvultlhh.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2goaohjrk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2akbfhtqf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pfhsrdnw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2nerikmzz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hjwptbda.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2syaxapvu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hjyearqw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2xzjzsjea.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2evaphutk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wseeiejk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dbjlvmrd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vcatrqzf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2yzwexggj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2obdkbjyd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2hosvydpl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2gxcldmav.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2mltiflww.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2azjdsria.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2iwxxdevz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2paarnwxo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2lhquavhu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hglwvkuy.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wiqanjst.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ymcytqze.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcqkctvv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2dxsrxbyh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2iupzieyr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zletlajw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zrjkaleq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mxkmzzlq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfapfvpo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ekzpkpgw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rjbwkwyl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pcehihbn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rmyuisgc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mmyxnsko.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2njsdvtxm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mfddokah.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vcpeyvnh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fohdzuer.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2txeqmyew.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjgfpcwi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2ltufqgaq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xeagzcvw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nycfcwby.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nfnfckex.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mefgdjtf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2speluoqp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2fzhcdkkg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuheuszr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vtpynlud.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2zivihlxi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2foycdgsg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2ggwemhiv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2scjcenxb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wiuwxhhl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fwuhmovx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dmsvyfnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asdvfuuj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rlkqgrkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttepqmar.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gukvqfxg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2djiyblpr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2eotkuxdb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2umhzzcxc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2chwjcuyw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rtodfeuu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xaieywdx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2twpaupql.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zohovrmh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2coiltdqv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2irkkjggj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dqibzkus.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2govcsbsy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xszmyczo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tghiqqmv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gbjdkhcv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gpobpmyz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2sdoplrwr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wudfrrfo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ohzjudka.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2xpjejlxs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2sldbuewf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cnfhtbbz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ortlxaug.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2rwoxcwxg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tiljbzid.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mymojonk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zoyfwtcy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hlcsrxfd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2uiirrkqx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lhncgvsk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wbykvorp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2nwgglwos.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hqvqomvk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ciicrgze.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2wdxlgtom.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ohqnmhge.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qiwnhkqt.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2uqcovxue.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gzjvsmci.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vqggpgby.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2wisltwoc.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2yrgjitaq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jobhcfxz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2sjbjlhzh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bxxvzfhp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2nayiurwp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jnkyvfdb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ttqzwhth.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tgfgjnlj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2omixydbz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ciyayvro.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2eofrnqyj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xmnylqai.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vlhxuhal.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2zxaogrun.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xucvlpmv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lhlnxcfc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cjgwsxrt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2yrowfbyr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2izcqtqze.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wojzonss.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hzhegnrc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2wsgrzyji.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2knhxipsp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2xzmbjhuv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mmvnqkan.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rbnwjjaq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zpwrjvpf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2fanakumu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2trhsrqso.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2dslccvut.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2duyphubg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xsawmyhm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kemxsfyc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xozsmnjf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2crppnxji.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2nupetelq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2xufomsmi.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cdzzleiu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kdineoda.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2orzcuojm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2vooyeefw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2klsxluvd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hmqbiqeo.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2itwqldda.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ftauevzo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2dcylzgar.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2coqxvxmt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2swegbklb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vkhipple.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvgxzozn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ridmxhmc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2elofwccz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ejryukkw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2jlstbflz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2pjfsmdyj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oaeaqupe.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ovsdcexj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2otxbeigd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekqatvyv.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2udenybdb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iwbywaxz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2kgiorzcz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gzcmmisz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2toxodxlw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lnalpqsh.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2boigptqn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctiarppq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jdxgbfcz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2yzmmqivw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2mcujfhyf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jfyqqefr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sxiiprpx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ffrifepp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2didavwna.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hejczvjx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2esgqrxxb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ezlzelvn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qjskbvid.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2hllxopwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2najenqhq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rmkdvbke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjkzdreb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jifgonlv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2jflnniqr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ekakticd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vwiznavy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2tworqasd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2cdlsrzfe.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mqsegqht.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2rifsozck.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qovxbaup.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kkljyzko.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jpxupwgt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2kihjfokt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2achnzzss.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2sjpbzyxk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2fwchnpjv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2rizppezh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2opqipihw.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2cjnakktv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jbubwxvx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2puarahtl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2psjjxqvt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fxnvbowx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ciafdvgr.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tveidavv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2paxsatfp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2dribqnaa.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2mjhvabrp.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2pkcwbuxj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2tyvyepeq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2sqxsnxnm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2mublxmrb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pgajbjuw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2lwtcxyxt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2kpcezyvx.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2qaznymnj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qmybmxic.html


<!-- 参考信息 -->