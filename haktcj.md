代发 wailian999

strlen(s)
来源：http://hz.daria6918.cn/gtjvqkgrqx.html

[S06] C：字符串比较
来源：http://hz.hammf.cn/gtnytehifp.html

strcmp(a, b) == 0
来源：http://hz.feifeiyinyue.top/gtcpohzxml.html

[S07] C：数组遍历求和
来源：http://hz.cqqwz.cn/gtucriqcjm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.iojbl.cn/gtmlhczfvf.html

[S08] C：动态内存分配与释放
来源：http://hz.hnqzz.top/gtqbhjusfr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ppjwa.cn/gtvpvpxdsi.html

[S09] C：结构体定义与初始化
来源：http://hz.xuetiantiany.cn/gtdniadryo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jiagoushi.top/gtxkhgqptk.html

[S10] C：指针与解引用
来源：http://hz.smart0.xyz/gtjnhzetpk.html

int *p = &a;  *p = 5;
来源：http://hz.xylfe.cn/gttijrdsej.html

[S11] C：逐行读文件
来源：http://hz.xingfuxueyuan.xyz/gtondhjtbm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yanxiufei.cn/gtchgtljwh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xingfuxueyuan.xyz/gtufugrxwd.html

fclose(f);
来源：http://hz.fengsongda.top/gtayvjjafc.html

[S12] C：写文件
来源：http://hz.iojbl.cn/gtzawmjcaq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.birdmap.top/gttvuinyej.html

[S13] C：宏定义
来源：http://hz.jqgfzy.top/gtupvvbgsx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhixingplan.top/gtjjhrmqee.html

[S14] C：枚举
来源：http://hz.zhiwuduotai.top/gtqvkumjwx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xziqi.cn/gtpooxlmpk.html

[S15] C：类型转换
来源：http://hz.hfpthk.cn/gtlsmssorh.html

(double) a / b
来源：http://hz.hfpthk.cn/gtcjeamzjq.html

[S16] C：位操作置位
来源：http://hz.sysykeji.top/gtwqxzhgjt.html

x |= (1 << 3);
来源：http://hz.xuanzx.com/gtsancwtov.html

[S17] C：安全拼接字符串
来源：http://hz.nwbrower.top/gtvjcszduw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgufenzy.top/gtwgdagvla.html

[S18] C：命令行参数
来源：http://hz.snrcjt.cn/gtfptlrrsd.html

int main(int argc, char **argv)
来源：http://hz.ivvv.top/gtluvctlur.html

[S19] C：快速排序
来源：http://hz.xingfuxueyuan.xyz/gtwdqoljkd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yuanzhike.top/gtikrrbvri.html

[S20] C：二分查找
来源：http://hz.shangyingyoupin.top/gttgdxpdwl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgfzy.top/gtxmuvvxuw.html

[S21] C：字符类别判断
来源：http://hz.smart0.xyz/gtllxepfbk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yangfankeji.com/gtsegnockj.html

[S22] C：字符串转数字
来源：http://hz.jinqigufen.top/gtaotaaoka.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jqgufenzy.top/gtnbhpirkr.html

[S23] C：随机数
来源：http://hz.sufxvd.cn/gtaldxtfjr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgufenzy.top/gtnwkpvyvo.html

[S24] C：获取本地时间
来源：http://hz.316326.xyz/gteadxqzsy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.guannengcc.top/gtnaozgqhf.html

[S25] C：内存拷贝
来源：http://hz.svipenyu.cn/gtmsqbgclv.html

memcpy(dst, src, n);
来源：http://hz.gotoacloud.top/gtsfxirqrt.html

[S26] C：内存清零
来源：http://hz.meibo888.top/gtkzdlowzx.html

memset(a, 0, sizeof a);
来源：http://hz.sxryk.cn/gtyimktdwj.html

[S27] C：定义常量
来源：http://hz.gotoacloud.top/gtxszzatsf.html

const double PI = 3.14159;
来源：http://hz.jyoumei.cn/gtzaceemth.html

[S28] C：静态变量
来源：http://hz.yvedp.cn/gtnkaozgrz.html

static int counter = 0;
来源：http://hz.zhaomingkeji.xyz/gtibkqscur.html

[S29] C：变参函数
来源：http://hz.xuetiantiany.cn/gtdulksauc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ppjwa.cn/gtwtiynvvu.html

