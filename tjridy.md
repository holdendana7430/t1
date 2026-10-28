代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuanzhike.top/gtmvwkakpe.html

[S10] C：指针与解引用
来源：http://hz.ppjwa.cn/gtorobdpwe.html

int *p = &a;  *p = 5;
来源：http://hz.daria6918.cn/gtgwxhyqpo.html

[S11] C：逐行读文件
来源：http://hz.chenzaomai.com/gthogpjrxw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj20258.top/gtbppsbpbm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fzhhl.top/gtouzjqszn.html

fclose(f);
来源：http://hz.9152youxi.cn/gtvrvczzua.html

[S12] C：写文件
来源：http://hz.hfpthk.cn/gtbybloclj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sxryk.cn/gtpehgxmfk.html

[S13] C：宏定义
来源：http://hz.cucudq.cn/gtvcrygpcg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenlongwang.top/gtxbxzrmmk.html

[S14] C：枚举
来源：http://hz.gotoacloud.top/gtrxsyvwos.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.quarkkingdee.top/gtgviiadwu.html

[S15] C：类型转换
来源：http://hz.hfpthk.cn/gtzejygrhs.html

(double) a / b
来源：http://hz.aizwys.cn/gtignpwrbc.html

[S16] C：位操作置位
来源：http://hz.feifeiyinyue.top/gtqinikkyh.html

x |= (1 << 3);
来源：http://hz.tanke756.top/gtotsdiony.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtzprbirfp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.meibo888.top/gteunyqozs.html

[S18] C：命令行参数
来源：http://hz.nwbrower.top/gtwwtfoiwt.html

int main(int argc, char **argv)
来源：http://hz.dashuyun.cn/gtniohfmtl.html

[S19] C：快速排序
来源：http://hz.hysaishi.cn/gtakihlldn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtqvraeftc.html

[S20] C：二分查找
来源：http://hz.dashuyun.cn/gtlclukzlw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtlvdyiqgy.html

[S21] C：字符类别判断
来源：http://hz.haohaochexian.top/gtpquktwcu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hnqzz.top/gtvxzasypa.html

[S22] C：字符串转数字
来源：http://hz.ivvv.top/gtewvrmrzl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shanyushiyangtech.top/gtwthblsls.html

[S23] C：随机数
来源：http://hz.kuanghao11.cn/gtwpfcojpi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xinyue.icu/gtqodiqehc.html

[S24] C：获取本地时间
来源：http://hz.meibo888.top/gtnlfbravj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuxming.cn/gtnkapmbai.html

[S25] C：内存拷贝
来源：http://hz.hnqzz.top/gtrmmibjqo.html

memcpy(dst, src, n);
来源：http://hz.wangdashe.top/gtujimtcqx.html

[S26] C：内存清零
来源：http://hz.jinqigfzy.top/gtjbdgveuk.html

memset(a, 0, sizeof a);
来源：http://hz.jinqigufen.top/gtwpxedraj.html

[S27] C：定义常量
来源：http://hz.iojbl.cn/gtqxjdepdj.html

const double PI = 3.14159;
来源：http://hz.52xcode.cn/gteroynlbk.html

[S28] C：静态变量
来源：http://hz.yanxiufei.cn/gtqnshqwfx.html

static int counter = 0;
来源：http://hz.jinyuanbaomall.cn/gtkdgoopaq.html

[S29] C：变参函数
来源：http://hz.nanxinkj.top/gtfbsezleq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hysaishi.cn/gtayexzxlg.html

[S30] C：头文件保护
来源：http://hz.hnqzz.top/gtkeirakns.html

#ifndef X_H
来源：http://hz.c1oappe.top/gtfayybrdh.html

#define X_H
来源：http://hz.birdmap.top/gtdnwtshzn.html

#endif
来源：http://hz.zhijiandao.cn/gtgqmqysxr.html

[S31] C++：Hello World
来源：http://hz.dashuyun.cn/gtptaevbxx.html

#include <iostream>
来源：http://hz.chenjidiqi.icu/gtjrdvupdr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.quarkkingdee.top/gtslizyxod.html

[S32] C++：字符串
来源：http://hz.yangfankeji.com/gtnsrgwcfl.html

std::string s = "hi";  s += "!";
来源：http://hz.aizwys.cn/gtajogpdle.html

[S33] C++：vector 增删
来源：http://hz.yongpay.top/gtuteuhqmd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gtltcdojon.html

