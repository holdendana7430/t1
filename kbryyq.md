代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aibaodan.cn/gtsmavkfgu.html

[S10] C：指针与解引用
来源：http://hz.ehwqpu.com/gtbytvimkz.html

int *p = &a;  *p = 5;
来源：http://hz.316326.xyz/gttzhzaynz.html

[S11] C：逐行读文件
来源：http://hz.redwolf501.top/gtaekgucut.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gtldkseejn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.0kj1m.cn/gtnjibuwpv.html

fclose(f);
来源：http://hz.c1oappe.top/gtpplmylus.html

[S12] C：写文件
来源：http://hz.vqdsnc.cn/gtrarqkkia.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.redwolf501.top/gtqeebarlz.html

[S13] C：宏定义
来源：http://hz.chenlongwang.top/gtsarpkknx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgufenzy.top/gtmocfqboe.html

[S14] C：枚举
来源：http://hz.aibaodan.cn/gtjhfxabsu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shanyushiyangkeji.top/gtvqxdxjjm.html

[S15] C：类型转换
来源：http://hz.tianlin.xyz/gtgxzfriar.html

(double) a / b
来源：http://hz.zhengqikj.top/gtbvattsnc.html

[S16] C：位操作置位
来源：http://hz.vqdsnc.cn/gtchyepibo.html

x |= (1 << 3);
来源：http://hz.xziqi.cn/gtblyxqqfj.html

[S17] C：安全拼接字符串
来源：http://hz.guowangkeji.top/gtknccmfle.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hongshengwenyu.top/gtjnifgahh.html

[S18] C：命令行参数
来源：http://hz.shanyushiyangkeji.top/gtjibcmrns.html

int main(int argc, char **argv)
来源：http://hz.redwolf501.top/gtulqpjdit.html

[S19] C：快速排序
来源：http://hz.xziqi.cn/gtqaexflai.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shuidangran.top/gtodlaltuw.html

[S20] C：二分查找
来源：http://hz.guowangkeji.top/gtasbyfrsv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.smart0.xyz/gtzrqxrgag.html

[S21] C：字符类别判断
来源：http://hz.gogol.net.cn/gtwxfsbnww.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigfzy.top/gtuznguedx.html

[S22] C：字符串转数字
来源：http://hz.birdmap.top/gtawwwnwtf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yangfankeji.com/gtnegszzch.html

[S23] C：随机数
来源：http://hz.redwolf501.top/gtaowsbwjp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinqigufen.top/gtjvpcgivk.html

[S24] C：获取本地时间
来源：http://hz.zhoulong.xyz/gtgmyarcrk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gotoacloud.top/gteygvcaer.html

[S25] C：内存拷贝
来源：http://hz.shanyushiyangtech.top/gtcqziuslg.html

memcpy(dst, src, n);
来源：http://hz.yangfankeji.com/gtafzfqavk.html

[S26] C：内存清零
来源：http://hz.ywan-chungtsiang.top/gtgfxvvesu.html

memset(a, 0, sizeof a);
来源：http://hz.redwolf501.top/gtesegtgbw.html

[S27] C：定义常量
来源：http://hz.pengpengdd.cyou/gtssgaicct.html

const double PI = 3.14159;
来源：http://hz.yj20258888.top/gtckqseedw.html

[S28] C：静态变量
来源：http://hz.sufxvd.cn/gtsnqhfsku.html

static int counter = 0;
来源：http://hz.zhengqikj.top/gtnzdhinun.html

[S29] C：变参函数
来源：http://hz.zdqjudy.top/gtgekiqpxv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gzhubu.top/gtsgqufcqg.html

[S30] C：头文件保护
来源：http://hz.fzhhl.top/gtztakaelc.html

#ifndef X_H
来源：http://hz.shanyushiyangkeji.top/gtxpojbtwk.html

#define X_H
来源：http://hz.chenlongwang.top/gtjeibvrrs.html

#endif
来源：http://hz.hywenlv.cn/gtjmfkhtjx.html

[S31] C++：Hello World
来源：http://hz.cheryme.top/gtdnefsmmb.html

#include <iostream>
来源：http://hz.ivvv.top/gtvdmsxhjs.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhijiandao.cn/gtisqwrlev.html

[S32] C++：字符串
来源：http://hz.mhx1999.top/gtnfmjhllw.html

std::string s = "hi";  s += "!";
来源：http://hz.hammf.cn/gttzidvnmh.html

