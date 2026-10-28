代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.kuanghao11.cn/gtpastmhhl.html

[S10] C：指针与解引用
来源：http://hz.gzhubu.top/gtfjkznovf.html

int *p = &a;  *p = 5;
来源：http://hz.jinyuanbaomall.cn/gtetmaeszw.html

[S11] C：逐行读文件
来源：http://hz.haohaochexian.top/gtlmbwxupt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fengsongda.top/gtonteojju.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ppjwa.cn/gtaspyswzl.html

fclose(f);
来源：http://hz.hammf.cn/gtdkohwpdo.html

[S12] C：写文件
来源：http://hz.shzxlz.cn/gtxudkmibt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.vqdsnc.cn/gtvafnwiqa.html

[S13] C：宏定义
来源：http://hz.zycfv.cn/gtsgnpnpxw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuxming.cn/gtymxnmtru.html

[S14] C：枚举
来源：http://hz.shzxlz.cn/gtbmgxtxrb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.guowangkeji.top/gtzroodmhy.html

[S15] C：类型转换
来源：http://hz.xuanzx.com/gtcfgmodpl.html

(double) a / b
来源：http://hz.cucudq.cn/gtpfmxinrv.html

[S16] C：位操作置位
来源：http://hz.jlsjyb.cn/gtpeiicgmm.html

x |= (1 << 3);
来源：http://hz.fengsongda.top/gtykigwhyc.html

[S17] C：安全拼接字符串
来源：http://hz.zhoulong.xyz/gtngwrgwfy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.iojbl.cn/gthyscuvub.html

[S18] C：命令行参数
来源：http://hz.ybcxt.top/gtifotcedf.html

int main(int argc, char **argv)
来源：http://hz.zhixingplan.top/gtqaywniiw.html

[S19] C：快速排序
来源：http://hz.sufxvd.cn/gtsfzpkjua.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gthcnxneap.html

[S20] C：二分查找
来源：http://hz.hfpthk.cn/gtlmiybdgs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtkznorptz.html

[S21] C：字符类别判断
来源：http://hz.jinqigufen.top/gtpqsakdoh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hfpthk.cn/gtddglxhxj.html

[S22] C：字符串转数字
来源：http://hz.shuidangran.top/gtpslfbugm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cqqwz.cn/gtqjpvccee.html

[S23] C：随机数
来源：http://hz.snrcjt.cn/gtzqscivxp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xinyue.icu/gtkvdrbyqu.html

[S24] C：获取本地时间
来源：http://hz.fzhhl.top/gtetnuazjf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aizwys.cn/gtoduteepd.html

[S25] C：内存拷贝
来源：http://hz.fzhhl.top/gtgaamfdvc.html

memcpy(dst, src, n);
来源：http://hz.chenjidiqi.icu/gtfhgkyksk.html

[S26] C：内存清零
来源：http://hz.birdmap.top/gtkhjnwsvo.html

memset(a, 0, sizeof a);
来源：http://hz.c1oappe.top/gtyemavmvm.html

[S27] C：定义常量
来源：http://hz.meibo888.top/gttvfltzym.html

const double PI = 3.14159;
来源：http://hz.jinyuanbaomall.cn/gtibmxodbf.html

[S28] C：静态变量
来源：http://hz.shangyingyoupin.top/gtkvfhnwgu.html

static int counter = 0;
来源：http://hz.aibaodan.cn/gtvrccfibf.html

[S29] C：变参函数
来源：http://hz.jlsjyb.cn/gtyjaqhfkx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ivvv.top/gtoareuvit.html

[S30] C：头文件保护
来源：http://hz.zhoulong.xyz/gtmgtidyrk.html

#ifndef X_H
来源：http://hz.shanyushiyangtech.top/gtffdzknwn.html

#define X_H
来源：http://hz.shanyushiyangtech.top/gteequiycc.html

#endif
来源：http://hz.gzhubu.top/gtogkbgswp.html

[S31] C++：Hello World
来源：http://hz.jiagoushi.top/gtuiwmqybl.html

#include <iostream>
来源：http://hz.xingfuxueyuan.xyz/gtqmrgzdgj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuetiantiany.cn/gtozzhhdib.html

[S32] C++：字符串
来源：http://hz.nwbrower.top/gttbmypywp.html

std::string s = "hi";  s += "!";
来源：http://hz.pycfn.com/gtdhbxffbf.html

