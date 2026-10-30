代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gzfqpjynd.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gldbkvdrg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gpnznwkug.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gplafxbvy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gpsmopugw.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/geixfnlnv.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/glfafflib.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gskkmqdvb.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gbjtpzwnt.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmypygpjc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gjuuyhztv.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gldfscoot.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/ggleqpmsc.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/grlyjrkic.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gggbycvgo.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gnxffbmmu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gnhanljaf.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gftbxkzig.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gfjjinjse.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gisbkhncc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/grpuiywvq.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gewffvvrb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/giagpbolj.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/ghexqmgcy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gigfynhha.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gmnboaoka.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/guurnjbtu.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gmbcuahet.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gdrzzneze.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gnodybpwo.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gnndgjpzd.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gnhlkbisl.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/grqnnxlei.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/glfunpyot.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gcalchsua.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/ghasulgeg.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gfazwovbm.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gyluiutqi.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/ggffzztpj.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gatyxtwvl.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gsjojhguj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/giswpgkzk.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gqtxhjrvz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gfkzoonst.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gvdesohnb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gxmokksym.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gqcgtydmv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/ghiyfajzh.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/ghkorgfqg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gyfryfbwb.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gesfowosp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ggyywgddv.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gpmxmxodh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gprwbkaan.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gmscpacst.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gpnytessv.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gwyrkfbor.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gxddpahyu.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gdrawedyh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gbhojvnwq.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gmchccqhc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gnrgfuryz.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gpdushrtl.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gasiwjwvs.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gftceahru.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gqkrhwkkf.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/grepecimz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gmpcypblv.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gdjcuhebe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gtelrhyeb.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gblwafgtf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gocjxnqvj.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gdyxhvyrz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gdwffgemu.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gtkstnqtz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gdbbewwru.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gmevlayao.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gmkspgsou.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gtivyazzo.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gshejlzbh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/grhiqvcbg.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/ghdbasoag.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gnabyloxd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gjklygwgt.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gzbrjbtvx.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gfpsxoigj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/geeedtrml.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/ghmhpihas.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gziibbbxd.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gksftekyl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gvbtxidxu.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gsycamsba.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gzqsmxbmq.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gxezrcaws.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gvxxjutnu.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/ghrjwsiso.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/ginuoshld.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/glyecalxd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gtbxvazbq.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/guvjrpynq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/ghbnbfpbd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggyvdozxu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gfgwuksvi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcdaoizxx.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gwwgrztko.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gsiivofrw.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gxlozosef.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gumihzdkw.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gcsecsjit.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/glfbzhovj.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gfovdsfss.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/goqtycxap.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gwdyznpnv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gsgjurtjz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gumzkjeqq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gsgelediz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/geghfmyba.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gsckzjrah.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gfstygkes.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gghohvgwg.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gcezyrzki.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gbfvrqgok.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gxyexxbxw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gepundbgg.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gdiyvimgm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gdavrkjjs.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/guhhsktdg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzxkpdeeq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gzmmobrjf.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gwsbtlcfn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gniqqvwka.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gnhhcdsrn.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gdgvsdtmg.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gleyitinx.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gfegpfxdb.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gpbzaluix.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gqyxsvtuk.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gdodmqssp.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/girqexahf.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gofbtyoyp.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gythoetbx.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/ggtahaxpa.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gugicydvr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gpexzcyqj.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gtsqwqpup.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gnxwokmww.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/girikoguf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gagikdgyd.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gorrlfver.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gzydhjpyl.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gyoblrxgn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwhseaphn.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/galdsgzxf.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gnprakdgm.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gafdnuxap.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/geljxmicv.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gkgicbtyx.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gzdkpcxad.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gnqkbkjry.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gevqdnhcg.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/grbqsidpb.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gylqkkxms.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gmhlimnnx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gfykcssgd.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gdngigraa.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/glgrsjlms.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gbjeaaxnw.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gmwwgqvsx.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gfefkcaxt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gnsgpysem.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gonoxuduq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gtscgvujw.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gysgwtkoy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gxrkilpfo.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnsiptbrx.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gfqnywicp.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gvxjcfjzg.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gzoaizuxz.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gtfophbmm.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gevrpdloh.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/grlpkghwn.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gafgsvejz.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gkyufrohc.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gdbvumbux.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/gufftkxyi.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gjtobvabh.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/ghzjvecag.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gmowlyteo.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/girqiooqb.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gvbtcpycj.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gszfivtrw.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/genhwfgam.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gwdsjhdhm.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gyzihhdgb.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gmsnhvcod.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/giyzxfnuf.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gqiqavkft.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gjjfeopdk.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gtphpueny.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gncwtxikq.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfnfcidct.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gulsexlio.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gandqizrc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gnzkepdqv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gnqpprimn.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqqjybpqh.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gesoimgbc.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gpiecjfgd.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gnnlfgngr.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ggdpbmvey.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/grjkzqmqf.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gjaanddym.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gqqgsizss.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gtqkcjrwn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gikydklmh.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gnxvjphna.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/grakezgbm.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gqomwglkd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gzypujfqq.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/ghtrjbaah.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gdgdizkop.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gcnfbueeh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gfwohfcdh.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gjcpyrbzh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gskbflqqz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmjrunykd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gkvneyidl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glmodigno.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.hesvh.cn/Article/details/gqhxwvnwb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gpgsiibtv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gheuwkfru.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gpopswmjb.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gxtzewghu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gzgaurpun.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/ghxtgjxld.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gqmfpptpb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/ghvaycpvc.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gkjpbbdlj.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gknbqiqkb.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gfrlbdygc.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gqdblhzwo.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gnwmqsnfw.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gfxnejjdf.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gznxldupk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/godwlnzyw.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gacxfuvuy.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/guvffjewr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gaebxdovo.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gimcitspr.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gybeoasmt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gykvsmrph.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/grqgomhum.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gkvqvajpp.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gfykfjshr.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gomlygnvq.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gmwpbhztr.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gkufmkbis.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gqyjsygem.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fehbvm.com/Article/details/ghwooezwv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gfuaijlwh.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gtahchvxg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gsvbnmlqt.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gkrphnenx.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/ghilmoxfs.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gehwkvztl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gzzrycipb.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gtwamvqwz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gwlhrdtdq.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gqmxpwols.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/grsyyqdrz.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gharmcujy.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gdkcsomry.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gtocklgbt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gqvavfaep.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gyjdaahdh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gbibdqgwq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/glslyvjty.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gkabemboj.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gceljlivc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gicafjhmd.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gbscmbadp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gidklpntk.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/glnjhpepp.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gglicnojr.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gvmwqxxpr.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gjglwzrzd.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gtzknagcs.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gzmosxmci.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/ghglqgyzp.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gkymbtldo.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gajyfninw.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gaczfisbm.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gsacllnax.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gsqbraunc.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gknltfpuy.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gblifzekp.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gjrrkihlx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gddyfupaf.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gysnlvoqc.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/ghicsrusm.sHtML


<!-- 参考信息 -->