[S34] C++：遍历 vector
来源：http://hz.zhixingplan.top/gturyhgtcs.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hysaishi.cn/gtnivbeuus.html

[S35] C++：map
来源：http://hz.fzhhl.top/gtwosgwhsi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtwqhzixuh.html

[S36] C++：unordered_map
来源：http://hz.hfpthk.cn/gtgozmwsbs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuxming.cn/gtavcchqrd.html

[S37] C++：set
来源：http://hz.dianchejie.cn/gtmezguvqr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cdnleiting.top/gtavsogoxt.html

[S38] C++：排序
来源：http://hz.aizwys.cn/gtotvhuqon.html

std::sort(v.begin(), v.end());
来源：http://hz.snrcjt.cn/gtgxeydcxi.html

[S39] C++：自定义比较器排序
来源：http://hz.wangshuangyany.cn/gtmhrzbvyp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj202588.top/gtcwivrauf.html

[S40] C++：查找元素
来源：http://hz.dianchejie.cn/gtyuukioxf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hongshengwenyu.top/gtusjesaeh.html

[S41] C++：类与构造函数
来源：http://hz.hongshengwenyu.top/gtzmyufmvm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aizwys.cn/gthbjdidtg.html

[S42] C++：继承与虚函数
来源：http://hz.vqdsnc.cn/gtgcqbsbpg.html

class B : public Base { public: void f() override {} };
来源：http://hz.feifeiyinyue.top/gtyiogxzvb.html

[S43] C++：智能指针
来源：http://hz.haohaochexian.top/gtvvaedfdd.html

auto p = std::make_unique<int>(5);
来源：http://hz.tian-w.cn/gtcerzhncm.html

[S44] C++：引用传参
来源：http://hz.chenlongwang.top/gtixwwtfjd.html

void inc(int &x) { ++x; }
来源：http://hz.zhongyouzk.top/gtbsdmqhwn.html

[S45] C++：lambda
来源：http://hz.316326.xyz/gtgzjddsri.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xingfuxueyuan.xyz/gtjepueacu.html

[S46] C++：函数模板
来源：http://hz.pengpengdd.cyou/gtqaqiudbo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenlongwang.top/gtmlgsblvn.html

[S47] C++：结构化绑定遍历
来源：http://hz.hywenlv.cn/gtemgpunkt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tian-w.cn/gtkczjvwfo.html

[S48] C++：逐行读文件
来源：http://hz.zhoulong.xyz/gtqkcdxfep.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgufenzy.top/gtwrihpfzr.html

while (std::getline(in, line)) { }
来源：http://hz.gaohongyu789.top/gtxzwglwcl.html

[S49] C++：写文件
来源：http://hz.dashuyun.cn/gtghlblogj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.dashuyun.cn/gthlchokqv.html

[S50] C++：格式化数字
来源：http://hz.fengsongda.top/gtaljcajor.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yvedp.cn/gtongtztsh.html

[S51] C++：显式类型转换
来源：http://hz.zhixingplan.top/gtynmfzpxh.html

static_cast<double>(a) / b
来源：http://hz.yueranfly.top/gtzuaoosgw.html

[S52] C++：const 与 noexcept
来源：http://hz.andypj.xyz/gthavncrlt.html

int size() const noexcept { return n_; }
来源：http://hz.hammf.cn/gtxuhbwqvt.html

[S53] C++：移动语义
来源：http://hz.0kj1m.cn/gtflzpblla.html

std::vector<int> w = std::move(v);
来源：http://hz.cheryme.top/gtdhbahxsb.html

[S54] C++：异常处理
来源：http://hz.sufxvd.cn/gtaywndnje.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnqzz.top/gttkbvhqis.html

[S55] C++：结构化绑定
来源：http://hz.andypj.xyz/gtjrpfqysu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgufenzy.top/gtelzhrcwd.html

[S56] C++：optional
来源：http://hz.dashuyun.cn/gtrlfffssu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xinyue.icu/gtvifwoset.html

[S57] C++：编译期常量
来源：http://hz.yj20258888.top/gtfcmijwsr.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gtgzlcmpop.html

[S58] C++：命名空间
来源：http://hz.hnxiangtu.top/gtpabdkdkw.html

namespace ns { int f() { return 1; } }
来源：http://hz.tianlin.xyz/gtbgfmgtgj.html

