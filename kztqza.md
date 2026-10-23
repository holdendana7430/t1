代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsgpbzur.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jdhofajq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3gzpzxbrg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ipwxmzcr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3lrwitydc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3zlnhezjz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3smvpxjti.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vfhotzvr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdmkhvwi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rvsvtbth.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jvqwqzga.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3teggjjoi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3iroqpczk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3wlkifgnb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cpyiwkkq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3zurvexsl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3whbhdyyj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ybrmtyjm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rkhctbfz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ogejmrat.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3bvmgrjpw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cqwmmhox.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uudtdmhf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qfkoulxs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dlkudgsq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ahrkfipl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3krauzadf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3svqxxvqi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3hboomtsw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jacwcqxh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3shfvxyvi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wnuyomqp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3emygrsir.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ndcyvntx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3wfpfuxxw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nccmqyzq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3axseicww.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ypiincid.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zqjcfynk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3pzgecbbx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oreaggoc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rgwekabh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3cwmjfbck.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3juvdxxpt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mqjcfijz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3fqboqwpz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3igzjwoxb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3iphfntqh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3adgmkqbb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hsvgeiax.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3huaogpjd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xoloncyo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3orwwqxwi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3crkmlkyy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wrycvbhn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3hmuplxzn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kcoojjli.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3lsmtwenv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3fvmxoojx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qqhgacfn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eucqoiou.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mwzqeukn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nkesqery.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cnyhtzef.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jqkylnuf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpbgnyow.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3spejytou.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mfmdydny.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3qisbukfe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fqvnqqqz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ktknlcfj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ezdwlnfq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3uatjpbwz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fcojcfyn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3hhnzdwrc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xusjidwj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3prfmcwmt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vltfsetn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3iskjboir.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mwnaqejk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3smhguixa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ratvhnqn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wwiixttr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wrbtqoxr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3puvzcbwt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3velhvrhk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3vrtyiaxx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cistjhwv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wyczpvln.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3poobolsd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rnrliyid.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrmqhvwf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qthpmsrp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3efdqqpia.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3nbqiluvp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wauznpyz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jkuczddz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ogywjwsy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ecamramp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3suxialhc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3aegvdjkz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3blnmsvcy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ymfxthyn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wpipnvky.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fznokqua.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ulgnldtm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ysholxct.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3kpdtfgvz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gfswpvvk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ctdvouui.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cbcusaos.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3uqcyhctp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3mhihruem.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ftfakihb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3busimurv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mxzusigc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ccbzboyx.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wyktleqe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3nwjtprub.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3nftvbspg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3bczkojuk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ednjfkxd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tsieekjl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dznjoial.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qpumnvnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlngizsw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tjdacdjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpekqynn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xakrjpho.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3msvawhkv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xsdpcxfe.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3hhlqrztf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3kqcgmfkq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3cfgtjqwb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rewrprve.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zieiafhy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uojosreb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3oggsvdqh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mgjyzwoa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jhlghraw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vcdqovgu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ywevzpjc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nrgqijpe.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vjsgwnzq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hiqbsgcz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3yvqglddw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3grjntwdp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3impxtcry.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3cpajkgmc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3odsfwtek.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3uvkqtiju.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpcdhwjk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3tuesdhxc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pchczmlb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ojqqhbmh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pdhhntyf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qrbbevgo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3rsqegsnj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3asolipyq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bcyakfna.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3nhafyrzn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3wmmrtgrh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ljjajdyp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3aokrstuo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wwddzllh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3zhfcremd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dawwlboo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3cwylgmcv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jgezhiwl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3tfuwjkay.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3dfkspohu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zjfelful.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3eufcjvmz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3xhwwietx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ktsfpsuy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sccoxzyc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3bpxipkai.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nqenlwvs.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3piavpdxd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3sqjsbcrf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dpnbmcrs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3kqvezhbt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rspuigyz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lenvuask.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ttfrimay.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qnmsfpiv.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3txgeipag.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3brrpbkyj.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dsnigcvt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3prswjokl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ynrexqls.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3seqsbaxl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ipacqlny.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pnvedbzq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3liizemvc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3qiuebbug.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vafzcllw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gwlvykrb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qoqiwgiy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3bdhxinwf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3eeezdwrf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3wcwytito.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3pfhrxaol.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3fuqangra.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3orhsqyis.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3iylihoxf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ztgbanbo.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3otoxjnis.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yorbdxhn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xmrynjmc.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3oryvgsfe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3egsqkffa.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ncsyrvqm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3pdqrcjcs.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rdivjelo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctfhwuzp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mwojhkjr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ktelsssv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3skyivvbx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcopepsr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ohwkaxxa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3toqmoyga.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3emittzjh.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mqviuano.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gwhhywfn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kdwboiul.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3csqvjlvj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ywuouzcg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjlqxmkl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3apeofraq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jpdqnvrl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ggnrzmmh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gwrkuquw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3podqprbw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ybmdzprn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3aipjutet.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddypnlir.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lgqejxwo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3niytyltg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3xgvzjwhv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lzrrgkbl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qzvfotzz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dxvueuup.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3geszljky.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3msmxkoms.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3alawzqem.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gunpvqlg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3kzimrtqi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3paxpitjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqwblquf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dobfgrhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxdyugzz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ezgjealh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3laxwhnkg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qrwjrams.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qfcbfqnl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nglanedo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3lasljpdi.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3zmygutwc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3coexnegh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bzffhkbi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hsqkdarz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3kgbhcsmb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3avwxodbm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3tcfvjgwb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nzftnaqv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xthtkqdg.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qllkenaw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3nnytcibe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3fjsbbsbw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3gqqmsedf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kfdegyye.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3qcblgsfq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nzwihibd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3gquteybn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oyfqsnbt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3dmnrbhpq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ublvbbjr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wffwgada.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3lfwfvlij.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3valmrnxx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zdfxjsdw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3kcrigtpw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3rjnoydgb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3gjfgcavh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3edzausrq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3frztcgdm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hfmszazo.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3klmtvvfn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbjsgoiq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3hnbrzvut.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xuxgdnfj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zwmdawyr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3vcvcwemo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3vmtcszrj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3iqljsypv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3voyyflyr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tgxaqduj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ajecocdi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lhhgqpqr.html


<!-- 参考信息 -->