[S33] C++：vector 增删
来源：http://hz.hysaishi.cn/gtppidrpvs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xziqi.cn/gtmnqalecb.html

[S34] C++：遍历 vector
来源：http://hz.shuidangran.top/gtbklxtpty.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nanxinkj.top/gtoqsotvbq.html

[S35] C++：map
来源：http://hz.cashguo.top/gtdkhgjswf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtfmnthonf.html

[S36] C++：unordered_map
来源：http://hz.jqgfzy.top/gtzigayzyh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.kuanghao11.cn/gtggcphcwu.html

[S37] C++：set
来源：http://hz.ywan-chungtsiang.top/gtucqgozbv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangkeji.top/gtagridqhg.html

[S38] C++：排序
来源：http://hz.jinyuanbaomall.cn/gtnxxoigat.html

std::sort(v.begin(), v.end());
来源：http://hz.birdmap.top/gthdfnnvsb.html

[S39] C++：自定义比较器排序
来源：http://hz.smart0.xyz/gtmwdlsznj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.birdmap.top/gtglfkjbmt.html

[S40] C++：查找元素
来源：http://hz.hammf.cn/gtplqpbeqy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.daxiang520.top/gtpixoprmm.html

[S41] C++：类与构造函数
来源：http://hz.havefunace.top/gtrhmrlajf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.vqdsnc.cn/gtbuuiwqur.html

[S42] C++：继承与虚函数
来源：http://hz.sufxvd.cn/gtmghdgdbx.html

class B : public Base { public: void f() override {} };
来源：http://hz.sxryk.cn/gtuumcwmbo.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gtdbssjeav.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhoulong.xyz/gturdgcnsu.html

[S44] C++：引用传参
来源：http://hz.jqgufenzy.top/gttukvxzrp.html

void inc(int &x) { ++x; }
来源：http://hz.pengpengdd.cyou/gtakbsivxt.html

[S45] C++：lambda
来源：http://hz.xuanzx.com/gtumcobcyo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aizwys.cn/gtdjbsaarw.html

[S46] C++：函数模板
来源：http://hz.dashuyun.cn/gthvznocxp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.havefunace.top/gtllgjrnco.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenjidiqi.icu/gthhjtgkhd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sxryk.cn/gtaojrrkpj.html

[S48] C++：逐行读文件
来源：http://hz.shzxlz.cn/gtcymmmwzi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydjk.org.cn/gtejwtwump.html

while (std::getline(in, line)) { }
来源：http://hz.birdmap.top/gtsendzvod.html

[S49] C++：写文件
来源：http://hz.shuidangran.top/gtvtamlmtk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydjk.org.cn/gtdybezabt.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtfpmpfmhc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuanzx.com/gtkjvvzfpw.html

[S51] C++：显式类型转换
来源：http://hz.xuetiantiany.cn/gtkpsvgyvd.html

static_cast<double>(a) / b
来源：http://hz.yj20258888.top/gtvngtiikr.html

[S52] C++：const 与 noexcept
来源：http://hz.gaohongyu789.top/gtcvklxoqq.html

int size() const noexcept { return n_; }
来源：http://hz.shzxlz.cn/gtmdsupzbp.html

[S53] C++：移动语义
来源：http://hz.zhengqikj.top/gtrjqobiwq.html

std::vector<int> w = std::move(v);
来源：http://hz.xuetiantiany.cn/gtnljiqmgf.html

[S54] C++：异常处理
来源：http://hz.jiagoushi.top/gtezjlalsy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jqgfzy.top/gtjzpvfabx.html

[S55] C++：结构化绑定
来源：http://hz.c1oappe.top/gtibibgwah.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.andypj.xyz/gtltgbksoj.html

[S56] C++：optional
来源：http://hz.cucudq.cn/gtdwrfsqsr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgufenzy.top/gtuioxxwxt.html

[S57] C++：编译期常量
来源：http://hz.jianghu66.top/gtahulidzj.html

constexpr int N = 10;
来源：http://hz.zhongyouzk.top/gtodfjdwxv.html

[S58] C++：命名空间
来源：http://hz.ydzc1.top/gtfwjfrutk.html

namespace ns { int f() { return 1; } }
来源：http://hz.smart0.xyz/gthbcckdeo.html

[S59] C++：静态断言
来源：http://hz.xuanzx.com/gtjdkzfehc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.meibo888.top/gtisalzikf.html