[S59] C++：静态断言
来源：http://hz.52xcode.cn/gtzixmbhtd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yonumen.top/gteiqyizbi.html

[S60] C++：遍历并删除元素
来源：http://hz.jiagoushi.top/gtfvhslusw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jlsjyb.cn/gtbujmbevo.html

================================================================================
来源：http://hz.gaohongyu789.top/gtiuoyirpb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.iojbl.cn/gtlsjiqlxp.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtozjjonfh.html

[T01] Kotlin：Hello World
来源：http://hz.xziqi.cn/gtoevswfdm.html

println("Hello")
来源：http://hz.sweek.top/gtegergnrh.html

[T02] Kotlin：变量
来源：http://hz.snrcjt.cn/gtkfwowgtq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhengqikj.top/gtzvpzptwr.html

[T03] Kotlin：字符串模板
来源：http://hz.pycfn.com/gtoepjjebq.html

"值: $b"
来源：http://hz.pengpengdd.cyou/gtwzniqzid.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangkeji.top/gthruohjru.html

val n: String? = null;  n?.length
来源：http://hz.fengsongda.top/gtoybsijas.html

[T05] Kotlin：when 表达式
来源：http://hz.yongpay.top/gttcjbtwpo.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.meibo888.top/gtqctsrdrj.html

[T06] Kotlin：集合映射
来源：http://hz.xuetiantiany.cn/gtzrfduvmy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sufxvd.cn/gttsbonoyb.html

[T07] Kotlin：集合过滤
来源：http://hz.ywan-chungtsiang.top/gtbsjrefal.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.kuanghao11.cn/gttldwqtqr.html

[T08] Kotlin：数据类
来源：http://hz.sysykeji.top/gtkrqoaama.html

data class User(val name: String, val age: Int)
来源：http://hz.xuanzx.com/gtarynqqzp.html

[T09] Kotlin：扩展函数
来源：http://hz.cashguo.top/gtvsspsjai.html

fun String.exclaim() = this + "!"
来源：http://hz.hnxiangtu.top/gtiqxmegsh.html

[T10] Kotlin：默认参数
来源：http://hz.ehwqpu.com/gtoqhxxksl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gtqstbsmuz.html

[T11] Kotlin：协程
来源：http://hz.shanyushiyangtech.top/gtkuwflsom.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ppjwa.cn/gtggfotjdr.html

[T12] Kotlin：解构声明
来源：http://hz.xuetiantiany.cn/gtsktoxtbd.html

