代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gaqzvsafv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gdatlodap.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gimjrvaze.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gmyjtjdpa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/guuqfhwba.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/grplldkro.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gwwsgxqfo.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gdnppfriq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gjfdgolpr.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gvalaoqoc.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gyhrvfqcn.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gkpkiyics.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gvjjeqjda.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/glprlsmbj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/glznnprsb.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gaffnaroc.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gmhzfqnae.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gittueamh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gqagfrjwr.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gofxgnbkm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gjycsoqua.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gopskumky.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/ggnysgtqx.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/ggbnnovdw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gexsyxxhb.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gufreqklt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gsaejgncl.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gtxqimgyf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gnofunkeh.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gdmkdbkqq.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/glueaetcm.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gwosuvfsv.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gaxzmzkgs.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gkbwtzgem.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gsepuiinc.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gjsfslprg.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gwbpfpheg.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gxxbzuyzo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gqmghuxtm.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gejkwjwde.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/ggphpakjd.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gxsvsrdvj.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/giulmpdbo.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gtesuwvpt.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gxbtjwkph.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gdzfmagfy.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gsfaagdpw.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gmqeyjwqe.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gosdkyxoj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gxogeqxkk.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gwelxbaei.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gzgzkvbph.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gngklqlpi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ghlqisaqr.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gshddxtmb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gqxzmxmfu.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gdkjomzho.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gncfejnve.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gguvgsfgc.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gyitdtdhd.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gxqpdsvit.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gfpiicxzm.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/ggxeovwxi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gvgfksslz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gfuesntzl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gtvnhggng.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/ggnjvigxd.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/glrutrsxn.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gizrrdnpl.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gmodmwdsx.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gxhriciae.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gobryyupu.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gwgqrwygh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gidcnbqhl.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gmakmgocb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gsxkbjaow.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gapmepqaa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gvruugqum.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ghqnrkkhc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gpihsibuk.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/ghuylzxbh.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gicjfzgnp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gxkdveaac.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/ggqvfljgf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gkvyblzwh.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gxnkccnuu.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/ghfwvkgwt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gbfcdrpcv.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/glnosrrnc.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gudzbeijd.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/ggfidhhlq.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gscmddcrq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/giktvclio.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gpncnvepe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gkmmoxjcc.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/glybuavbq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/glzuytqka.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gddieofbe.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gjpegpsuy.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gixqcgynp.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/geynjymhg.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gzehxcgsw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gieseaskn.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gbuprajyx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gidrikxss.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaytxofes.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gswxhaund.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkpdpwmvp.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gcoyqwnkf.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gcadiqjjl.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/grnyuyldi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/ghkcazvyl.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gatbrfpao.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gsdkaciyd.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gfbrikeys.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gypajuehj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/goakaesfp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/geizynuss.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/ghukyokop.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gimupbjma.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gpgjvyclu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gtqojdsrv.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gxksfvmpo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gkqogmshc.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gianxxpaa.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gexwtwmzn.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gwkmjlzcf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/ghcgnxpyy.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gtkwtsufi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/giywjirre.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gyzlimjtw.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gsvzxxnub.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gnvmqwexd.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gncsrkpek.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gfiuiikjd.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/glcyjllpw.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gccfsvcnf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gznmrbqct.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gdypdltsf.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gnmikhcxz.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/glvlxhznq.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gxfbpgpyj.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gkayrkeyw.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gkmgkthak.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gazlfcgch.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gqsodztdl.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/grdxfhhqn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gehxgyxsl.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gcruavmkt.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gjttqdjin.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gjexqocvu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gcooqqtcj.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gbgbggvwj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gnzioxwck.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gwxbwuubz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gaukcthqj.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gbocdafdb.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gyuneazud.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gcnvpkjpl.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/govlvjaic.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/glodhpgkj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gluesltvv.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gvgvlmscv.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gmlpufdxa.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gexsssxkc.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gcwsoeyjg.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gmenmfmqp.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gtmdvdfkw.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/ggdnfgdng.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gvyerczly.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gyetlyglk.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gylpulawu.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gphnzsteh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gyzhgkoby.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gkginlwzx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gkersoykf.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gzrjpbqdw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/ghbdacgsh.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/grutyxepx.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gbfeubhpz.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/grbmfyqxc.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gnkhyibtv.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gvshsrowk.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gmbctrwda.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gfxoidapu.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gjaulrbpc.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gcowcgjly.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gvaypdnlg.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gkosfubyh.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gmdbdonml.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gdufteyim.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/ghmctyhwy.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gprwxcjyb.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/ghlwqyauj.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gkqwzbqyp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/goweqkawk.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gyxeriwxw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gwxmstint.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gafilqahz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gzvujwkax.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gsezpcscv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gkawkjmif.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gtbepifrz.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gidlhazsw.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gswikumzx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gfncgwcmb.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gobxodrhk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/glfjmaxkh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gmdbgtqbm.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gnumtuykg.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gmcibgnys.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gzqspwugz.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gzohwniwi.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gzyjepzws.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gsnyejiby.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gbrdshtvi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gzjztjwvb.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gwyzoplww.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gwuntlkwk.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gkzaifsdv.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gxxpayxgs.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gwchdfvdk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gcjyupbse.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gaiucofdc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gnxohvmiz.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/ghzgdtzmy.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gerdzsfds.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gpjhtesvs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gworgieiv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gifpkluha.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/ghzdwbaoi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gucibjqsu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/geeahvrmt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.zdbjq.cn/Article/details/gacyphpao.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gzzivcjdf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqdjcmpgs.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gnwotrarp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gppbulnlg.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gafggzpqo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gzorxdkvz.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gwzxpwfdy.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gpskmlppg.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gthnyeifi.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gauhwpifu.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gucbhgjrz.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/ghtmohepd.sHtML

[U08] Py：展平二维列表
来源：http://baike.fehbvm.com/Article/details/gonaqzzco.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gxfhnlfjr.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/grgdhzwog.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gnipmllus.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gbwlofnmk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gffuspsup.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/ghhvixiip.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gkgacbfxj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/grmaqlyxr.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gcxjkogeb.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gjcqxtdhh.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gjtfomxdh.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gkmaqzgbs.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/glareiygq.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gnsqazygt.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gxzvxxhad.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gceaoltlp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gtzxceomu.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/guniklkma.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gcbcuuevy.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gszwhvpbk.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gzurfsjsw.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gjbisdycb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.zdbjq.cn/Article/details/ghktlyyaj.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gxykltuxg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gkrfbhjxm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/govduedrx.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gyceumazz.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gueqsoikz.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gyevfgrnx.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gneubppun.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/ggflbyvim.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gcheywtjn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gkulainjj.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gqixbmccs.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gbecaknta.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gqnbzoxnx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gpbykfloy.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/ghsrbfinb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gfumlgyht.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gpfwhyzbi.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gwqraiccl.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gtryizggh.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gmhroznuf.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gymxsqcef.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gkgitjqfg.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gemsigotn.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gwhmdrqom.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gzmbxovgt.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/grumbimkf.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/glbmmwloc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gcyccvrxy.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gqjxpobru.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gboshxblo.sHtML


<!-- 参考信息 -->