[S60] C++：遍历并删除元素
来源：http://hz.gzhubu.top/gtibzczspk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenjidiqi.icu/gtxktopxlu.html

================================================================================
来源：http://hz.zycfv.cn/gtjgvgfdcp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenzaomai.com/gtyydelfyl.html

================================================================================
来源：http://hz.wangdashe.top/gtkqhkpawd.html

[T01] Kotlin：Hello World
来源：http://hz.ydzc1.top/gttridkmxs.html

println("Hello")
来源：http://hz.xuanzx.com/gtlglsqhas.html

[T02] Kotlin：变量
来源：http://hz.jyoumei.cn/gtzyhdbwlh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hongshengwenyu.top/gtwlsrpkcj.html

[T03] Kotlin：字符串模板
来源：http://hz.meibo888.top/gttcqztahr.html

"值: $b"
来源：http://hz.yj202588.top/gtzetrxild.html

[T04] Kotlin：空安全
来源：http://hz.tanke756.top/gtwrtxeuik.html

val n: String? = null;  n?.length
来源：http://hz.yvedp.cn/gtepmngmms.html

[T05] Kotlin：when 表达式
来源：http://hz.zhoulong.xyz/gtlpfbbrro.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.nanxinkj.top/gtxfxvxzcg.html

[T06] Kotlin：集合映射
来源：http://hz.hysaishi.cn/gtxvsyaugq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.havefunace.top/gtjijwkxgl.html

[T07] Kotlin：集合过滤
来源：http://hz.ywan-chungtsiang.top/gtbqpxbigh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gotoacloud.top/gtmabxzoyx.html

[T08] Kotlin：数据类
来源：http://hz.zhaomingkeji.xyz/gtygeynitb.html

data class User(val name: String, val age: Int)
来源：http://hz.havefunace.top/gtbnbpsggt.html

[T09] Kotlin：扩展函数
来源：http://hz.ydjk.org.cn/gtzzarxdxe.html

fun String.exclaim() = this + "!"
来源：http://hz.jiagoushi.top/gtkkfevzoa.html

[T10] Kotlin：默认参数
来源：http://hz.chenjidiqi.icu/gtdkkrhcyv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shanyushiyangkeji.top/gtqyvxepth.html

[T11] Kotlin：协程
来源：http://hz.shuidangran.top/gtuwvvvnhj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.mhx1999.top/gtyacdysmp.html

[T12] Kotlin：解构声明
来源：http://hz.chenjidiqi.icu/gtlzoopfsa.html

val (a, b) = Pair(1, 2)
来源：http://hz.xuetiantiany.cn/gtclcixdpm.html

[T13] Kotlin：只读 Map
来源：http://hz.zhoulong.xyz/gtyrderico.html

val m = mapOf("a" to 1)
来源：http://hz.vqdsnc.cn/gtwlyqeuwo.html

[T14] Kotlin：循环
来源：http://hz.9152youxi.cn/gtizpuwbkf.html

for (i in 1..10) println(i)
来源：http://hz.gaohongyu789.top/gtprydgfzi.html

[T15] Kotlin：接口
来源：http://hz.tanke756.top/gtlmplmace.html

interface Shape { fun area(): Double }
来源：http://hz.hongshengwenyu.top/gtovcxqryw.html

[T16] Swift：Hello World
来源：http://hz.kuanghao11.cn/gtemrjtbeu.html

print("Hello")
来源：http://hz.yj20258888.top/gttfexfzok.html

[T17] Swift：变量与常量
来源：http://hz.cdnleiting.top/gtorpfmdrm.html

var a = 1;  let b = 2
来源：http://hz.ehwqpu.com/gtzrvuolgm.html

[T18] Swift：字符串插值
来源：http://hz.yvedp.cn/gthrfzpubk.html

"值: \(b)"
来源：http://hz.zhaomingkeji.xyz/gtnxbuviom.html

[T19] Swift：可选绑定
来源：http://hz.zhiwuduotai.top/gtaqmtbjsd.html

if let n = opt { print(n) }
来源：http://hz.yvedp.cn/gtseoqpbeo.html

[T20] Swift：数组操作
来源：http://hz.guowangkeji.top/gtwbdrvprf.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.haohaochexian.top/gtzfdhyjxb.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gteypzdign.html

for x in a { print(x) }
来源：http://hz.svipenyu.cn/gtkfgootdf.html