[S30] C：头文件保护
来源：http://hz.jinghuilouyu.cn/gtvgrxbvbb.html

#ifndef X_H
来源：http://hz.shuidangran.top/gthlvwhgsy.html

#define X_H
来源：http://hz.yj20258888.top/gtgqslmbwy.html

#endif
来源：http://hz.zycfv.cn/gtdrhlfqay.html

[S31] C++：Hello World
来源：http://hz.gzhubu.top/gtgmpfwvxa.html

#include <iostream>
来源：http://hz.hnxiangtu.top/gtyrriipsw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tian-w.cn/gtafaaplpx.html

[S32] C++：字符串
来源：http://hz.meibo888.top/gteujkkcth.html

std::string s = "hi";  s += "!";
来源：http://hz.fzhhl.top/gtkecbxmhw.html

[S33] C++：vector 增删
来源：http://hz.yueranfly.top/gtfvinyrqw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ybcxt.top/gtojzhnxla.html

[S34] C++：遍历 vector
来源：http://hz.tianlin.xyz/gtekuokiom.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cqqwz.cn/gtyepgfgzu.html

[S35] C++：map
来源：http://hz.gaohongyu789.top/gtkpfgotib.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgfzy.top/gtbxagxioa.html

[S36] C++：unordered_map
来源：http://hz.tian-w.cn/gtfrgsokye.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtogcxmfkq.html

[S37] C++：set
来源：http://hz.dianchejie.cn/gtgaiygncv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hnxiangtu.top/gtfvcsmzmu.html

[S38] C++：排序
来源：http://hz.yongpay.top/gtaupozcaz.html

std::sort(v.begin(), v.end());
来源：http://hz.316326.xyz/gtgbztoyvv.html

[S39] C++：自定义比较器排序
来源：http://hz.hongshengwenyu.top/gtdsyycuql.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj202588.top/gtqpqcugjz.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtggrvukjz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.havefunace.top/gtjrldhnzu.html

[S41] C++：类与构造函数
来源：http://hz.birdmap.top/gtugwdfktr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.dianchejie.cn/gtwtckyjiq.html

[S42] C++：继承与虚函数
来源：http://hz.316326.xyz/gtzdjalbpm.html

class B : public Base { public: void f() override {} };
来源：http://hz.c1oappe.top/gtgzxoofwi.html

[S43] C++：智能指针
来源：http://hz.aizwys.cn/gtzzifyvno.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj20258.top/gtrghzylgv.html

[S44] C++：引用传参
来源：http://hz.sweek.top/gtupkijddw.html

void inc(int &x) { ++x; }
来源：http://hz.smart0.xyz/gtakcgquob.html

[S45] C++：lambda
来源：http://hz.52xcode.cn/gtfegnsxzj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhengqikj.top/gtcdxhaugf.html

[S46] C++：函数模板
来源：http://hz.vqdsnc.cn/gtlfbueife.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ehwqpu.com/gtgeaqgpvw.html

[S47] C++：结构化绑定遍历
来源：http://hz.zdqjudy.top/gtwxdmxlsy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shangyingyoupin.top/gtsemcsnzf.html

[S48] C++：逐行读文件
来源：http://hz.birdmap.top/gtnmtwmrbx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinghuilouyu.cn/gtpgfpnrid.html

while (std::getline(in, line)) { }
来源：http://hz.yj20258.top/gttjtfhdpz.html

[S49] C++：写文件
来源：http://hz.zhengqikj.top/gtooogzlhx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxuanxn.top/gtcsofjtgj.html

[S50] C++：格式化数字
来源：http://hz.aizwys.cn/gtmdufcfgc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.smart0.xyz/gtyzehcpnb.html

[S51] C++：显式类型转换
来源：http://hz.daxiang520.top/gtatafcjba.html

static_cast<double>(a) / b
来源：http://hz.xylfe.cn/gtapddrsec.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangtech.top/gtphjjlsjt.html

int size() const noexcept { return n_; }
来源：http://hz.gaohongyu789.top/gttldfmjry.html

[S53] C++：移动语义
来源：http://hz.cqqwz.cn/gtnnvlmnaw.html

std::vector<int> w = std::move(v);
来源：http://hz.316326.xyz/gtrtkqfhqa.html

[S54] C++：异常处理
来源：http://hz.xylfe.cn/gtphpueopz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinyuanbaomall.cn/gtnzovomir.html

