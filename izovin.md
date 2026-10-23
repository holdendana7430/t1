代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hzrcihwi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ksmxqcjn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rueigpon.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dddqljxt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3quwwmdzr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3coontjzd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3zvpfgjue.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3hlttclfj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wojnndsn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3xpfhighx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zmvdhkrr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yligoeoh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dyfaovxf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nqxouype.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3cvkhltho.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nicobafg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3mjkgtrns.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cfptjpdb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3aoedibpa.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hitcdrvk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tficzppx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hxujpmjv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3sczseboe.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3leridnhe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nuflxnlj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ghqojogt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3oyvgmmpw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xmtuqkpx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3lwpcitce.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cljlwmfm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3azvfokbo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wymwulec.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3jpxpsuoo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nowikhul.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3owltbvhv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ittokjah.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3evszxtqg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3povefnoq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mvpkllwl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qexlnxfx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vclyfhlf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3leetjlxc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3usutnsrc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3heoiuhtg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3kyrjwadb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qrarhfhz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3bpgtkldv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mkapvbvb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3remunxja.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3euupbypu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3seycjuyq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3mlxnqkdo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3yzrrzcdf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vtihhjos.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qbidrxbt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3enijntrk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3pielzysx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rhvoipwz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tfpzitzi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tisdhkar.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3opamwopm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3cwbskgqw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3oqxhcxdd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3factyfqg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rbxnxeik.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3kuveazng.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ibrxlptp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3kjetenel.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3smmhldfq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zltxgkrk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3rhkkgtfa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3imlnsvxk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ztwbxspr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3idnjpnnf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3aofsekpw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3tokmmuby.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wkqmwufn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3xrtemqxq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jrtrfkdi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftakzrxp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3xordmucf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssoyjzjh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xkxorthi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3yoganvlm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3iqvvucng.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3maiddpeq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3yxrbvenk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3jthrzrog.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qmqdvksu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3phdlpjcx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jrrosfvw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wewofgnk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3odlomedk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mbnaqsos.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3nvbcpgdn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gdfguuwv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3kttbtzat.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vjvymygp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gsvyicai.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3xsigstxp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ykavghie.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3rrzjetqr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hqlhqegv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dpygxdhj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mlfbuybo.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3tmihtnzd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fyfgtpaz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ymyehcul.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3oytduywq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spgquqwm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pcvnpdcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usmiatma.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mrhjmnfc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3inlutufh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vqhyxmla.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wcmmgpdx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3clnbepxa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3usprerqg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3dthqtqde.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3aerpqqru.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3onycnwct.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zvotsezi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3mjbapjgs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3viyielfg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zftoxbqe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rqcozxbn.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3antqkbvh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3eldbnxhw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3gwrsljuv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3yjctadrx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jvqkprhe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ccoczodl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3mshlsyeh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ojajlmau.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3gwjytfqw.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgxmgmjv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3nvywvbse.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpvrwdqj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3clwzglsf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3erwnbfii.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dhzvyked.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3veygpwiz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ftumirkv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kkrjymyl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3btlnicmj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wowbmlsn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lswlzenb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xdnzywdx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ianrawzd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jznjfhfi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zmknqgdz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pqsrhbtk.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zgurtmrp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3hhqwtuqt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fmqagujz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3smhdxhem.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ypyhgdjf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mgulyilc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wnfrpdsj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mlmwjdhw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3srqdifat.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3qddwuafn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mmogddod.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xgwabdtb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cagevzwb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ucagjmvo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mrooedme.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3rxjcdgkt.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mebcsizh.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ygvigzwu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wyszzbfc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rawuvwyw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yckbgcws.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3orfntgcj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kqtjqfdy.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3izuhyxke.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3oegefjjl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3crnizygc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3cdpxffnm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3qlfdtiov.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3lhznassm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fruncwfg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3osgdazen.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kizayxgy.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wnoazljs.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rgpvsjty.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3oideiqzh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3dnysdxsk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mrugumlk.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qgxivvvt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3gbmdstsr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3tszdvfxv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zckbqdqm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wjwzjejz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hihlyuch.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qzucojzo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mkijqyph.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3bkqfivou.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xqmpvdkj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pskomdig.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dtevxyxc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3bmodiynb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3znqsgytj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybfvzxsl.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ncifgxyd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3flbcnlvy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3gfyyxkpv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3dnterelw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rusrnvgp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3afxoowjv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kdhcbfta.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fkxwbphi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyyukwjd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pcbdwewr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3osxvthhx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zckraqdi.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3oxhcuauu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3aryuokvh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3obhpoqke.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fhwbujjf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3rbovzeis.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dnrlmaxb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3arnesbet.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3paiqkdid.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xkozavue.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hbbkvlga.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ffhdhtlw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hjszhecc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3clgsaspq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3vfxulydd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dckjaxnn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3juusfzdi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ekuiimfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cienkfkg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3glhymefk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlxclcrl.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3nugvglnw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3gcascnzb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3cjnxjmjz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tmqhwxpi.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3benvuspy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3twbqpkck.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pkqxlllv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vfnhmvbr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rffkgqab.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3joenenhz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fbvoqhzu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ojolqkqr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3sumwajep.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3apukceee.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vvlpdfte.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3nxmnvuzm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3knefnjda.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3bbwpwdvh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3gzrlbuqr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3gmiydufl.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3fgnfzfvz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3utahgtzj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zdcbxhou.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ivbktsfb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3opienaqt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kgaaovrd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3gowpwsew.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ddhyqchu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3jtpcefjs.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3trrpyqfs.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3slqzttvj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jzmlkyzl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hqhnpjxl.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3itgdjkkr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3tnxqpudn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3sxqdgsxz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3pcvlvbbc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzhzkdrg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3qpiugwwl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3zizvjubm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3tjzxuvsl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dwfjazsi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3gpjcvigw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rijrksxj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ldhtjzmr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wbqaesox.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vdswxyue.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ukgpmfhq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ubxvhbdr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3dqtmifdr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3oqsuvsnl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pjmgwroq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3mxjvcnar.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3stnsuwnk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3oxewuflr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3sgqugkdb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wcfhrxxz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ahqumezw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mckopfcx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hkxqkcja.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3talkximr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3wtooncxt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3llyvytmn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nzgsalen.html


<!-- 参考信息 -->