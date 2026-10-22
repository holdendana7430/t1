代发 wailian999

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ihlsbivu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wezegrat.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2uqrspdrx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nqzvoemh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2uhbckhsb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2gmvnbeip.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2kjbdowia.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rkbllaqg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2itdeagic.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2arvwtpyc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2sajrfogo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fnfahjcn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2oapyvnyh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dlnzfsds.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zkzmqomg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2htwynzmh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2juixtfmp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2dvusvzda.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ndjtpuqk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wdudqajc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2spmhpxyq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2koafpgpi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lsxedggu.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bkourikb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bwlekunz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fvywmluz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wcadaksh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jchcxdom.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2thyoittn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xbnwpkgz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rtbpjjcy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hcvcxoug.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ijjcuvcb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2dnjfuuwp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rlzhwrgm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vokxexff.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xzigxctx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2sruaxusa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nakevvsy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zzrmfvbr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fvjohoea.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2etjlpxmn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2nwpsnopz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qwdgdtex.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2pketnaxp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2zbjoxnyz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mnypqelg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ofdefmso.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mdujehym.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gvbquyki.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ebjqxtop.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2yivrcxbu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jevpohmz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mfghgtuh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2elslosss.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2izpcdhud.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jfzwutld.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xopsycce.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2salgtmzq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2cvsndgka.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2dbhhftru.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pruzqihx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ssejkauj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wsjlrwjj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wuglmbub.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kvtpguwa.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2pujbptyl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qvywlecc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2odhyqnlj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cycqedhg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bquldpnt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2foxqzddq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jhvtndgq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mgaoxaif.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2dlbgjake.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bnfiozwp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nnmhhkoc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fghetpmo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gayinbve.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jefxdrol.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2mjqqkchp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2igyufraa.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2writoitb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nornwlsm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rrvnyjwj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zbcjxtwv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2gsdjvmzu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsnpxeld.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lhlshtrr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfgyqrqw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dtteqhhs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2jgstaqzr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2rhdsvvqq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2llofdfim.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dbphbbvr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ajsrdqfl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rlnqcyyr.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jadpzhhl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hmekhjbh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2einouzix.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhdpeawa.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ijftxyix.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jqsnxkvc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gzelbnwd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2szixiaad.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zqphxakw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wkbxukje.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2blctbnkt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgvpkvfn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hswqzwxr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uxfwrtow.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ufrkjzua.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vcrdrdvm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hyqybcsm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2tdhljjwb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kqfltpns.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pofqkpqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pokyuyrs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kpjchagz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyglistx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xbythqqj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2galsmxck.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vxmiddaf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hnixyvfl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fvfktslu.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lwejavui.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2adyzxtas.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2idbzhqpz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ojuaoehp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jmvvwake.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bqgglcmu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jsofpfhb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ugkmaoli.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2evfxqksl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dkapuapo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bqpphuqh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2wwmhjvjj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zzuidwgn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2hyhsgyax.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2wxqawivg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2gplewqsz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2orjgrsrz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2upnuqspq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nkaqpslh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2hhhuxfok.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpkpnemi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2uoemxztf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nvqtwbkj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2gfgdhaqu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2blwunmkj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qocefcmm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gvvnrkdl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2vleqsasv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ngrvdqmn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2zebopfib.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pcsglabe.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gixjhjxi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2eghzktuq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ewjqhist.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xsuqpwwz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pyxiyeqc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvxmxbtn.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2bifwhkok.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2utlkabzi.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cxcobhxr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fmgkbcpw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hywozkyr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qkjpvvhb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2sudghvlw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qrywhbwk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2bvqczxut.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2fcrjvoub.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2gepwkmki.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2nkisunwc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2bgexeoch.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2xjywpjwy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ejclhfaz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dlkeowhs.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jdlqhpko.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rsryrlzm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xfwunuxl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vpivxavw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ruvujcel.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cqkkjxog.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kqdqesod.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2szfmhrxf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2gygbxijk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kgxasytf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2hndiaggx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2koykbcvj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hnwijwvd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2vgtedvzg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jkjgcrlo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2xyryiuxp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2syhftkxu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2czfyfkaj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tfkxtehi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2olyhyvmv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2zsttetmq.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2tmmwzvoi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hahhxgsk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qhuhgegi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dhqfohde.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2msodqmcz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wprgualp.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2fvodjaoy.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cncgrdmp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2lfvcswkm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cmjqvkgp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljgpsxwb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2kgxheskc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2rjekztqo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ualitktx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xckefxoa.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2rrttpeul.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xutnwtid.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yureyawc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnvcbjcp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hqmumama.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2kvqkbbgm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2mwjawziv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mlvwxpca.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hqzxfltt.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ekaqcvii.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wdukwing.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sldduwjm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2feqlgsex.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zvvgrmao.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejsnsufk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aquewfcx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2xofhdwti.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2bmecpovi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rxfxrksl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cwjumnfm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dsjbramj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tstteitl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2gbvfcown.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vlromzwx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mircideh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2vxgdydhd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2imexzvjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olphrtny.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2oqickaio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2scuyrpst.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2hketwizd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2cndnzxon.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2tqlfyryo.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2wuzmfnqy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rmqmswcw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2olwptcfh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xehhvfiq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2olmvumbk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ndxsaojc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ditkczkq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jbacxjyc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2rnvfzqxq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2pbwvklck.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mqsnpnrw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ijcixpom.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2efeumvkh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2vazssqzt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2uzloommw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2lgdawrwi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hqgoqqyx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ikjdsuxs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qlevrcqu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2suvcsnpt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qqwolhbz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2oxziybht.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2knpokzcd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2sbatmzgd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ylynmybl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2plobbcpi.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2yxvsyvqb.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2gbmszxib.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2yivicqcw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pdowqnmh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ixvmljva.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kmpptewr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cmwkvvwt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qsjjbpmr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2lxwkcjhk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ktdbregj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jqtfsrvg.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2xrnpauhi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2zpsjuquq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ntzmyksw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2ilidqxjq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vuxxeext.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2gfhkhzgz.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2nkdihnko.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2msmzeqlo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2wfjgxlcj.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2pjqoejtt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2tjfnllwj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2utvscucr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2gqngecao.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2xgilgbaf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2orqxrutd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2fdtatolk.html


<!-- 参考信息 -->