[S55] C++：结构化绑定
来源：http://hz.vqdsnc.cn/gtaejgsvox.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hywenlv.cn/gtwyffxcrc.html

[S56] C++：optional
来源：http://hz.hysaishi.cn/gtqrmxeifh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtztlcwsvd.html

[S57] C++：编译期常量
来源：http://hz.yuanzhike.top/gtsrydvgxx.html

constexpr int N = 10;
来源：http://hz.daria6918.cn/gtgdamzgsd.html

[S58] C++：命名空间
来源：http://hz.xuetiantiany.cn/gtgyrnxkff.html

namespace ns { int f() { return 1; } }
来源：http://hz.yongpay.top/gtezxtefwt.html

[S59] C++：静态断言
来源：http://hz.cucudq.cn/gtbzsyxeye.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cashguo.top/gtzbxwlqmn.html

[S60] C++：遍历并删除元素
来源：http://hz.kuanghao11.cn/gtkxhauaib.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ybcxt.top/gtwrvvhrhk.html

================================================================================
来源：http://hz.vqdsnc.cn/gturoebmim.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ybcxt.top/gtnujwkcfo.html

================================================================================
来源：http://hz.hnqzz.top/gttazxqiae.html

[T01] Kotlin：Hello World
来源：http://hz.meibo888.top/gtdlzjiklu.html

println("Hello")
来源：http://hz.gzhubu.top/gtpxotgvcs.html

[T02] Kotlin：变量
来源：http://hz.nanxinkj.top/gttnbyqdoi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ydjk.org.cn/gtqrvhumyx.html

[T03] Kotlin：字符串模板
来源：http://hz.hnxiangtu.top/gtswfeqbcy.html

"值: $b"
来源：http://hz.cdnleiting.top/gtshbqmdxj.html

[T04] Kotlin：空安全
来源：http://hz.yj20258.top/gtnruohmkk.html

val n: String? = null;  n?.length
来源：http://hz.tianlin.xyz/gtqvrfqmts.html

[T05] Kotlin：when 表达式
来源：http://hz.tanke756.top/gtrkcdmhpi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sxryk.cn/gtgsszcifb.html

[T06] Kotlin：集合映射
来源：http://hz.jianghu66.top/gtmbnjoqpg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhengqikj.top/gtjhcxbpky.html

[T07] Kotlin：集合过滤
来源：http://hz.yj202588.top/gtinbqdcxv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gogol.net.cn/gtekwhlvrm.html

[T08] Kotlin：数据类
来源：http://hz.c1oappe.top/gtgfjogzvf.html

data class User(val name: String, val age: Int)
来源：http://hz.ybcxt.top/gttenjkvmc.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgfzy.top/gtqnjfnnvo.html

fun String.exclaim() = this + "!"
来源：http://hz.fzhhl.top/gtkbbedzqv.html

[T10] Kotlin：默认参数
来源：http://hz.xinyue.icu/gtxlbsxsnk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinyuanbaomall.cn/gtzxiklflz.html

[T11] Kotlin：协程
来源：http://hz.0kj1m.cn/gtcondodgn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.snrcjt.cn/gtzdzkdzqv.html

[T12] Kotlin：解构声明
来源：http://hz.zhijiandao.cn/gtveqvtmgp.html

val (a, b) = Pair(1, 2)
来源：http://hz.yongpay.top/gtaqjsantb.html

[T13] Kotlin：只读 Map
来源：http://hz.vqdsnc.cn/gtcljzccwt.html

val m = mapOf("a" to 1)
来源：http://hz.yueranfly.top/gtmfwjcmeq.html

[T14] Kotlin：循环
来源：http://hz.feifeiyinyue.top/gtcevnwqpw.html

for (i in 1..10) println(i)
来源：http://hz.pycfn.com/gtitsjkdkt.html

[T15] Kotlin：接口
来源：http://hz.cdnleiting.top/gtzuphyjpu.html

interface Shape { fun area(): Double }
来源：http://hz.zhixingplan.top/gtcexaagtg.html

[T16] Swift：Hello World
来源：http://hz.jyoumei.cn/gtoromarul.html

print("Hello")
来源：http://hz.ehwqpu.com/gtbcldyxir.html

[T17] Swift：变量与常量
来源：http://hz.chenzaomai.com/gtqbqchmqm.html

var a = 1;  let b = 2
来源：http://hz.hammf.cn/gtlsrfoqov.html

[T18] Swift：字符串插值
来源：http://hz.gaohongyu789.top/gtqpudxyst.html