[S33] C++：vector 增删
来源：http://hz.jyoumei.cn/gtfnqrcrty.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fzhhl.top/gtdiwtdrar.html

[S34] C++：遍历 vector
来源：http://hz.kuanghao11.cn/gtscufrexs.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yuanzhike.top/gtpakdntak.html

[S35] C++：map
来源：http://hz.zdqjudy.top/gtnclpakqs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gthpsulaii.html

[S36] C++：unordered_map
来源：http://hz.xinyue.icu/gthtzacvxn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shuidangran.top/gtsggjvzlg.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gtjisynmdf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xziqi.cn/gtduwncceu.html

[S38] C++：排序
来源：http://hz.nanxuanxn.top/gtfelbgpaw.html

std::sort(v.begin(), v.end());
来源：http://hz.guannengcc.top/gtkshxgine.html

[S39] C++：自定义比较器排序
来源：http://hz.zdqjudy.top/gtpcicqvmu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hfpthk.cn/gtxrmqeiqq.html

[S40] C++：查找元素
来源：http://hz.zhijiandao.cn/gttaituuot.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hammf.cn/gtuvxtegzb.html

[S41] C++：类与构造函数
来源：http://hz.52xcode.cn/gtullfuazj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shangyingyoupin.top/gtatczvnfr.html

[S42] C++：继承与虚函数
来源：http://hz.316326.xyz/gtofelgqht.html

class B : public Base { public: void f() override {} };
来源：http://hz.zdqjudy.top/gtqwflrghq.html

[S43] C++：智能指针
来源：http://hz.jinqigfzy.top/gtaljrncaj.html

auto p = std::make_unique<int>(5);
来源：http://hz.daria6918.cn/gtlzwsmgjo.html

[S44] C++：引用传参
来源：http://hz.gzhubu.top/gtrfkcgqmz.html

void inc(int &x) { ++x; }
来源：http://hz.andypj.xyz/gtplylgxoi.html

[S45] C++：lambda
来源：http://hz.hfpthk.cn/gttiogrvqr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ehwqpu.com/gtuwpdsqyx.html

[S46] C++：函数模板
来源：http://hz.yangfankeji.com/gtrnzhqmkj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258888.top/gtasuoauky.html

[S47] C++：结构化绑定遍历
来源：http://hz.ywan-chungtsiang.top/gtkddunola.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.52xcode.cn/gtmrdtynrr.html

[S48] C++：逐行读文件
来源：http://hz.chenjidiqi.icu/gtrylrztmm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jlsjyb.cn/gtragrxemj.html

while (std::getline(in, line)) { }
来源：http://hz.daxiang520.top/gtskctbbqd.html

[S49] C++：写文件
来源：http://hz.52xcode.cn/gtruzqomjd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinqigfzy.top/gtomfafqrs.html

[S50] C++：格式化数字
来源：http://hz.hysaishi.cn/gtavikisgb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yonumen.top/gtzgrlevic.html

[S51] C++：显式类型转换
来源：http://hz.9152youxi.cn/gtsypyaocd.html

static_cast<double>(a) / b
来源：http://hz.nanxinkj.top/gtvrocnpqa.html

[S52] C++：const 与 noexcept
来源：http://hz.daria6918.cn/gtzhwvqrpd.html

int size() const noexcept { return n_; }
来源：http://hz.tianlin.xyz/gtzytvemyn.html

[S53] C++：移动语义
来源：http://hz.yj202588.top/gtiinevtor.html

std::vector<int> w = std::move(v);
来源：http://hz.jianghu66.top/gtsyyjsjck.html

[S54] C++：异常处理
来源：http://hz.xuetiantiany.cn/gtxxlhciim.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gogol.net.cn/gtiowksanb.html

[S55] C++：结构化绑定
来源：http://hz.zhixingplan.top/gtjeavcyjl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yanxiufei.cn/gtzbtckqzd.html

[S56] C++：optional
来源：http://hz.gaohongyu789.top/gtdlxgopqk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxinkj.top/gtkstdlxky.html

[S57] C++：编译期常量
来源：http://hz.hywenlv.cn/gtcupcfedl.html

constexpr int N = 10;
来源：http://hz.jqgufenzy.top/gtcyaphzex.html

[S58] C++：命名空间
来源：http://hz.chenlongwang.top/gtqnyaorvl.html

namespace ns { int f() { return 1; } }
来源：http://hz.xziqi.cn/gtfopzwlio.html