[T22] Swift：字典
来源：http://hz.quarkkingdee.top/gtyuujwdfz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hysaishi.cn/gtfhqlfbmr.html

[T23] Swift：函数
来源：http://hz.shanyushiyangtech.top/gtajfhqtkk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.redwolf501.top/gttpypbzbo.html

[T24] Swift：闭包
来源：http://hz.kuanghao11.cn/gtupkmysev.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shangyingyoupin.top/gtdlclwvgf.html

[T25] Swift：结构体
来源：http://hz.hysaishi.cn/gtrwnaahpm.html

struct P { var x: Int }
来源：http://hz.zhongyouzk.top/gtngskspnu.html

[T26] Swift：类与重写
来源：http://hz.9152youxi.cn/gtsqeunwcc.html

class A: Base { override func f() {} }
来源：http://hz.zhixingplan.top/gtrzcajict.html

[T27] Swift：错误处理
来源：http://hz.xingfuxueyuan.xyz/gtkvwiyreo.html

do { try f() } catch { print(error) }
来源：http://hz.nanxuanxn.top/gtkrbemeqw.html

[T28] Swift：枚举
来源：http://hz.gotoacloud.top/gtydpdghms.html

enum Color { case red, green }
来源：http://hz.jqgufenzy.top/gtsdjxsofk.html

[T29] Swift：guard 提前返回
来源：http://hz.yanxiufei.cn/gtyeorltwy.html

guard let x = opt else { return }
来源：http://hz.hnqzz.top/gtxjevpahi.html

[T30] Swift：协议
来源：http://hz.xingfuxueyuan.xyz/gtgojbscuf.html

protocol Shape { func area() -> Double }
来源：http://hz.shuidangran.top/gtggimsqsz.html

[T31] Lua：Hello World
来源：http://hz.xylfe.cn/gtpzhcflgu.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtvbptutdn.html

[T32] Lua：局部变量
来源：http://hz.pycfn.com/gthdtfkgjb.html

local a = 1
来源：http://hz.feifeiyinyue.top/gtwsocokhd.html

[T33] Lua：表（数组）
来源：http://hz.chenzaomai.com/gtnlzsiwrl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.guannengcc.top/gttgtbjqdr.html

[T34] Lua：遍历表
来源：http://hz.cucudq.cn/gtqlziuoex.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jiagoushi.top/gtxsnjafas.html

[T35] Lua：字典表
来源：http://hz.yueranfly.top/gtbvhhaife.html

local d = { a = 1 };  d.b = 2
来源：http://hz.chenzaomai.com/gtkyakijeh.html

[T36] Lua：函数
来源：http://hz.cqqwz.cn/gtbeotncef.html

function add(a, b) return a + b end
来源：http://hz.316326.xyz/gtfvjqqhcj.html

[T37] Lua：字符串拼接
来源：http://hz.snrcjt.cn/gtpqitstwp.html

"a" .. "b"
来源：http://hz.jqgufenzy.top/gtpgxbnpfv.html

[T38] Lua：条件
来源：http://hz.jlsjyb.cn/gtebuknkgs.html

if x > 0 then print("正") end
来源：http://hz.dianchejie.cn/gtqtctnydm.html

[T39] Lua：模式匹配
来源：http://hz.c1oappe.top/gtszffidhb.html

string.find(s, "%d+")
来源：http://hz.xuetiantiany.cn/gtzhldkxav.html

[T40] Lua：元表
来源：http://hz.havefunace.top/gtorjgsvrn.html

setmetatable({}, { __index = base })
来源：http://hz.guowangkeji.top/gtqbxoksiq.html

[T41] Perl：Hello World
来源：http://hz.9152youxi.cn/gthnygeiww.html

print "Hello\n";
来源：http://hz.chenzaomai.com/gtvkxcggiz.html

[T42] Perl：变量类型
来源：http://hz.fengsongda.top/gtkcscrshe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.fengsongda.top/gthhbzkupm.html

[T43] Perl：字符串插值
来源：http://hz.jiagoushi.top/gtgathwyak.html

"值: $a"
来源：http://hz.zhijiandao.cn/gtbjtzkdon.html

[T44] Perl：条件
来源：http://hz.dashuyun.cn/gtkwlsibeg.html

if ($a > 0) { print "正"; }
来源：http://hz.andypj.xyz/gtopkxgssc.html

[T45] Perl：数组遍历
来源：http://hz.feifeiyinyue.top/gtuyafbtwj.html

