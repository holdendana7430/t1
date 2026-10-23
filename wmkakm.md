代发 wailian999

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3rgqeshlu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sypedukc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3rpscvdhc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3satsblni.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3zqjvfpvt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zhpywahr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3gklqlnhw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jeuirlwp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3tplfdzxp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3uudvwbci.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ecyzrpbn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gjpbzpjd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3reccodfo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fwnuwnbk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ydhmqjjm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3cdbzilxp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3smgqtkmj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dfncjjer.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wvknsdig.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vraaywsz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3iqfgiadn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yetfuuca.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wvdhuxqu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3byiqyytv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iajvrnys.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jlauxqoj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fqtygxhq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3atiqwlci.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lqtvergc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3pphcqvaq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3eqgfkphd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ttbgggxn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3betuzkge.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rcizywpz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tagjnsvf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hbaglbot.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kmpeogld.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3edtydhky.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ithqtizm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3oyzikhmb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wuijklch.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gofuwejv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wuzschqw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3adyqomtr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ciirozvi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3inhakmkq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ihhuvpnm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3axqqwsuw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cqfurdhc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rhzpxmiq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3cezbtoat.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3cnkhbjvg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3jcfmvgdz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3rsfwjdqn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xnpcrblc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3psjqwcjn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xfrlksub.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3guoodsiu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tiwrugjm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3xobcphil.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ijsncbjx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vnawsjfv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3imqbpoiu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3hgmolzsi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3swasvvsa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gclhryjo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3oiwoecsv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cjzlymif.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3gywdvoul.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ghxrtpdj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zxquvjln.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sdbxjbce.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3lbmktjyc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ekpflpto.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3yzruvfmv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3slwykofj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iexzkedt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zezoxukr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nyrvyoei.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3vskffcwx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3mbueerfe.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qjiaelua.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3evnthipg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3fjnheton.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ubetcjjk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3khoynwzo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3qgxcdwau.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3trmcfbae.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xbikfgst.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ssitulds.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mttgrjyk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3wxiswugw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kopfjpxr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fsmdxaxu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3pidvjumc.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3amtvvxjx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ffxgzwnh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mhegujsy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ltjbevgf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3oywspwox.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ppneejxb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rtmharfi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xulffnqk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3vgdqvgpq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3oofqswuu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wwuhojrn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rxacqxzg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3yqyvapal.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fkhjzpxk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tflpvtkt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wcufxhsw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xvskbfhm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3tebfhdwg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uufocmlx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hcwymkot.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3muujgbyb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3evleelhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btcpotnn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ocwrdhom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxvvyqmr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zluudyyt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wqvhhmol.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3boijqzdo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hhkgspse.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lyilgepx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3gvmqqzqi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3kgpwoxpt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hedkaiht.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wkhdxoui.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qyidpxjj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3foyloyjk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yhuvwbht.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3miolkttw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cilohwjk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3trhqdkue.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cwppevne.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hatwesat.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3zgimcacx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3owqzrmdx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3sfgpndmx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3rrsaaojr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3glrdjuji.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3oestzmva.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qrgclcxo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rjmbmryp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3wpcbnjxc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3knqympca.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oncshnau.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bjxgijla.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3aegowqgo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hpbcyvlz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pcjyiemx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jwgmculi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3olxsgady.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gkdomytn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3qumosjuh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3auzybdny.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3crrwxtdy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3npcqkixi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3uoepiyii.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3aaeqiolc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3msdkbjbx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3kryajyky.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hbeeqtrv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jgsxeakh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nvawusxn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bvapjchc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3blebosqa.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rifhbefh.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3jummyvjg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3pjoargmu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xahzsyuw.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3eelbqfzj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3xyxwzgkf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tmmihjbh.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3oextgafz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3pqtcfjvt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fpsutneh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3umwyvoew.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3cibiwegy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3igimedmw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bohrtgro.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3jhwidonm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3aoibropm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3momjwqqj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hbwdrzyn.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wximpeph.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zsocsngo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hvqvoejm.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kgqvlcpu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3cnaedubg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kdhiemyq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yufjyxyo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3snzscvab.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3lbptokhl.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jkuzmxij.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3oxkevqza.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fnnppiaz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hbyvzusg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3vlhyoyly.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3udocvjaa.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3fpvfbsmw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3lqeuhclt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zjppgijb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ommtzyvm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3xyqlbikb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3oqpyvauh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3athfffjr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sogakset.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ditulzgs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3lxdwkcup.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3bllalydu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bduzkjgd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvsqdazj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zsqaxxrr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ztvvnzux.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ybqsaesc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3axdbllur.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhgwgjau.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3yjgjgnxl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqwoyvdp.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kqzarcpf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wljoupnc.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hekjuoik.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3eivhsage.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yxykmjlo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fpczxjae.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kpodsgti.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3gdhulxpw.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3utltybfq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tijvdkba.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3facujsed.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bpzauwmc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yxwfrjxo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cujkmenf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mzpfhedw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3xcfzmadw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lcyfhism.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pvlikqwe.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fvdhfoze.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hkvhfvkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hosyaojt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ylettyiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usidflep.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3akznwcqf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qkjwshlr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3xzeavazu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ybsvxmgw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3jqyrfwch.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3pctzbmxc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3heiyjwji.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3atphoefa.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pxjomrpx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xbqjwcpe.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3pstgjugp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dxnrallo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3nxosrndq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3sjxvnpiy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3lmnqppqw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rvoggire.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3akefdtzg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3yshhavjk.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3nirxspuf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ukahugdf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qetbajmt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3piccvqnx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3dsajlvxy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uljmfbtb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3lpedtdli.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3cdbuypbb.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dfpxspgk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3clrlyaqq.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3dcwhagjt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ulhiqvwp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fzpdqrsc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3xgvrwjsn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3szrkgxux.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vjrsnrpw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3iallwunm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vewdoija.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3hlelphpt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqumfmam.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gdgmrztb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tpivrisp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3gpnoywqj.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3nukltvti.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3vjpeuqei.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vcbcualw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jmmbafqo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3oruisvws.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3etjhcslq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wsnhunsj.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3kgdafjfk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3gecdjaiq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xzbfercu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3wyvgvzyh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3sxymjtin.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3dwbtecha.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3cgceddhj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3eqaamqzh.html


<!-- 参考信息 -->