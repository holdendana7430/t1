代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2utslizna.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hbluojdj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lfzktxov.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ysbozisw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2mpuuwsdg.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2dzqpsagc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2spbgenca.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlazkset.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zngddtqe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xkonhpoh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tnwqamxu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfsmkvvo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hkygqwyy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ezkzisjz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ziyokezh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fycvjggp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2tuxggarm.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vgohvyvi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jyxcqdhb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ublcvmdy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dailudsu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2anhifdur.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xttjcizp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2exefrlpn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2rrcijziv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qugylmph.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nmwkpiry.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2oexxblxm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dwlhwxic.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2rtwltfqd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mrdevftj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gcipitkm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2immgxvuu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wedfrcjb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2vsywbumf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2yzkiotix.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2coeashdb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2syvkclbu.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hmtwtlaj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wfsjpuat.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yrdkyddh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2gicyovjt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aunmkenp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vgsdtpde.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2euakkqqq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2xksmvzmy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2lakujdhb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2stesoqvd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2afyrapuw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2krithsoc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2eduflccz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rphyxbim.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2thycukjk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wtjeswca.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xhgyttkf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2uyggwwqx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ywufuenv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pcwnuzwf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2gjeujgsc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2myjejcnt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pvvcduqt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yblszzpj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ivujxgbq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qtdkqspe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2pustcacg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2qyrdtzjs.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2xuoaecek.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ozacloqk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2njqxbxfp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2gdcaziwj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2hllellwm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2inoqobuc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2wpftnxcw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2iankznmq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2xlfzuzkm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ksgsckjh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2jbqjewxg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jqaiboox.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xlumsyes.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vmmtlcoh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2hutzhhsf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2vhbqtism.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ltinkgye.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2uhcuedke.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nhorjydl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2clfyokbp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2oaroqeuj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2oyguhayz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zcfwcwyc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mlvmooha.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ayvmzrmg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2oqnamifp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cibrskab.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2totwdjxk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2amhjobsn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2btseiskw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tcsptmbk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xjvkhjrm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2qawmxorb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ktezezke.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wexbfjgl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dqfkeyln.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vtbfgusx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qtxuummo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2nrczmkso.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hfvvukqk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2blgxvfly.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gzzlajxm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2yushaawv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2dshabqcd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2cstvsecc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2barbkwzz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zvidvkah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izolfwjt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zctvrunm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sppqgndd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mwmnqbij.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hgnnqgru.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2evcjofqd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ezqcdnbc.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2unzaqjox.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lqwcngyw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nqmxbnsz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2itlhuznr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kcmqsovj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2kjbemroa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mufzvfyz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sciassby.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jiufmfln.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lonbzhmi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bxpbwclp.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tjhsvfvq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2qprgmysj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gmwwcavb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fnmidrbi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ixjntuax.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2fawsumjj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ogagrjjs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2mdtzigih.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cikctvat.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hzoslyik.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdtyvklh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ytyoivtq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jutnypur.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zilltxba.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bqstulkb.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ismmnvrl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2psqikqyy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2yaxydvhb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2odakntav.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tiyldkyy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pdymzbfr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fykteqkf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2bjrroufp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2dynpahpd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zslbtadi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iibsyinm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2vjmrbndt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2pogbbhyu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2upnvxxnl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2trmqwsou.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2yrobtwjy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2efebmlrp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kesfysvh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wqlbahri.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2udeokuas.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2oisqtlta.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ircpngiu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2upepjcvh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ogieeepk.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cbhatxea.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2elpxurwx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lsrwbehl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gwbxfeih.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2upzewnts.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lturgrka.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2swqeatdj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bftdmfpm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bmjbmciy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2sxevnsru.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2inssxncy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ztdvaxof.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mjeukmtw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2qskyuasq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2yfikvedr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2xyriqvgh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2lvlunqtv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2mbxihjxi.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nrakimzd.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tlgpyepx.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jtoxonjw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2nndtavyx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2coqgcstx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sjiqqpho.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2twbrgrma.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2mxlyikpx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tzdaumsq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2dhjljyne.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pwfqresl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ikyfncbw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2onrdgoqn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2yhqssmfb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2yhekxuus.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjlqhcfs.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ojpnkhor.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsvigdly.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2tqkqyfil.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwgpkyli.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2frdrnajr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wukuksdx.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lczctqoi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lhlimbih.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kfzqldup.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wyhonnbf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lvpeewaw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jneyfewh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2blryawzz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fyyjifle.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2imxgcgbz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2uhfchcab.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iyddlqwt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bqqwmmrc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dayrajgy.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2thaspifk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vwqnrvnd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2warqtlha.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2dhbbwolc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2oeohqbjt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rdxnutts.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2agtutmvd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fmencmhb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2xxvpcokn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ijlgpkij.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tunbuazd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2swnvjaqv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ahggchct.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2mkkegkwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcmvckqe.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ejvwfhtt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uiwywtfc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qqmfakcu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mfqiiyha.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tgkfeavw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vgtgljwd.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2nqpuocws.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2lotppkry.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2pvpvqtub.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2vxdnymnt.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2zpzlqdvg.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dxpbxmtm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ajgfjshn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2onrsrzrz.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2fcieektz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2srbgbiwx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2jlwahcwx.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2urztybfb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2hjcdddvy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2rjacekmr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2jrfwdroa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2ayuazfpg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2hatjqynl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2gkoiuicz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2uytfcdip.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2aqoarofq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gaturwcy.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2sfwiekty.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2slgysbvp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jutzpvve.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2xhexejtr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2elnftntq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qiavhoty.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ahqdduan.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2yatfqoeo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2pitisoxf.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ypirbcok.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kmitsvgi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2fkoctdpw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2utzjvlpv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2rrzvebuy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ofvcxpxx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2htrrlpkw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2sqfxnqik.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2bvkwdros.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2kztncmwf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtbbtshh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2uccqgpkd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2iplexwrb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bscexiqb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fxarjera.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ngiddkqw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2sukghywn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2gwftdctv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2pbapmkyz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2jywnagdg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2tthufbff.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2iptsccez.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2eqwkvzbn.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2gqnlaahb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2pcneolfb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2oqjfvcjy.html


<!-- 参考信息 -->