[S59] C++：静态断言
来源：http://hz.hammf.cn/gtyoauwsir.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.quarkkingdee.top/gtvwbynnpf.html

[S60] C++：遍历并删除元素
来源：http://hz.nanxuanxn.top/gtkjxvvupi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xziqi.cn/gtdujgkglg.html

================================================================================
来源：http://hz.xuanzx.com/gtelxrrpzs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxuanxn.top/gtbkqlxadl.html

================================================================================
来源：http://hz.svipenyu.cn/gttxvephfp.html

[T01] Kotlin：Hello World
来源：http://hz.daxiang520.top/gtjqvpjkze.html

println("Hello")
来源：http://hz.gotoacloud.top/gtflyirmut.html

[T02] Kotlin：变量
来源：http://hz.chenlongwang.top/gtkbrsczfw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.havefunace.top/gteudcvspy.html

[T03] Kotlin：字符串模板
来源：http://hz.chenjidiqi.icu/gtetcutzfg.html

"值: $b"
来源：http://hz.hfpthk.cn/gtugwlbjhz.html

[T04] Kotlin：空安全
来源：http://hz.meibo888.top/gtlghmyhyf.html

val n: String? = null;  n?.length
来源：http://hz.xuetiantiany.cn/gtvpkneane.html

[T05] Kotlin：when 表达式
来源：http://hz.chenlongwang.top/gtgdaqifuc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hongshengwenyu.top/gtjankhmvx.html

[T06] Kotlin：集合映射
来源：http://hz.cdnleiting.top/gtpuokcjii.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yonumen.top/gtlspwqtel.html

[T07] Kotlin：集合过滤
来源：http://hz.cdnleiting.top/gtqkewaltf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuanzhike.top/gtsartpnld.html

[T08] Kotlin：数据类
来源：http://hz.jyoumei.cn/gtlnaqwdio.html

data class User(val name: String, val age: Int)
来源：http://hz.sufxvd.cn/gtthyishws.html

[T09] Kotlin：扩展函数
来源：http://hz.wangshuangyany.cn/gtspnfhlxw.html

fun String.exclaim() = this + "!"
来源：http://hz.nanxuanxn.top/gtjeeybtky.html

[T10] Kotlin：默认参数
来源：http://hz.0kj1m.cn/gtjumtbsjt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shanyushiyangtech.top/gtqqjbctmr.html

[T11] Kotlin：协程
来源：http://hz.jinghuilouyu.cn/gtmnuwdtrb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xylfe.cn/gtsshgbdrn.html

[T12] Kotlin：解构声明
来源：http://hz.vqdsnc.cn/gttfacdplw.html

