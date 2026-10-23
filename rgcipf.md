代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vmpegxki.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qeyabzqa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nicvkovh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3eexgsdxp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ogmvbmkg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ngucgskw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jsdqxrka.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qkbpdxgy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3sifkawnr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vfdpztvx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3gvomlanv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flgmywso.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3metbojfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sijvcrmn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nabzdmjz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vpmojqzl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjgzrerg.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dydckriw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xxjnxjif.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ovdkzvmo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3usjyfgqp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bjodadzy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mbbwzwye.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jwfceafy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3flbycuho.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wxxhcpke.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ltzjiltn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ijzgreru.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3jgyevuqb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3crnjqtle.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3orzehkiy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3jdcujyat.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hzlpizal.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ilwzfzko.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pykbrnyf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nhngehmu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3gwwviuce.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3yejotrhi.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bifhxzdq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iyljrcgj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nyickbvm.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3tjwwjvfy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3qkdkuqvj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hpdjgwru.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3brvyqvdz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3bjqfpaqg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3exzrnxyd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3krezruqv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3myqiyfgy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qfvbvnsn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vwjgjvcb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3okhcpcba.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rvjmtmvq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3taryvmyt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qkoavccq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dqhynvlj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3osgqtaom.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vrawgpbs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tvegbajj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rqyghzau.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3avvzltws.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3etpiagcf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3csefsvwy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vfjsijeq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3jwqigwgo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uirtcfwj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3yaocsybs.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3lagcimbp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3qeflcodm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ocmydakl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ixgbatbl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ftovzqjl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3siirdgoa.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3knudkgrv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mrbtyvuo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vzvyzzry.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ptwmlzgn.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ybqwciyk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zgccnikk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iwwimmto.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3btbmwhtj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jorwkere.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3wamzwlsm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3muuwjuoi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3idgksjig.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qkdvvsns.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3tcsdwwxj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssnffilt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ausoscyo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ovkrxbvi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ngzthfvk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rncwozqt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tndzpfap.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3bwtgsjtb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mwutrtau.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3thcmyijg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mginrcqq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3peouzsag.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rjxmocgy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3gbeltogf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dadgsgdr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3apeftqim.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jnayosay.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ynmbzjxc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rusiplzv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kvchmxzq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3zitbmifq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ucxujhtv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3kresmqau.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rypqjjag.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ootfnyqy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngcuqkug.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3gibnuhmf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbdbywcv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3szfjnwnm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3hzowhxpj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fyatewjx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qrcewxme.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xbnwenbe.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3xnzoekfm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3udxhxjxy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dpveblgi.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3pzumykmn.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3boregsch.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3lidfedcz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3eepdifnn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3vlnurmcl.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fqogccml.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yrfywclb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3akqtqhqe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3flrmmjvj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zyltndoo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnurjlsv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vfedyvtc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qwfnpksi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3yynihqgt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3dxyxyblq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lwlmqtep.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3idiuzgyu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cljmgrtp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ohbbrdhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3geovozta.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zkfcaclw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crktoxrm.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mnokysgw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3smqihplt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwinnhba.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3cpporikn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xdbniexj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dzxsxurl.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3mneinlfv.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vdguhnnc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lhgxhtbt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3gndwvyfp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vfbqugru.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bafrmmvn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ujipgfwl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mexnmbjn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fagzfiou.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mmpllhju.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3nnwjmyfm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3mefqkoah.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kszgibgo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zhbbqpte.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3eyaipwre.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3sfcmmzuu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3twejbjvg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hkesetyz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nehpiuyy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3uksroozc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xnrathwg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vzattmqe.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ctdobmut.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ithhtsuo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kdfslkav.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bpdmtnhw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jdfdakpn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3zhnrhiph.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dolbjvft.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3izdgmcww.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3skcexkxn.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hjuezhwl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zcbegtfj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dtyowhav.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zqzsyugo.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3sxuharrx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3srjurdne.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3egxfrbmu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmfkpawm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3cvxsxlih.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3usixipyc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvpcisjy.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jopygegp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3gmtpjnbd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nitgippj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zidicose.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oakvifzo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3lhnxljqo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3yoagqvfy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3sdcejexq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oqcaeaia.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3cbpixrko.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kebbqeul.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3cbrsckas.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dxogrxdt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ijszkaxv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3mozujrsi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjljfxdn.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dbovuqup.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3llhwmnit.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3yywdiuon.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3rwqcsoyr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3afkwxvlx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xjuucnfs.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rekaeofl.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zyaalxgi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rboelzru.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3uiirvyhc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kazfgpww.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rceobobt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vekkhcsg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vwakzpsq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3fsvnfeji.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gnihykwj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ztfqnlfj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vqspmufb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gfxvntwu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3zgcnuoyl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lqohuyvz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lolyiyjc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lmdvoccs.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3sqrdrhge.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mhoafcvm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3slbjaksh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kxolqcaq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvmmbfae.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3mcdannkb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovtnadtq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3muywyrso.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3phgamymr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3kwodqvyn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tcvqjvwt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wuhwvpdd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3tnpitvgp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3myolxwcu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3itwxzhol.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eyhegveu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3egtdckik.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3rhpmnqml.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sxequygb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3phsjrqob.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nvhcpfps.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ybwuavnc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dhxqemfs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rnnbrmzh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3tbgvczbz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3atwqqbnm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mjepecse.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kxoxwrak.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3lvhwuqtc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ivpvomtz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yonpmwsz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wjfrkwxr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dgcqstua.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3egajhkqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqlzndqp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ycvzlrdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gflhgifk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3cmryrkcw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3icokbxxl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3kwimsnbm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vzkckpuy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xqdrzvac.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3tdnjyfpk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3wksjzqqk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vigixkam.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ltdwzbdr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oxdwvfbo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3xjdxkkaa.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3rrsywtfe.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3serfprvv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nusfdhgs.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3eiuvboyv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zxjssgml.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3xxalqmoy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xvtnqekv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3flqgqavt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3iahwfqpq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ivnzsaax.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ngkmbwde.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uaxpapay.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3tywdljar.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3cgtxtcmj.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3aqrrlrji.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3inupqzuo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ckazvihz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3gywguggr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3qvvqncnk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3eckjjfpv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3mladullt.html


<!-- 参考信息 -->