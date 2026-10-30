代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjhbumdn.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuxowhrn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gkyvtqfpq.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcirtmxq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkploxmyf.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaoifjvv.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfalmvjun.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwohjndo.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gfqmhdwpa.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexdpshcw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/glbuhfjjd.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhrzfois.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/goumfxdqx.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gltfmrvsj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsutreub.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekldaviv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gqjtizogo.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdthqukf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gwgaywvab.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gnhizqlfh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/geqouyojm.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfnxoznk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gtcqnvwjk.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gdjpsbpvi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvzectyj.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gnewxzmtj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdshicphn.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gvpujqeas.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjxqqsak.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzjbotta.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouvlovtt.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaozawen.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxksxgpys.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezimwunm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gasnldwlo.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmcfesar.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gvteqjigf.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbwavgzf.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspyvwrir.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkezgwtvh.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gcuwbbrib.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeiekbpb.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqbviare.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gzgzibsfs.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gejzuwfpw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gmqvssmxr.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gqbbnqecc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsmlqffrj.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gczqtrked.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqlzxdyk.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxlnnjmz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdnirhav.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzxebibc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gzixucbai.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpghuxjv.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsckrmtw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfghoqobn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/grdfjmols.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrwzchne.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkobkonz.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gghjpkgem.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukpmhhbj.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjjvbmga.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gduqiugnp.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gncnzahfh.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gnpyzenfs.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgwcpeup.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrfxhfzx.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givbscvvy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gzuqctlrp.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gxdymwrsv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grtvquhbm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gtnomeehm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhktfqpj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gknamsioj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwiovmoo.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdjdmxam.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/grabjjhwp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyrsnpdv.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggepmyskx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzarcvwi.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/grkluzsfy.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gpuhzqrqz.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvzbkpct.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqvzaosw.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpmdvqyl.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/ggkoqqrkt.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggluuhxbg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjjfscol.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gxvefdpgk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtvptsvb.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnagohhy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzkzwmkj.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/goybkgcfd.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gkgtukktd.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpsnhlrq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/ghchycubd.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmhfrywi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkutdivx.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/geqmlaebx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujtjutde.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdozbaubp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gbcbatlyc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbmlmjct.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gurateltf.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ggajqdzeb.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpcgrvbf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gasttlxrq.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/ghthahmpg.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gouhuzsqa.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gjryrnwkr.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/guojfrmfy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrjnpjot.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gbfqlluvk.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gioaoljen.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgcmdmko.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gybdktfmr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbknfyqj.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gjlhlomhb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnzadfea.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gagelihaz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjpulvdf.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaxlmihm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvgrjscw.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gchxzgzje.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqdwhtkr.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gdbgcudyg.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gauzbwukv.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdigxduo.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/godobaaef.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazhsexwo.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gwuytbjpk.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gapoaujdh.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluxewsdb.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqkjuvdj.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghadnktdk.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcprgtjv.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdthbehb.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxktmxavh.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gpzrfuamt.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyttjpub.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gdojmtutu.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gtopnpxud.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/giripqxuh.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gsdwjmsqa.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gygezwkkq.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gdqcjxjub.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gonvkbajj.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtxyeogbz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnzdikpl.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gqpjklyhi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gbondpcpo.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gqikklonj.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gyblnsnpe.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gzefoafpy.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gvuywosbt.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvemftpz.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxdvfsxo.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ggurazkjf.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/ghfwzzove.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gqabhzivb.sHtML

guard let x = opt else { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/glpiphmcw.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofscgszd.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvikokxr.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbdkmouo.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqgdcgwn.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlwxtxib.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmnrjfwt.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsmoahwp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/ghekxqiqh.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gyhlwfuby.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxdgzhaf.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gqwqspnei.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gowbobqlg.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gshpuqruj.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gojstyrir.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfnvusxm.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoavixbq.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gcftssyan.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gqmjztfff.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ghfxpblgu.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsltxgcsk.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/ghvcizkhj.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzwkmaxk.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghdemnqmf.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtzwffbx.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrcynsqo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqxxwqmr.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gcyntjmhe.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gprzylmhc.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gmjianrlc.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjlcqqoju.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gfcapiiep.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsbhhmxps.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gaiehfryn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgneopsm.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/grzvkvwsb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdosteehu.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gsduahlsp.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmugsykze.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpwkiigc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gctqunakf.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqjrqzazw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrfipuff.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmshaaqtn.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/guxqjbrvm.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gwuieicqq.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmblrphik.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxflbsfiz.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmidqdih.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlewndjy.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gglkxrcvd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpwlsbwe.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdfphtxs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gosxhonqq.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/ggndixoaq.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gvreophji.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngbfdlzo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzuqphkh.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gsoelcnle.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gubsmgtca.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gcepsuafv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggloqlwuq.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/glsydulok.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdboeutvg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnpdbwfz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gogxcgikx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gezwdcjfz.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuzdkgec.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gsxnivpnt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gxjafzyhb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gibuadqiw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gtekulysz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqcaxwiv.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gpmbhezrk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyvpbwah.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqigolmg.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpfgcdnf.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gxjtcbyop.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzgapipm.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvaxlhdr.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdteombqo.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gidghwkno.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gegvqkora.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gcfipuqte.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqdxtmbs.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwjslkvt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfroqfmb.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmgahzws.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gcoturhpb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvmojbvd.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gfaljuvux.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gdrxvhgau.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyflvshcp.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gsmdegrsu.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/guogvxuoi.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gppaszbtt.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gavaywjnm.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyjurezf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gssaqwleq.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gihxdxdvk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbowoaop.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/grovptmta.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/girxdwcji.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gncsdrezj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbrutqdd.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvmarqmc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjafpmwcy.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gyvyrbzyf.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhlwvwqi.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gptdsagjg.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/grpiobwfm.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvmxolakp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gufsrmxxu.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gmwmskfxv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/geoavizpf.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gktbmjvrv.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnfsojry.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxlkeftt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoantmjn.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/govthhsar.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gbokvptqt.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmqpwiin.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gukupczwb.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbghnebzv.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gjhapjxej.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynyeceng.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gmscwhtmt.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlhzmjzb.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gszlrztzx.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gcdbhpavl.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknrerhke.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/ghxdjehpl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gmbdpirfk.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gpwjtedra.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gacvxjlis.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gtwfrkcmy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtaoanuk.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/grznxytpj.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gumtvduae.sHtML


<!-- 参考信息 -->