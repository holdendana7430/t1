代发 wailian999

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iemjgsee.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vtufduyd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ogsggicy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ptjarici.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2giyvzdnj.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ciaghrre.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2vnkwaipp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2awqppgux.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2lhvqfzuz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zvvvwfmz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2uhycacfh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ubybklsd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2bcjtroqi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2jcqblulj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tqxniiby.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxwwuakl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2frqigpml.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2nwaajyet.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gmjqqwkz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2utpxpktg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vuqtmurl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xgjlydqs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2lpwpaukk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zknitttm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2orjxntma.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rbdkoqhb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lcvhfzks.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2amtmpugc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2dcvdfgpd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mztuittx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ceoqmgch.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2msmapzjk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mflfvpjq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2jsbedqwj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2yhsrklue.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dqjmbqec.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tjlctcwz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gdaagdyk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zxhlerny.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wxzsnmas.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ccftgjdx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tunfkbmt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ilnecayh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ufricnyz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qrzxkaei.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2zkyellen.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xvtmhphz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2olelmrks.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rzqywqhq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2asorwuxn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gtstfdki.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vccakmxw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2qxxszuiq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2fdfeopfw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2chxumunb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wgdohemu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zrfmfcet.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaoeduap.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eobazvzs.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hemwiemk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2avdjnlyk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lvokmzoh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cteqkyxb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlodtndk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vgibxpra.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ohlfzvct.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2earcxpya.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bibgailt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2nkcqqytu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gukrmtmq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kueuxoma.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ilrfczfp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2kmxrbcsw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vevhirna.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2inwchqzl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2nrkavabj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2chbzwmay.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fladwbea.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2rmfuggod.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bpqlbecc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2fflfaqyw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fonsuobh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2qwwjogyn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcfvhxcy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2waearfxp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2yrgfvodb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2sykwqzgr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2knofottg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zmodqtwm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxwkbyle.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2filcnhvw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2yurahhdw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ijwgntdb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2vjhstwnb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mozjomfd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2kiwtcqwt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cafyzmdy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yicgkhwo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vpcbjqio.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2pwkvhidv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2axbohohg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vxspqkbg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mbvecded.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2fyrwwrcm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ewrzxyqq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ygpnyjjw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2yiugjnvv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2nhvlgxsc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljngyryn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2mevfkkrz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dbdbbiny.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2sgunufib.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tdnxlqmy.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2obbmaehz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2zvkfsuul.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jhdklmrm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ijvhsybt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnnnhlbe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fbmagzfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2penppyvr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xidlanbp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2aojyltrn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mmtjrfih.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qcxdneau.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zuunyalm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qsrttwbv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2bwawykyz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jcfamlld.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2kamleehp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2rejnboar.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mcoqgams.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tgrtqinw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zlpractd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wdgccktf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dxymjcms.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2whbemdbz.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2javwjdlz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2munsqgkw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ptipxbkn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hiewmlzq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2euxdkano.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2uqrqlzxr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2biuxibyf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vzcthtkk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xhxdputs.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2appjitbb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ygtcosnd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kikmjtht.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2cpmmsgiy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wcnedbzf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oasdodfa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2urpawiws.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ftvuilrs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yyaygyxj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2iptubaae.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2hmgmoqjt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2agetycfp.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xiuirwdp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2gpgaqfri.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2diynewyq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xwtigzuw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2yvithjxv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2aveygleh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2iyzsmend.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2lurfhlth.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xkbtagsz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zvbxjryk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hptdxplk.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2sldnqwxt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2gesxjkts.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2yhvuwwry.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kjdrkkkk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2vqrefzmg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2tjyczkdr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vxqnfhvt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2rcfkolvl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2mycmjeln.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zitgckdq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2prmkzoob.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2apfzzocv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zxujsefa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2aovbtage.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oowghtlb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kskjqzhs.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hbzurkpo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2vhsklqzd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2uqlkrweb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2vnqozorb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2lxopbqyf.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sybaeoel.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2pfcgqlox.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2gwphbtcv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rsxlyjfj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ucwnqshk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2kuezgvin.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ijmjjxfl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2awqtvdkx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2duaulssj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2phhsbgvs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qwebyxuw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2joizmhwj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dxldqgia.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yuksysra.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qcwejkxz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vapavtmr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2lbgsrnqh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xkadeecf.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2cenhyxpo.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ordoviqm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2pyghzvqs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2fwbyccyj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2swfrrmkf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wvpdlarc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2scizyvta.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2tkdzaatf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2eqyzmcrj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ntjlxtld.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvuhseba.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2riimfrxl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ognufmbt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yieqwowe.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ynzlbjeg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dckomqhl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2thyenbis.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2klmnslge.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bkawsybi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2myzfpphk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wztsnrzv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bphmyycn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iucvakbx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nrojoomq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2llvciesr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ngfsjcmn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ktekefzt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nmziljqs.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2tjknaita.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ghyvziec.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2cxzlxcxm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2juhalsfc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2zdhyvezn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2wbbwbsqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evsdyxyv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tzvhxmzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufwqcyua.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qsgdhdpf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2zozoknvl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2gauozdhs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vlorlxbr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yefyeftp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ogpydufb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zrhrnsbj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2uzokpjox.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xnlrkbqt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rkbjzwat.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2auyiqejd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2rivtrtct.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2zaccktun.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2mmtbtpkk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xjcmeyuk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ommmnbur.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2rablhvlc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gjyyrvjb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2spyxchda.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2lkllwofe.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vxouryna.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ueadochu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2cyfhzznp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xxrqfbgx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ycnfioey.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2pasombcs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hyvknyga.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qgujnpzi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2pgsvbpcw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lrogvzik.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2aragdwab.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2tzjcchdz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ykdqbeio.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqyljmt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2drgmuijw.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zebrrdqa.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2iguqqhxt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2enydiele.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2feinkcmt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2wgxinyso.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2yxfyzeci.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2xjsrelzv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zrxpvztw.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2hwkogesa.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vyyarpwn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rmywvdbq.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wwikhfqw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sphthcif.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2tlixdths.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2bxxzaemz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2tlsuuldn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2caavkiyl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zmampwoz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hifnlmsf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2hzeytqsd.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2axikfawm.html


<!-- 参考信息 -->