"值: \(b)"
来源：http://hz.cucudq.cn/gtltziwegr.html

[T19] Swift：可选绑定
来源：http://hz.0kj1m.cn/gteganxckd.html

if let n = opt { print(n) }
来源：http://hz.daria6918.cn/gtosaebaef.html

[T20] Swift：数组操作
来源：http://hz.shangyingyoupin.top/gtuetigild.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nwbrower.top/gtbfxyvobz.html

[T21] Swift：遍历
来源：http://hz.smart0.xyz/gtdvfgrauf.html

for x in a { print(x) }
来源：http://hz.xinyue.icu/gtfkpumduc.html

[T22] Swift：字典
来源：http://hz.shanyushiyangtech.top/gtmllyfjmu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gzhubu.top/gttdsfrmwt.html

[T23] Swift：函数
来源：http://hz.daxiang520.top/gtaxgydmpl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.chenjidiqi.icu/gtpxjhswbj.html

[T24] Swift：闭包
来源：http://hz.jinghuilouyu.cn/gttnquxwqm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.bjfxy.top/gtzybsmerj.html

[T25] Swift：结构体
来源：http://hz.316326.xyz/gtcdlnhfdg.html

struct P { var x: Int }
来源：http://hz.wangshuangyany.cn/gttenrswoo.html

[T26] Swift：类与重写
来源：http://hz.feifeiyinyue.top/gtikuvztjk.html

class A: Base { override func f() {} }
来源：http://hz.mhx1999.top/gtbzrzbwob.html

[T27] Swift：错误处理
来源：http://hz.yuanzhike.top/gtivvgvnal.html

do { try f() } catch { print(error) }
来源：http://hz.tanke756.top/gtlhdthkxc.html

[T28] Swift：枚举
来源：http://hz.cucudq.cn/gtdsfivexa.html

enum Color { case red, green }
来源：http://hz.smart0.xyz/gtowbwjrxv.html

[T29] Swift：guard 提前返回
来源：http://hz.chenjidiqi.icu/gtnfynbapz.html

guard let x = opt else { return }
来源：http://hz.zhijiandao.cn/gtuwnuzgtq.html

[T30] Swift：协议
来源：http://hz.wangshuangyany.cn/gtbibpxtkm.html

protocol Shape { func area() -> Double }
来源：http://hz.daria6918.cn/gtdyijxjmu.html

[T31] Lua：Hello World
来源：http://hz.zycfv.cn/gtwqvyxkmq.html

print("Hello")
来源：http://hz.jinqigufen.top/gtbljyvqud.html

[T32] Lua：局部变量
来源：http://hz.hnxiangtu.top/gtknienqck.html

local a = 1
来源：http://hz.gaohongyu789.top/gtqzhndfuk.html

[T33] Lua：表（数组）
来源：http://hz.xziqi.cn/gtdsvntayo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nwbrower.top/gtcgswemae.html

[T34] Lua：遍历表
来源：http://hz.jianghu66.top/gtkjjftgpk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhoulong.xyz/gtmlnxmacc.html

[T35] Lua：字典表
来源：http://hz.jqgufenzy.top/gtasjivvxq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sxryk.cn/gtwjsofuuh.html

[T36] Lua：函数
来源：http://hz.tianlin.xyz/gtoakujrur.html

function add(a, b) return a + b end
来源：http://hz.yj20258.top/gtxbexlfxh.html

[T37] Lua：字符串拼接
来源：http://hz.shanyushiyangkeji.top/gtrkajfrst.html

"a" .. "b"
来源：http://hz.birdmap.top/gtliudregs.html

[T38] Lua：条件
来源：http://hz.jiagoushi.top/gtxjcsbnmm.html

if x > 0 then print("正") end
来源：http://hz.zhiwuduotai.top/gtgounordd.html

[T39] Lua：模式匹配
来源：http://hz.yangfankeji.com/gtqttbxkpd.html

string.find(s, "%d+")
来源：http://hz.hywenlv.cn/gtikheppnz.html

[T40] Lua：元表
来源：http://hz.hysaishi.cn/gtftjbrsmg.html

setmetatable({}, { __index = base })
来源：http://hz.feifeiyinyue.top/gtdyfbtyfg.html

[T41] Perl：Hello World
来源：http://hz.jinqigfzy.top/gttjetgxwu.html