for my $x (@arr) { print $x; }
来源：http://hz.tianlin.xyz/gtxfirfhua.html

[T46] Perl：哈希操作
来源：http://hz.cucudq.cn/gtxvlhtbay.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.bjfxy.top/gttigzchlu.html

[T47] Perl：正则捕获
来源：http://hz.yonumen.top/gtmgunhmoz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yongpay.top/gtmgdtydlp.html

[T48] Perl：正则替换
来源：http://hz.xuanzx.com/gtqhxyldxd.html

$s =~ s/old/new/g;
来源：http://hz.guannengcc.top/gtovmqpykr.html

[T49] Perl：函数
来源：http://hz.jinyuanbaomall.cn/gtfnqhsgao.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.iojbl.cn/gtmgnmzcuj.html

[T50] Perl：逐行读文件
来源：http://hz.sweek.top/gtudusbnpk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hfpthk.cn/gtnwbrqhpt.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jqgufenzy.top/gthwmxrror.html

[T51] Scala：Hello World
来源：http://hz.chenjidiqi.icu/gtvczxmngn.html

println("Hello")
来源：http://hz.yuanzhike.top/gtpzabylwa.html

[T52] Scala：变量
来源：http://hz.nanxinkj.top/gtmovsfnrp.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangtech.top/gtdcjnkphk.html

[T53] Scala：字符串插值
来源：http://hz.jianghu66.top/gtwielholn.html

s"值: $b"
来源：http://hz.jinqigufen.top/gthfsuwywy.html

[T54] Scala：集合映射
来源：http://hz.zhoulong.xyz/gtmhtxosnk.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.pengpengdd.cyou/gtckwsmrvn.html

[T55] Scala：集合过滤
来源：http://hz.mhx1999.top/gtobnbqkdb.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jiagoushi.top/gtvgvbhcop.html

[T56] Scala：样例类
来源：http://hz.wangdashe.top/gtsvmrjcoe.html

case class User(name: String, age: Int)
来源：http://hz.jinghuilouyu.cn/gtpeoocazi.html

[T57] Scala：模式匹配
来源：http://hz.mhx1999.top/gtdgwqmyhf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.andypj.xyz/gttpfgvdxu.html

[T58] Scala：函数定义
来源：http://hz.ydzc1.top/gtmnbouabq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.pycfn.com/gtpqhuatko.html

[T59] Scala：循环
来源：http://hz.quarkkingdee.top/gtnwhttfwb.html

for (i <- 1 to 10) println(i)
来源：http://hz.nanxuanxn.top/gtyvufdjgl.html

[T60] Scala：折叠
来源：http://hz.aibaodan.cn/gtssnzwswj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sysykeji.top/gtbmqfzdbb.html

================================================================================
来源：http://hz.daxiang520.top/gtjmzosogg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.aibaodan.cn/gtmnnfmsal.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmotgtlxr.html

[U01] Py：创建虚拟环境
来源：http://hz.havefunace.top/gthpevqmpm.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zycfv.cn/gtkoavdtoi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gzhubu.top/gtihamotod.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gzhubu.top/gtzllssoml.html

[U03] Py：加载 .env 配置
来源：http://hz.feifeiyinyue.top/gtroltdlzg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.yanxiufei.cn/gtpylkltoa.html

[U04] Py：变量调试打印
来源：http://hz.ydjk.org.cn/gtjuamwdqy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yueranfly.top/gtxdlplbfs.html

[U05] Py：列表去重且保序
来源：http://hz.yvedp.cn/gtasekqwho.html

list(dict.fromkeys(arr))
来源：http://hz.xuanzx.com/gttfgvaxjj.html

[U06] Py：合并两个字典
来源：http://hz.shanyushiyangkeji.top/gtyzvifyir.html

{**a, **b}
来源：http://hz.haohaochexian.top/gtgoehulzt.html

[U07] Py：反转字典键值
来源：http://hz.pycfn.com/gtcedavjcr.html

{v: k for k, v in d.items()}
来源：http://hz.yvedp.cn/gtsyzmwinp.html

[U08] Py：展平二维列表
来源：http://hz.feifeiyinyue.top/gtzvkewjsa.html

[y for x in nested for y in x]
来源：http://hz.yanxiufei.cn/gtmrwlgroe.html

[U09] Py：字典取最大值的键
来源：http://hz.guannengcc.top/gtkpibbtuy.html

