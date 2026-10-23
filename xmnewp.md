代发 wailian999

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3eappfsin.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3cywifttm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3tzqhizhg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ifyvjkyv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jsqyqsxp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ubipldov.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3pyyrstlc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3uxatoyyo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zilkcyzc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3gahijuuw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3yetooxev.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lilupklp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mtzgmnne.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3jyzcctyk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gvcuujrs.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xzbmcnlu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3zdxglafu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3fwpioitx.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bzppdaku.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwpiwpxq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vkjitfry.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wqgbyhuf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3qzcsqyri.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qeatitjm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ytsbwiof.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uhaeetll.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ivnbtpsp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3abiraedt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dgbnhggy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hpgvzxsy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3syogpnsi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tllmcduo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vqpfryan.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3uxkhbhee.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lpacadmh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zimfczzn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qqocmatu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3tevmjtor.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3reqgyfct.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zuozklid.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jpyfvezc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ivbzursx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3svjhixiu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3icxnqmid.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3huvcuanf.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3vzxuubbw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3krlknsid.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3bwllratp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vtyymkdh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ztaufggj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ssiwehbt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tbagocuy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pcxesykc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3noagpcpk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3avdqcbjc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3faxqyzrc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3iphnofcz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qxgvasst.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hshcvxus.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3coplyvxv.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ojcyrymh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3rdjjplya.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3voajepby.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bgfhkurl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3atioqjkl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bqppxrcq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3oxevqolx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gswnfgty.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jfdsfcib.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eldvmpeq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3yozpfsga.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aycbsdgn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3aptuoobp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3nixjrrtz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wzgnnhhz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uveeffoi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3wcfdsstb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3holwnxdj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3uqbxgjxf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3lfaabqxd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjbilvxz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3smomrtyq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3pcwtkslf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3oqsjbvpv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3mrzukvwf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3oekrdabm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jxarpiel.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3fqukyvjl.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xinvlweg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3pofcogha.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jhwhkftq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qahsrygt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ssorfyum.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3yobczwju.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cwfadqrv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3qktlrrup.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3utmrgajs.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hdhltsxy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tucolfdf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3pgqgqaqr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xarzebsj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ugoxumnz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3koorcsuq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3lfdzbkut.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3pwkhnecy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3blrwjueq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3umeemazx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fssluypp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3mmwglqnf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mllgfiao.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qgqmnycg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3wlrdgobo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ypszdpeq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3flqzyzrv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vtgxbkof.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3osvixsie.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3vugwmfca.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xvzcokco.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3euhbxtqz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3yzksptke.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vcwypbeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddwmckur.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3prxwbexl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tojthufl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kqmmmntv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zczzjgdr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3aixiemww.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3mexycngi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vcgmktyq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3emtrcqwa.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3imjyzvfw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jqlqdkmm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fpjywxap.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3upccvmdu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hurveuvp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vxdoiwxw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ypsmlxto.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3acdrousc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fbsdfgke.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qwktxslq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3wskqlvjb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mehglhfw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lzbfpeyr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3jvbxlmdl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3odfizlqa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3jaumozdc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ndnjujsz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3csrrmgod.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jjsvvrbv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ooshkmla.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mpsqgmgh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3czmricmq.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3typbsacz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qwmvlhxz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lveocwax.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kxrkyjyh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3eojoqhay.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3opmemvov.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ehdwldrt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3sypnfwhh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3iwozulhe.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3yyyvigkr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3kppzqkaw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kvcyzbjs.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xjyzwnyw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zkcladks.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fskinfgw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jadzchyg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nmuvknbz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lntnrmjr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3omucmdxu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uomaeorx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jwughubz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jynfennf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3bonpobuz.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rlmivmav.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3nldfpllu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ghshbykq.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3futcrwro.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gwfjeevm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3syafwkrd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wnqqrgjn.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hweytzan.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3vtahrxiu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dvgtjulm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3optzftlo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3nldjprvm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3aivbotww.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3dpjiuujx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ukarfkwp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3iumdpwzg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3lghchzer.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kszgmhuo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zufxyxwr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3gxoqmbys.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dvfvkjed.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vrfdajvc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jfwreylp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3wtnbqeag.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zalianim.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yuoqxxls.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3symnuojp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3kvfbqigk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3cbqmtcie.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mcgsjfrm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3dnyylpyg.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wuboznoo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qruddvtf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zkodmieg.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3jtnsyynq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3vvtgynze.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3pflkiska.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3nlqtrofu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3dnmukshc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3smseusnk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3udmezlsf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3fwxrbaow.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wasenzpg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3irvxpwqk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3fmghwfyy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3sbcjilen.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xjlhofhd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xgcxodcu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dhrsncnt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3gtjjybuu.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qamwkxyi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bvgjmzsn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hocilzup.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jgedisup.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ktokwyvn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lvwrzkee.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lfqvknyb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vhdlapin.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mwrndbfi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ylgabuvc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3muaoxcui.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eavbrsxy.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nivhzyod.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dsaxoizx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3jorqujkk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qamamiit.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hjyfaqjm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3enjprstz.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ipuqmjis.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3cbkfkmhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knbpfcuo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3klihawqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odkwxjcb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3bwbzyxrw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3dubtbkjw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vvlhrlgp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mwtilyho.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3cvhbasjb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3lbslcvam.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3dmbmgwuk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3tpmhhphb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fqshbmox.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gybieshy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ckesfbje.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3xaewahno.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3kvxryclh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ypkpsjcz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bkvtsfhu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jopmkzyn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3raegrqmw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3bndutzlf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3cyuvvehx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3czwfiqjh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jvhmtzkb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ibgljboz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3xcpkclft.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ocjtoelj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3yolztgii.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ulinrslx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wshxahmb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3qdsqojof.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pbewwykx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3xcsiehgj.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3fvntvrwh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3neghcgmh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3bbdhbkqs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3wghdyvyu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3lrprwaar.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3tqmpkmci.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jopwgjcy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ehtliojc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3yykvxgru.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3fjrvizev.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3smxpqajo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hgrxzulr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ukhimdbl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3tumelkhm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jkpwezyd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3iuhqfprt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3daldwvwp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3egmlhpcm.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3undirouy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3yujzndrp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3isdnnzrr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3uskaqhku.html


<!-- 参考信息 -->