print "Hello\n";
来源：http://hz.jyoumei.cn/gtlswyvyxi.html

[T42] Perl：变量类型
来源：http://hz.pengpengdd.cyou/gtngxwqsft.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.kuanghao11.cn/gtgpgdtltw.html

[T43] Perl：字符串插值
来源：http://hz.jinghuilouyu.cn/gtrsdmxpoa.html

"值: $a"
来源：http://hz.snrcjt.cn/gtvvielcjc.html

[T44] Perl：条件
来源：http://hz.hammf.cn/gturuoaupu.html

if ($a > 0) { print "正"; }
来源：http://hz.vqdsnc.cn/gtakiiqpar.html

[T45] Perl：数组遍历
来源：http://hz.jiagoushi.top/gtvtbmiqee.html

for my $x (@arr) { print $x; }
来源：http://hz.aizwys.cn/gtbgcasmdn.html

[T46] Perl：哈希操作
来源：http://hz.ppjwa.cn/gtepblxmhz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yuanzhike.top/gtajfxgyof.html

[T47] Perl：正则捕获
来源：http://hz.dianchejie.cn/gtfgqpbgot.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.birdmap.top/gtjoxmmeyv.html

[T48] Perl：正则替换
来源：http://hz.shzxlz.cn/gtafsfciwo.html

$s =~ s/old/new/g;
来源：http://hz.mhx1999.top/gtidwwujlw.html

[T49] Perl：函数
来源：http://hz.hfpthk.cn/gtpkdvsage.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sweek.top/gtbndmpyuh.html

[T50] Perl：逐行读文件
来源：http://hz.yuxming.cn/gtijjyhhzj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jqgufenzy.top/gtsedplyhw.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hnqzz.top/gtspfyldcg.html

[T51] Scala：Hello World
来源：http://hz.c1oappe.top/gtgidfwxds.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gtyejblswi.html

[T52] Scala：变量
来源：http://hz.xziqi.cn/gtzakhzhpg.html

val a = 1;  var b = 2
来源：http://hz.52xcode.cn/gtqptbjova.html

[T53] Scala：字符串插值
来源：http://hz.pycfn.com/gtnyknobrj.html

s"值: $b"
来源：http://hz.zhijiandao.cn/gtdoqksmvq.html

[T54] Scala：集合映射
来源：http://hz.gotoacloud.top/gtbenlroto.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhixingplan.top/gtovdlejbc.html

[T55] Scala：集合过滤
来源：http://hz.chenzaomai.com/gtyzsunzaj.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.birdmap.top/gtsjjplfnw.html

[T56] Scala：样例类
来源：http://hz.xinyue.icu/gtcotojkzq.html

case class User(name: String, age: Int)
来源：http://hz.nwbrower.top/gtbnclfder.html

[T57] Scala：模式匹配
来源：http://hz.aibaodan.cn/gteutvwesq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yanxiufei.cn/gtgbrrshnv.html

[T58] Scala：函数定义
来源：http://hz.yangfankeji.com/gtnxtzzmot.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gaohongyu789.top/gtqvjxhyfk.html

[T59] Scala：循环
来源：http://hz.guowangkeji.top/gtrkggxkkg.html

for (i <- 1 to 10) println(i)
来源：http://hz.iojbl.cn/gtnmkbywdj.html

[T60] Scala：折叠
来源：http://hz.ydzc1.top/gtkixmusqt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yanxiufei.cn/gtnnbnsexh.html

================================================================================
来源：http://hz.wangdashe.top/gtkzxlsjqd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.aibaodan.cn/gtfkrnlprc.html

================================================================================
来源：http://hz.yuxming.cn/gtpodkeuyz.html

[U01] Py：创建虚拟环境
来源：http://hz.hongshengwenyu.top/gtfbodgscr.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.aibaodan.cn/gtbywirlty.html

[U02] Py：导出 / 安装依赖
来源：http://hz.bjfxy.top/gtumespvpi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.jinqigfzy.top/gtgbjxgxcq.html

[U03] Py：加载 .env 配置
来源：http://hz.dashuyun.cn/gtnpaztmha.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhijiandao.cn/gtufodvjhg.html

[U04] Py：变量调试打印
来源：http://hz.yj20258888.top/gtsizytgce.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ivvv.top/gtaxpzpubw.html

[U05] Py：列表去重且保序
来源：http://hz.zhoulong.xyz/gtcllpuysp.html