max(d, key=d.get)
来源：http://hz.gotoacloud.top/gtymwsymna.html

[U10] Py：按值排序字典
来源：http://hz.gzhubu.top/gtxuejcgtv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nanxinkj.top/gtuddpnxah.html

[U11] Py：生成器表达式
来源：http://hz.jinqigfzy.top/gtctutbhkw.html

(x * 2 for x in arr)
来源：http://hz.zdqjudy.top/gtuniuimpd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jianghu66.top/gtussjxqkf.html

Counter(arr).most_common(3)
来源：http://hz.pengpengdd.cyou/gtnqtleuxk.html

[U13] Py：固定长度队列
来源：http://hz.vqdsnc.cn/gtofzokjxt.html

deque(maxlen=10)
来源：http://hz.sysykeji.top/gtouviawmb.html

[U14] Py：分组收集到列表
来源：http://hz.zhengqikj.top/gtmvbausbl.html

defaultdict(list)
来源：http://hz.xziqi.cn/gtewxeovss.html

[U15] Py：高精度计时
来源：http://hz.zhixingplan.top/gtzblktidq.html

t = time.perf_counter()
来源：http://hz.hammf.cn/gtajejljpl.html

[U16] Py：命令行参数解析
来源：http://hz.daria6918.cn/gtgbkyteye.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gaohongyu789.top/gtmwfkwijf.html

[U17] Py：初始化日志
来源：http://hz.sxryk.cn/gtwfctnyoz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shuidangran.top/gtgqmtvrqb.html

[U18] Py：预编译正则
来源：http://hz.sufxvd.cn/gtttrzoxks.html

pat = re.compile(r"\d+")
来源：http://hz.fzhhl.top/gttimxzyvp.html

[U19] Py：正则替换带回调
来源：http://hz.daxiang520.top/gtcwnncflw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.fengsongda.top/gtqpigxwbm.html

[U20] Py：缓存函数结果
来源：http://hz.birdmap.top/gtadgrkzyy.html

@functools.lru_cache(maxsize=None)
来源：http://hz.daxiang520.top/gtzorterbm.html

[U21] Py：自定义上下文管理器
来源：http://hz.aizwys.cn/gttygdebwd.html

@contextlib.contextmanager
来源：http://hz.yongpay.top/gttgxpamup.html

[U22] Py：矩阵转置
来源：http://hz.jinqigufen.top/gtexhztflc.html

list(zip(*m))
来源：http://hz.xingfuxueyuan.xyz/gtxlxfvtho.html

[U23] Py：分块读取大文件
来源：http://hz.vqdsnc.cn/gthhhwifsj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ivvv.top/gtrxstnxmk.html

[U24] Py：路径操作
来源：http://hz.yueranfly.top/gtbarywxjr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhiwuduotai.top/gthuladtmc.html

[U25] Py：CSV 按字典读
来源：http://hz.c1oappe.top/gtwzexvcld.html

csv.DictReader(f)
来源：http://hz.wangshuangyany.cn/gtadzroewj.html

[U26] Py：并发下载
来源：http://hz.fzhhl.top/gtdjdmguzr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.meibo888.top/gtgtgwjbrf.html

[U27] Py：异步 HTTP
来源：http://hz.cdnleiting.top/gtgclfrarq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jianghu66.top/gtdoizecjy.html

[U28] Py：类型别名
来源：http://hz.gogol.net.cn/gtoeilcpno.html

UserId = int
来源：http://hz.xingfuxueyuan.xyz/gtkotutmia.html

[U29] Py：属性校验
来源：http://hz.jiagoushi.top/gtpkickutz.html

@property 与 @x.setter 配合
来源：http://hz.shuidangran.top/gtvctibxnj.html

[U30] Py：数据类
来源：http://hz.jinyuanbaomall.cn/gtrnpyvuzm.html

@dataclass(slots=True)
来源：http://hz.xuanzx.com/gtcuhvjwgo.html

[U31] Py：单测
来源：http://hz.xinyue.icu/gtbbjgoihf.html

python -m pytest -q
来源：http://hz.nanxuanxn.top/gtezmytvdl.html

[U32] Py：代码格式化
来源：http://hz.yuanzhike.top/gterdduyrv.html

ruff format . && ruff check --fix .
来源：http://hz.snrcjt.cn/gtsxedwajo.html


<!-- 参考信息 -->