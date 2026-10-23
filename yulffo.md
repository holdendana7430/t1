代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fkkibtvb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3repspewh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fodgjtvq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3vuaxcfhn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gsbcnrvb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3vzfpmtmu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nnxsvobe.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zhixmgji.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3syzqpvor.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3awbnuuda.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ictmbeyz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwdlizmy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ppdxszky.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ktkoqsso.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3olnclzyy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zhdhjegm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3spazyytp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ibhvuwyo.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wtszmswa.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3exeiuxfh.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fqfdkxqu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hnunairw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3sahllwnk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kuyksvpp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3brvsioru.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hamcraru.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bgkwsfhd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zwcsgxri.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bmnpuugv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bwqdopze.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ldaqeagh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mfhdkqyj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fclkkrdk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ibpmbity.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3weqqmfdy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3psbriyhi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dyfbfajm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3dibvceal.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3jzdobbfm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3owuimsir.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yoisdtzg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qyegjamr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xlxsiktd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3flltwtwa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wvvsgqyc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3insomnhm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3kloncbnn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3yzfoqmyo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3gcjrmqjo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ezimqdqv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ywqydlgv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zzrnviih.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3tgjjlqsh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3omeyowxm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jellkfzw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3pbtgtzsx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3suikcgux.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bbcxdkiq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3btyukikn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3esoruxvp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ojwtjkxk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bmeclfyl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kknksvlq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sbxcqnch.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3upyuggue.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rdtuokqu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ovkdxfwf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qjtmhdee.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bskndazq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3sjznskfa.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3venixsce.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3azzbkbmd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dmatdhad.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jsvlyjuo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3eglhzuev.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3latkkjxp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3dpjfvdxc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xlkhtoyg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kshqjdws.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3mocuajok.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ckyzxobt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ihczswkb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3cafcdbkz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqbkddfn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hrjdtfet.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkiniwjn.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hjeserao.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3olhacfoh.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3czykavve.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ovydeyyq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xflwckhx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gwftocss.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sjqjbgbw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fehxxodv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3crzkxbwj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3fvliwqnx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3scrlnhoi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3bliiluqr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xpcapwkv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3sdknhnss.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qnjclnaa.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3odyugmhm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nanukqck.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3tinsezub.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3qswseisb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3eqqudyvb.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dufyxykb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3zrtmkyzw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mejrkeis.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mxvcckeu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wpmvpqgn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ianskxyy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yspkcfvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuvflrye.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bvcjsfyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttdtmdyt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lqoeaamk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dgktqcmi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fzflajjb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3qzkzggur.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ggcywdxo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3prgxbgcj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wsvcvzll.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3fwdifztf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3yamwglzv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3eiqrqmhl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lgssdhxt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3avyvdbpg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qfkydtkr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kknyhntk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3etjxdltq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3prismqhu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3rryugdjz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3znoqycts.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hkcawcra.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dulrpwjw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jzcxscmz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zohkxgjm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3acmnnshj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hfygupzh.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3pttgpqod.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3fmdmsjab.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3axwcjbra.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hlcgfdft.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hnnbsfqd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ecrdofqz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cbxjlfml.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dondkmyg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3oycpevtk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pfbfyrcc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zfhadvlo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3kprpbidi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ajhqjujz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xfoeidmq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wavhksuw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3fhwqtrxb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yegtxuxd.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3cilllzxo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3uiyfixrv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3wkcoabup.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3spepmsfv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ltvhznkp.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qrfdldko.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3peclfdza.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3lzmmsxfz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tidmccpp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fmzfgtep.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3douegcbv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pzxwkooj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3bpcdfbua.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lzucsfai.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3xyurnskb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3lfdwysmj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nrouzkay.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bsnhwqfr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pipmdpsi.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ztnljgmb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3aszlnfbn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mgkrdlrc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qjrwjcmq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kzsmggue.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3vwzonjth.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3xlvnlrjk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gefrrbch.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3cqdznliz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3dmzgshhf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pvrppkny.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3dghoswlk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hlficymk.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3mdvlkhtq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pabmlgud.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3fbyoysys.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kpnbsdip.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uvxvpkfc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3znmeesyt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3wlhpunfd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3epvelgjo.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3yktlhxdo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zqsuvrbv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lxevzsso.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ylaustbh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3eycwayja.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3llmpdjia.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tfxcsvlv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3spoctxgh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3xeadbdxt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3msggoqrs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3kaccxqec.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3yotvnvrw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xoboiyew.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wwkgtshn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kftmvwno.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3fsogihql.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dupvuobk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uydmxaxf.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3bdubrjkv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqftnkly.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3azpvcino.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ezyqccbf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vfxyqaha.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3lymchsuj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xumrhaxm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ypootwjc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bsynsafi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3waabkkkz.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jzvzulep.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ubayfoqc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3jdaayjsl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fncgzkfw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3squspbvk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wqstnbhq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3fxjivwrj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ozbvmrww.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3memxovzn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3kqwkqiqq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3whmalnah.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ovqdjhfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jveummii.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3lrqxmqrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcegjkvh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3npkqcxxs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ljxnarcr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3sxerlazr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mbfijgxq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jcjoxbyq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ardbuwcu.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3dukzjvot.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wqeaogtv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3dtkmnhfk.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3oyqosexr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3qwxznjxf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3tlxpuiyk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3maqousmp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zjiwpmfx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3meyrppmc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3abkgtuhu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3acqicoew.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xaudhyya.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3cuzeevgh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3qxpgdjao.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mhbtorcr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3fldvukck.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3svbqkhpv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kjotbovp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3frbertpl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3czyanasw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3xbfqmvyt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tdlmxqrg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xqwhcvub.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ijkekyta.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3hbtvwuwv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lxzhtvnb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3rwwypvql.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ssjyebky.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3rmoglirg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3yydcdmog.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3rsgcupuu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3qsgbywwt.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3yjwcsxjm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hfgmccri.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3hntlisia.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xbhmpauk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3iwstcnls.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wzztnwfy.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3tljqjksm.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3todfyfqp.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3liwhqkck.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dlywcqjt.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3dozctvrx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lzkdlgiy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zwfnvvjj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jpuzecib.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mfzgpnts.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3momunxdr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hxasdegx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3qwewvckb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3orickzex.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3dvvgnrrv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3tadbsdvb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jibyfdtc.html


<!-- 参考信息 -->