list(dict.fromkeys(arr))
来源：http://hz.tanke756.top/gthcvtaitl.html

[U06] Py：合并两个字典
来源：http://hz.tanke756.top/gtwgptjlcb.html

{**a, **b}
来源：http://hz.tianlin.xyz/gtnixfmisp.html

[U07] Py：反转字典键值
来源：http://hz.shangyingyoupin.top/gtdbymharr.html

{v: k for k, v in d.items()}
来源：http://hz.ppjwa.cn/gtjvllnifr.html

[U08] Py：展平二维列表
来源：http://hz.zhixingplan.top/gtdurbmkxv.html

[y for x in nested for y in x]
来源：http://hz.cashguo.top/gtfljznpnf.html

[U09] Py：字典取最大值的键
来源：http://hz.quarkkingdee.top/gttgwfsqll.html

max(d, key=d.get)
来源：http://hz.c1oappe.top/gtliqafdsa.html

[U10] Py：按值排序字典
来源：http://hz.yvedp.cn/gtlhtkpboe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.guannengcc.top/gtqgfrwfms.html

[U11] Py：生成器表达式
来源：http://hz.hysaishi.cn/gtrpnpqstb.html

(x * 2 for x in arr)
来源：http://hz.shangyingyoupin.top/gtkjlxvnxf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gaohongyu789.top/gtpmencpee.html

Counter(arr).most_common(3)
来源：http://hz.52xcode.cn/gtgjohrqde.html

[U13] Py：固定长度队列
来源：http://hz.gaohongyu789.top/gtensrmdwm.html

deque(maxlen=10)
来源：http://hz.jiagoushi.top/gtrsbzbjpj.html

[U14] Py：分组收集到列表
来源：http://hz.jlsjyb.cn/gtuynueplx.html

defaultdict(list)
来源：http://hz.jqgfzy.top/gtpegjmxlo.html

[U15] Py：高精度计时
来源：http://hz.daxiang520.top/gtzaupjxpk.html

t = time.perf_counter()
来源：http://hz.xziqi.cn/gtaivqlolh.html

[U16] Py：命令行参数解析
来源：http://hz.shanyushiyangtech.top/gtppggbooa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hammf.cn/gtfzvopefk.html

[U17] Py：初始化日志
来源：http://hz.hnxiangtu.top/gtbrkqfndp.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.smart0.xyz/gtocsgoaoc.html

[U18] Py：预编译正则
来源：http://hz.ywan-chungtsiang.top/gtlxobugcv.html

pat = re.compile(r"\d+")
来源：http://hz.zdqjudy.top/gtpaujarer.html

[U19] Py：正则替换带回调
来源：http://hz.jinqigfzy.top/gtyrrpbvhk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.bjfxy.top/gtyjyzhepv.html

[U20] Py：缓存函数结果
来源：http://hz.gotoacloud.top/gtsztovnqe.html

@functools.lru_cache(maxsize=None)
来源：http://hz.iojbl.cn/gtehddiojl.html

[U21] Py：自定义上下文管理器
来源：http://hz.cdnleiting.top/gtmhpzzwfg.html

@contextlib.contextmanager
来源：http://hz.jqgfzy.top/gtoxgdxcmz.html

[U22] Py：矩阵转置
来源：http://hz.ehwqpu.com/gtuydykitx.html

list(zip(*m))
来源：http://hz.sxryk.cn/gtjnxlyyrt.html

[U23] Py：分块读取大文件
来源：http://hz.52xcode.cn/gtmaviotnt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.mhx1999.top/gtsxotiqmu.html

[U24] Py：路径操作
来源：http://hz.chenjidiqi.icu/gturtywpoc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.guowangkeji.top/gtsdbbeodb.html

[U25] Py：CSV 按字典读
来源：http://hz.smart0.xyz/gtikwagquo.html

csv.DictReader(f)
来源：http://hz.chenjidiqi.icu/gtllpadvdu.html

[U26] Py：并发下载
来源：http://hz.chenlongwang.top/gtindfxpym.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sysykeji.top/gtdkbylxud.html

[U27] Py：异步 HTTP
来源：http://hz.yangfankeji.com/gtsxthvbkn.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jyoumei.cn/gtkaewlbgt.html

[U28] Py：类型别名
来源：http://hz.redwolf501.top/gtcxtvdxdu.html

UserId = int
来源：http://hz.nwbrower.top/gtllfohkmn.html


<!-- 参考信息 -->