val (a, b) = Pair(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtndkotzqf.html

[T13] Kotlin：只读 Map
来源：http://hz.hfpthk.cn/gtswfvxohu.html

val m = mapOf("a" to 1)
来源：http://hz.bjfxy.top/gtmlmdsitz.html

[T14] Kotlin：循环
来源：http://hz.vqdsnc.cn/gtzhmtofkd.html

for (i in 1..10) println(i)
来源：http://hz.xuanzx.com/gtchujwlhq.html

[T15] Kotlin：接口
来源：http://hz.yvedp.cn/gtrektyqgg.html

interface Shape { fun area(): Double }
来源：http://hz.yanxiufei.cn/gtolokhzuq.html

[T16] Swift：Hello World
来源：http://hz.zhijiandao.cn/gtldiutwin.html

print("Hello")
来源：http://hz.guannengcc.top/gtldotmipg.html

[T17] Swift：变量与常量
来源：http://hz.xinyue.icu/gtqiglszwq.html

var a = 1;  let b = 2
来源：http://hz.gotoacloud.top/gtidisiqcj.html

[T18] Swift：字符串插值
来源：http://hz.birdmap.top/gtfednuzse.html

"值: \(b)"
来源：http://hz.ywan-chungtsiang.top/gtyurxlbsi.html

[T19] Swift：可选绑定
来源：http://hz.dianchejie.cn/gtbwzxdqzf.html

if let n = opt { print(n) }
来源：http://hz.gaohongyu789.top/gtlrtzhchg.html

[T20] Swift：数组操作
来源：http://hz.xuanzx.com/gtwpnqtgpo.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cdnleiting.top/gtwtrhywfi.html

[T21] Swift：遍历
来源：http://hz.xingfuxueyuan.xyz/gtnrdauoca.html

for x in a { print(x) }
来源：http://hz.guannengcc.top/gtabltibnk.html

[T22] Swift：字典
来源：http://hz.gzhubu.top/gtpyurmsht.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxinkj.top/gtgeoiiokw.html

[T23] Swift：函数
来源：http://hz.smart0.xyz/gtdtgffloa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhixingplan.top/gtrfntwfnv.html

[T24] Swift：闭包
来源：http://hz.shzxlz.cn/gtkiidhurv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenlongwang.top/gtaxveyaky.html

[T25] Swift：结构体
来源：http://hz.birdmap.top/gtxhzzekic.html

struct P { var x: Int }
来源：http://hz.xingfuxueyuan.xyz/gtuehxssqg.html

[T26] Swift：类与重写
来源：http://hz.yuxming.cn/gtwtfoppsk.html

class A: Base { override func f() {} }
来源：http://hz.ydjk.org.cn/gtxowpfzar.html

[T27] Swift：错误处理
来源：http://hz.hnxiangtu.top/gtoskcmgkz.html

do { try f() } catch { print(error) }
来源：http://hz.mhx1999.top/gtphgxwybu.html

[T28] Swift：枚举
来源：http://hz.yuanzhike.top/gtxxgzlrpp.html

enum Color { case red, green }
来源：http://hz.yj202588.top/gtiqffsohf.html

[T29] Swift：guard 提前返回
来源：http://hz.xziqi.cn/gtjhkkjwri.html

guard let x = opt else { return }
来源：http://hz.jqgufenzy.top/gtzhoolagk.html

[T30] Swift：协议
来源：http://hz.yueranfly.top/gthxaypdmq.html

protocol Shape { func area() -> Double }
来源：http://hz.xingfuxueyuan.xyz/gtavxrtmnf.html

[T31] Lua：Hello World
来源：http://hz.ehwqpu.com/gtemhmrsme.html

print("Hello")
来源：http://hz.zhoulong.xyz/gtzljgevkd.html

[T32] Lua：局部变量
来源：http://hz.zhoulong.xyz/gtxbbobzti.html

local a = 1
来源：http://hz.yongpay.top/gtlrmekerx.html

[T33] Lua：表（数组）
来源：http://hz.yonumen.top/gtkmefdxtu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gaohongyu789.top/gtoaobgfsj.html

[T34] Lua：遍历表
来源：http://hz.c1oappe.top/gtlrioifao.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.52xcode.cn/gtkygsoydu.html

[T35] Lua：字典表
来源：http://hz.xinyue.icu/gtntildxxj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zdqjudy.top/gtqajlyiud.html

[T36] Lua：函数
来源：http://hz.316326.xyz/gtnajherly.html

function add(a, b) return a + b end
来源：http://hz.jiagoushi.top/gtrvxqmvab.html

[T37] Lua：字符串拼接
来源：http://hz.daria6918.cn/gtsgoplotv.html

"a" .. "b"
来源：http://hz.ydzc1.top/gtciiunqpw.html

[T38] Lua：条件
来源：http://hz.fengsongda.top/gtapefpwpg.html

if x > 0 then print("正") end
来源：http://hz.xuetiantiany.cn/gtupopodah.html

[T39] Lua：模式匹配
来源：http://hz.pycfn.com/gtjmrslmvp.html

string.find(s, "%d+")
来源：http://hz.chenlongwang.top/gtvostawsm.html

[T40] Lua：元表
来源：http://hz.pycfn.com/gtmfmsdhil.html

setmetatable({}, { __index = base })
来源：http://hz.sysykeji.top/gtoourayke.html

[T41] Perl：Hello World
来源：http://hz.yonumen.top/gtnynmtktq.html

print "Hello\n";
来源：http://hz.yueranfly.top/gtrvbtzyvx.html

[T42] Perl：变量类型
来源：http://hz.fengsongda.top/gtmgfhfhcf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinghuilouyu.cn/gtstoiwkfs.html

[T43] Perl：字符串插值
来源：http://hz.xziqi.cn/gttrgsmwbd.html

"值: $a"
来源：http://hz.yuanzhike.top/gtjhxftcie.html

[T44] Perl：条件
来源：http://hz.fzhhl.top/gtqvbooylz.html

if ($a > 0) { print "正"; }
来源：http://hz.nanxuanxn.top/gtzmxuullv.html

[T45] Perl：数组遍历
来源：http://hz.jqgfzy.top/gtdgdmbzib.html

for my $x (@arr) { print $x; }
来源：http://hz.jinqigfzy.top/gtbtblljhp.html

[T46] Perl：哈希操作
来源：http://hz.jyoumei.cn/gtyswbyndn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yangfankeji.com/gtskwsulkt.html

[T47] Perl：正则捕获
来源：http://hz.bjfxy.top/gtsyxbqquj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.0kj1m.cn/gtxjdlbiwo.html

[T48] Perl：正则替换
来源：http://hz.hnxiangtu.top/gtgnaobfhk.html

$s =~ s/old/new/g;
来源：http://hz.jinyuanbaomall.cn/gtfdtyphtg.html

[T49] Perl：函数
来源：http://hz.gogol.net.cn/gtavyfelyj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xuetiantiany.cn/gteypmatid.html

[T50] Perl：逐行读文件
来源：http://hz.vqdsnc.cn/gtvdetnqgu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yongpay.top/gtjzqnbrjf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.daxiang520.top/gtcbggwyfi.html

[T51] Scala：Hello World
来源：http://hz.xziqi.cn/gtaoxghonb.html

println("Hello")
来源：http://hz.xuanzx.com/gtjvpalmoa.html

[T52] Scala：变量
来源：http://hz.jqgufenzy.top/gtiscqqizu.html

val a = 1;  var b = 2
来源：http://hz.xuetiantiany.cn/gtjfbmwrdq.html

[T53] Scala：字符串插值
来源：http://hz.feifeiyinyue.top/gtnsmnxvpd.html

s"值: $b"
来源：http://hz.xinyue.icu/gtwhlmfeii.html

[T54] Scala：集合映射
来源：http://hz.hammf.cn/gtrwgvsojq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zdqjudy.top/gtfwzxmyme.html

[T55] Scala：集合过滤
来源：http://hz.guowangkeji.top/gtvngehsnn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.nanxinkj.top/gtonspwujf.html

[T56] Scala：样例类
来源：http://hz.kuanghao11.cn/gtghsvyidv.html

case class User(name: String, age: Int)
来源：http://hz.xuetiantiany.cn/gtabvwvvif.html

[T57] Scala：模式匹配
来源：http://hz.gaohongyu789.top/gtxaoqfccw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.iojbl.cn/gttnshjskz.html

[T58] Scala：函数定义
来源：http://hz.c1oappe.top/gtmllmwxoe.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinqigufen.top/gtgrvhujwv.html

[T59] Scala：循环
来源：http://hz.zycfv.cn/gtywcpjyzr.html

for (i <- 1 to 10) println(i)
来源：http://hz.jiagoushi.top/gtwcymzezj.html

[T60] Scala：折叠
来源：http://hz.zdqjudy.top/gtitxlypzp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenlongwang.top/gtpmvyuvgi.html

================================================================================
来源：http://hz.zhengqikj.top/gtksmzijco.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.meibo888.top/gtgyiuingn.html

================================================================================
来源：http://hz.shzxlz.cn/gtnypcpuvp.html

[U01] Py：创建虚拟环境
来源：http://hz.zhoulong.xyz/gtkaimgulq.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.vqdsnc.cn/gtrjuzqywc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ivvv.top/gtdlkhjeya.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.fzhhl.top/gtfkfbzpnu.html

[U03] Py：加载 .env 配置
来源：http://hz.gaohongyu789.top/gtgtpljfyq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hammf.cn/gtrutijsxd.html

[U04] Py：变量调试打印
来源：http://hz.shanyushiyangkeji.top/gtfliaydrj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.guannengcc.top/gttidaqrzn.html

[U05] Py：列表去重且保序
来源：http://hz.cqqwz.cn/gttnhcmvnm.html

list(dict.fromkeys(arr))
来源：http://hz.andypj.xyz/gtacxvapdf.html

[U06] Py：合并两个字典
来源：http://hz.birdmap.top/gtuorjbqvx.html

{**a, **b}
来源：http://hz.52xcode.cn/gtaikckqbr.html

[U07] Py：反转字典键值
来源：http://hz.aizwys.cn/gtzogmadte.html

{v: k for k, v in d.items()}
来源：http://hz.fzhhl.top/gtskjipuhz.html

[U08] Py：展平二维列表
来源：http://hz.iojbl.cn/gtvfgmmnlu.html

[y for x in nested for y in x]
来源：http://hz.yueranfly.top/gtrweizunv.html

[U09] Py：字典取最大值的键
来源：http://hz.yj20258888.top/gtnlxpjsak.html

max(d, key=d.get)
来源：http://hz.bjfxy.top/gtmctduicb.html

[U10] Py：按值排序字典
来源：http://hz.sysykeji.top/gtihocndmf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.daria6918.cn/gtbyyhtibi.html

[U11] Py：生成器表达式
来源：http://hz.jinghuilouyu.cn/gtangsrpxq.html

(x * 2 for x in arr)
来源：http://hz.guowangkeji.top/gtwdkgvtbt.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.meibo888.top/gtyprnrhlb.html

Counter(arr).most_common(3)
来源：http://hz.nanxinkj.top/gtorjtmzir.html

[U13] Py：固定长度队列
来源：http://hz.zhongyouzk.top/gtbnsocoym.html

deque(maxlen=10)
来源：http://hz.ydjk.org.cn/gtolfgusyn.html

[U14] Py：分组收集到列表
来源：http://hz.shzxlz.cn/gtqkfmonuw.html

defaultdict(list)
来源：http://hz.mhx1999.top/gtgurcyabw.html

[U15] Py：高精度计时
来源：http://hz.bjfxy.top/gtgdsnikkv.html

t = time.perf_counter()
来源：http://hz.hongshengwenyu.top/gtabhhuhoa.html

[U16] Py：命令行参数解析
来源：http://hz.shanyushiyangkeji.top/gtojwfecec.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.guowangkeji.top/gtwmfunyaf.html

[U17] Py：初始化日志
来源：http://hz.jinghuilouyu.cn/gtptifdlah.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.tianlin.xyz/gthafvaalb.html

[U18] Py：预编译正则
来源：http://hz.ppjwa.cn/gtcwphmtwo.html

pat = re.compile(r"\d+")
来源：http://hz.shuidangran.top/gtnoohtqro.html

[U19] Py：正则替换带回调
来源：http://hz.chenlongwang.top/gtmdgciems.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jinyuanbaomall.cn/gtoeugufmy.html

[U20] Py：缓存函数结果
来源：http://hz.yangfankeji.com/gtywenadbj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.daria6918.cn/gtesddpfsr.html

[U21] Py：自定义上下文管理器
来源：http://hz.nanxinkj.top/gtnrkzngyu.html

@contextlib.contextmanager
来源：http://hz.guannengcc.top/gtfoqpjckx.html

[U22] Py：矩阵转置
来源：http://hz.sysykeji.top/gteetlkojj.html

list(zip(*m))
来源：http://hz.sysykeji.top/gtdpxoejhm.html

[U23] Py：分块读取大文件
来源：http://hz.yuxming.cn/gtfvsbvsmc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.wangdashe.top/gtxoangooa.html

[U24] Py：路径操作
来源：http://hz.dianchejie.cn/gtwpmmjjxz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.sxryk.cn/gtcqflbpsd.html

[U25] Py：CSV 按字典读
来源：http://hz.dianchejie.cn/gtgctvvbsl.html

csv.DictReader(f)
来源：http://hz.jinghuilouyu.cn/gtcmotskis.html

[U26] Py：并发下载
来源：http://hz.shangyingyoupin.top/gtbhntxaua.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.xuetiantiany.cn/gtiulmtlqy.html

[U27] Py：异步 HTTP
来源：http://hz.sxryk.cn/gtxnqxxlth.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sweek.top/gtemnnrabh.html

[U28] Py：类型别名
来源：http://hz.ppjwa.cn/gtwldnwdgo.html

UserId = int
来源：http://hz.smart0.xyz/gtohcdqend.html

[U29] Py：属性校验
来源：http://hz.shangyingyoupin.top/gthscreppi.html

@property 与 @x.setter 配合
来源：http://hz.52xcode.cn/gtnmrctmxq.html

[U30] Py：数据类
来源：http://hz.hywenlv.cn/gttzkupiva.html

@dataclass(slots=True)
来源：http://hz.hammf.cn/gtoqwijyxf.html

[U31] Py：单测
来源：http://hz.dashuyun.cn/gtvcttcmcf.html

python -m pytest -q
来源：http://hz.hnxiangtu.top/gtdzpywgky.html

[U32] Py：代码格式化
来源：http://hz.pengpengdd.cyou/gtfnquhflp.html

ruff format . && ruff check --fix .
来源：http://hz.xziqi.cn/gtjpqbpczg.html


<!-- 参考信息 -->