val (a, b) = Pair(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtqjeodman.html

[T13] Kotlin：只读 Map
来源：http://hz.cdnleiting.top/gtkqxypkeo.html

val m = mapOf("a" to 1)
来源：http://hz.yonumen.top/gtmtkolrya.html

[T14] Kotlin：循环
来源：http://hz.zhijiandao.cn/gtsixrlwhb.html

for (i in 1..10) println(i)
来源：http://hz.ehwqpu.com/gtdccbvgfg.html

[T15] Kotlin：接口
来源：http://hz.shanyushiyangtech.top/gtkdqqiyjd.html

interface Shape { fun area(): Double }
来源：http://hz.jinqigfzy.top/gtrutdjgwv.html

[T16] Swift：Hello World
来源：http://hz.smart0.xyz/gtxzqjelsr.html

print("Hello")
来源：http://hz.cashguo.top/gtxgkxotib.html

[T17] Swift：变量与常量
来源：http://hz.c1oappe.top/gtmdhtkqow.html

var a = 1;  let b = 2
来源：http://hz.shanyushiyangtech.top/gteyjkccjl.html

[T18] Swift：字符串插值
来源：http://hz.andypj.xyz/gtppqljugk.html

"值: \(b)"
来源：http://hz.aibaodan.cn/gtwqhukbvk.html

[T19] Swift：可选绑定
来源：http://hz.cdnleiting.top/gtszintltf.html

if let n = opt { print(n) }
来源：http://hz.wangdashe.top/gtrkzyaydk.html

[T20] Swift：数组操作
来源：http://hz.zdqjudy.top/gtdpgrifdr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gogol.net.cn/gtisnqwjrj.html

[T21] Swift：遍历
来源：http://hz.mhx1999.top/gthjnhrsqw.html

for x in a { print(x) }
来源：http://hz.fzhhl.top/gtsfcoeeoy.html

[T22] Swift：字典
来源：http://hz.shanyushiyangtech.top/gtfeyefxkz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.pycfn.com/gtgalfiqwr.html

[T23] Swift：函数
来源：http://hz.dianchejie.cn/gtmnnfkfbb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.dashuyun.cn/gtydwocfsj.html

[T24] Swift：闭包
来源：http://hz.nanxinkj.top/gtjvpdvigy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnqzz.top/gtlkjntwwr.html

[T25] Swift：结构体
来源：http://hz.aibaodan.cn/gtfwdohnaq.html

struct P { var x: Int }
来源：http://hz.c1oappe.top/gtcmadlydh.html

[T26] Swift：类与重写
来源：http://hz.shanyushiyangtech.top/gtwqsgteif.html

class A: Base { override func f() {} }
来源：http://hz.birdmap.top/gtznjrsgbw.html

[T27] Swift：错误处理
来源：http://hz.xuanzx.com/gthorwobos.html

do { try f() } catch { print(error) }
来源：http://hz.sysykeji.top/gtnxkjrjet.html

[T28] Swift：枚举
来源：http://hz.wangshuangyany.cn/gtknkazmkv.html

enum Color { case red, green }
来源：http://hz.jyoumei.cn/gtepnwvhxp.html

[T29] Swift：guard 提前返回
来源：http://hz.zhijiandao.cn/gtfgecbyyj.html

guard let x = opt else { return }
来源：http://hz.pengpengdd.cyou/gtopzvetve.html

[T30] Swift：协议
来源：http://hz.fzhhl.top/gtxvxcvvsl.html

protocol Shape { func area() -> Double }
来源：http://hz.dashuyun.cn/gtyinnakou.html

[T31] Lua：Hello World
来源：http://hz.shanyushiyangkeji.top/gtbaqvubgz.html

print("Hello")
来源：http://hz.cheryme.top/gtgamualjs.html

[T32] Lua：局部变量
来源：http://hz.hfpthk.cn/gttuwnbkgb.html

local a = 1
来源：http://hz.0kj1m.cn/gtkoyvbkdz.html

[T33] Lua：表（数组）
来源：http://hz.iojbl.cn/gtiodndnwo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ppjwa.cn/gtubkgjrnk.html

[T34] Lua：遍历表
来源：http://hz.shzxlz.cn/gtamwfvuke.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.bjfxy.top/gtiwnawfsh.html

[T35] Lua：字典表
来源：http://hz.yuanzhike.top/gtxatdosmm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtulfpsviw.html

[T36] Lua：函数
来源：http://hz.vqdsnc.cn/gtmuygdwfh.html

function add(a, b) return a + b end
来源：http://hz.snrcjt.cn/gtuqbzkxkx.html

[T37] Lua：字符串拼接
来源：http://hz.cheryme.top/gtvlwaqxnc.html

"a" .. "b"
来源：http://hz.tianlin.xyz/gtobpxyqlg.html

[T38] Lua：条件
来源：http://hz.cdnleiting.top/gtfzlimpka.html

if x > 0 then print("正") end
来源：http://hz.ydjk.org.cn/gtytisgngi.html

[T39] Lua：模式匹配
来源：http://hz.redwolf501.top/gtampzoblp.html

string.find(s, "%d+")
来源：http://hz.sysykeji.top/gterbfmjyg.html

[T40] Lua：元表
来源：http://hz.zhiwuduotai.top/gtxftafxqw.html

setmetatable({}, { __index = base })
来源：http://hz.yuxming.cn/gtvhsgprat.html

[T41] Perl：Hello World
来源：http://hz.ybcxt.top/gtwvsavmst.html

print "Hello\n";
来源：http://hz.ybcxt.top/gtentccthh.html

[T42] Perl：变量类型
来源：http://hz.xuanzx.com/gtvllcctvh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fengsongda.top/gtrxlhoivm.html

[T43] Perl：字符串插值
来源：http://hz.sufxvd.cn/gtwmdtyqwa.html

"值: $a"
来源：http://hz.jinqigfzy.top/gtpobgxydt.html

[T44] Perl：条件
来源：http://hz.yueranfly.top/gtvayponlv.html

if ($a > 0) { print "正"; }
来源：http://hz.sufxvd.cn/gtloistqxv.html

[T45] Perl：数组遍历
来源：http://hz.chenjidiqi.icu/gtymsrryta.html

for my $x (@arr) { print $x; }
来源：http://hz.cucudq.cn/gtlsskyzby.html

[T46] Perl：哈希操作
来源：http://hz.fengsongda.top/gtsrrrhxyj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.c1oappe.top/gtyssdwqjm.html

[T47] Perl：正则捕获
来源：http://hz.jinqigfzy.top/gtohhhzyrc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.guowangkeji.top/gtbrpgzywp.html

[T48] Perl：正则替换
来源：http://hz.redwolf501.top/gtofzynzpd.html

$s =~ s/old/new/g;
来源：http://hz.xinyue.icu/gtnaljufui.html

[T49] Perl：函数
来源：http://hz.jinqigfzy.top/gtklfituse.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxuanxn.top/gtktfrtsns.html

[T50] Perl：逐行读文件
来源：http://hz.gogol.net.cn/gtavsroldm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hnqzz.top/gtsziftlpx.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hfpthk.cn/gtxqpkjbfq.html

[T51] Scala：Hello World
来源：http://hz.jqgufenzy.top/gtcwappkfc.html

println("Hello")
来源：http://hz.fzhhl.top/gtnjciulfx.html

[T52] Scala：变量
来源：http://hz.tian-w.cn/gtucieiuhx.html

val a = 1;  var b = 2
来源：http://hz.c1oappe.top/gtfnlurjjt.html

[T53] Scala：字符串插值
来源：http://hz.mhx1999.top/gttckcbqyj.html

s"值: $b"
来源：http://hz.nanxuanxn.top/gtbizwzfup.html

[T54] Scala：集合映射
来源：http://hz.gzhubu.top/gtaxnpnbru.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.c1oappe.top/gtfcwimxbk.html

[T55] Scala：集合过滤
来源：http://hz.tian-w.cn/gtxkkvyusp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.fengsongda.top/gtknkfnzvn.html

[T56] Scala：样例类
来源：http://hz.cdnleiting.top/gtsihhtkwi.html

case class User(name: String, age: Int)
来源：http://hz.yj20258888.top/gtzhlaesxf.html

[T57] Scala：模式匹配
来源：http://hz.xuanzx.com/gtymppoozf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.meibo888.top/gtrhufytev.html

[T58] Scala：函数定义
来源：http://hz.yangfankeji.com/gtaqskycot.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.mhx1999.top/gtsqtezodc.html

[T59] Scala：循环
来源：http://hz.wangdashe.top/gthdgnatcw.html

for (i <- 1 to 10) println(i)
来源：http://hz.havefunace.top/gtnqtqwmla.html

[T60] Scala：折叠
来源：http://hz.quarkkingdee.top/gtidkbbfvg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shanyushiyangtech.top/gtronhttpj.html

================================================================================
来源：http://hz.xylfe.cn/gtefadjpjn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtukliqorr.html

================================================================================
来源：http://hz.jyoumei.cn/gtjtnlfsur.html

[U01] Py：创建虚拟环境
来源：http://hz.chenjidiqi.icu/gtszhgszqa.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.wangshuangyany.cn/gtscojeuxj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.pycfn.com/gtmgimdqlg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.zhoulong.xyz/gtymlodaka.html

[U03] Py：加载 .env 配置
来源：http://hz.316326.xyz/gtzfbxjsbc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ywan-chungtsiang.top/gtdbynnuua.html

[U04] Py：变量调试打印
来源：http://hz.cheryme.top/gtfrdybslx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hfpthk.cn/gtpfiebhtt.html

[U05] Py：列表去重且保序
来源：http://hz.jqgufenzy.top/gtgzytqrqb.html

list(dict.fromkeys(arr))
来源：http://hz.fengsongda.top/gtlweweotp.html

[U06] Py：合并两个字典
来源：http://hz.birdmap.top/gtnquergkr.html

{**a, **b}
来源：http://hz.wangdashe.top/gtgtacspom.html

[U07] Py：反转字典键值
来源：http://hz.ydzc1.top/gtlshcsqvd.html

{v: k for k, v in d.items()}
来源：http://hz.yj20258888.top/gtvpuepxyw.html

[U08] Py：展平二维列表
来源：http://hz.dashuyun.cn/gtxzpxhndu.html

[y for x in nested for y in x]
来源：http://hz.hnxiangtu.top/gtekxdpgse.html

[U09] Py：字典取最大值的键
来源：http://hz.wangdashe.top/gtvjpvocaf.html

max(d, key=d.get)
来源：http://hz.fzhhl.top/gtrwjgueyp.html

[U10] Py：按值排序字典
来源：http://hz.yongpay.top/gtyltvsnin.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.0kj1m.cn/gtaqxjwvco.html

[U11] Py：生成器表达式
来源：http://hz.chenlongwang.top/gtimuucaav.html

(x * 2 for x in arr)
来源：http://hz.wangshuangyany.cn/gtsjbxtvdr.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yuxming.cn/gtzqkwxmab.html

Counter(arr).most_common(3)
来源：http://hz.guowangkeji.top/gtoylrikhg.html

[U13] Py：固定长度队列
来源：http://hz.hnqzz.top/gtnhblixyb.html

deque(maxlen=10)
来源：http://hz.zhaomingkeji.xyz/gtbmugmzjb.html

[U14] Py：分组收集到列表
来源：http://hz.0kj1m.cn/gtgzpqjhea.html

defaultdict(list)
来源：http://hz.gaohongyu789.top/gtxdofkzzr.html

[U15] Py：高精度计时
来源：http://hz.birdmap.top/gtrksurxio.html

t = time.perf_counter()
来源：http://hz.hysaishi.cn/gtahsxqygm.html

[U16] Py：命令行参数解析
来源：http://hz.yj202588.top/gtowjwrpxu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gotoacloud.top/gtympejxbe.html

[U17] Py：初始化日志
来源：http://hz.svipenyu.cn/gtfxtjljpu.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jiagoushi.top/gtatoshpjv.html

[U18] Py：预编译正则
来源：http://hz.daxiang520.top/gtftkaugzx.html

pat = re.compile(r"\d+")
来源：http://hz.yj20258888.top/gtpuwqemxm.html

[U19] Py：正则替换带回调
来源：http://hz.shzxlz.cn/gtyvbbtndf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.vqdsnc.cn/gtgafehspg.html

[U20] Py：缓存函数结果
来源：http://hz.wangdashe.top/gtaeukwhbr.html

@functools.lru_cache(maxsize=None)
来源：http://hz.snrcjt.cn/gttdqgzpgs.html

[U21] Py：自定义上下文管理器
来源：http://hz.hongshengwenyu.top/gtbjpidzug.html

@contextlib.contextmanager
来源：http://hz.ybcxt.top/gtxejhsran.html

[U22] Py：矩阵转置
来源：http://hz.wangdashe.top/gtoxcpxyei.html

list(zip(*m))
来源：http://hz.shangyingyoupin.top/gtyvoimkcx.html

[U23] Py：分块读取大文件
来源：http://hz.yueranfly.top/gtpfxexesa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.nanxinkj.top/gtxstlckwo.html

[U24] Py：路径操作
来源：http://hz.9152youxi.cn/gtcnvflpll.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xziqi.cn/gtafzfbclm.html

[U25] Py：CSV 按字典读
来源：http://hz.cucudq.cn/gtvlqatnxc.html

csv.DictReader(f)
来源：http://hz.9152youxi.cn/gtxeygoqfw.html

[U26] Py：并发下载
来源：http://hz.sysykeji.top/gtubgboohh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xingfuxueyuan.xyz/gtvwdnyohz.html

[U27] Py：异步 HTTP
来源：http://hz.ivvv.top/gtpfohmtdu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shanyushiyangtech.top/gtntfpmika.html

[U28] Py：类型别名
来源：http://hz.meibo888.top/gtdwlcawjh.html

UserId = int
来源：http://hz.pengpengdd.cyou/gtvgkyadzl.html

[U29] Py：属性校验
来源：http://hz.zhoulong.xyz/gtohijxnia.html

@property 与 @x.setter 配合
来源：http://hz.feifeiyinyue.top/gtmxztdmzx.html

[U30] Py：数据类
来源：http://hz.nanxinkj.top/gtdhmwvvdj.html

@dataclass(slots=True)
来源：http://hz.iojbl.cn/gtonaehqmi.html

[U31] Py：单测
来源：http://hz.xylfe.cn/gtognfwrom.html

python -m pytest -q
来源：http://hz.chenlongwang.top/gtmabdsrsi.html

[U32] Py：代码格式化
来源：http://hz.sxryk.cn/gtnlzbkevj.html

ruff format . && ruff check --fix .
来源：http://hz.chenzaomai.com/gtfkzdpequ.html


<!-- 参考信息 -->