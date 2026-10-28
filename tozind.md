代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ydjk.org.cn/gtincrdamt.html

[S13] C：宏定义
来源：http://hz.fzhhl.top/gtvbhktico.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.52xcode.cn/gtsvypaaug.html

[S14] C：枚举
来源：http://hz.andypj.xyz/gtvslgtjqw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenlongwang.top/gtqnpkzsxi.html

[S15] C：类型转换
来源：http://hz.c1oappe.top/gtibbeteuk.html

(double) a / b
来源：http://hz.wangshuangyany.cn/gtsyrpkzov.html

[S16] C：位操作置位
来源：http://hz.meibo888.top/gtmkoxzsch.html

x |= (1 << 3);
来源：http://hz.fengsongda.top/gtbmpdrnyh.html

[S17] C：安全拼接字符串
来源：http://hz.hnqzz.top/gtmmgbvtkw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.aizwys.cn/gtomdvxbdv.html

[S18] C：命令行参数
来源：http://hz.iojbl.cn/gtlzprngya.html

int main(int argc, char **argv)
来源：http://hz.svipenyu.cn/gtimxooato.html

[S19] C：快速排序
来源：http://hz.tanke756.top/gtiyfdarlh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.vqdsnc.cn/gtyhfxysyb.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtabfwznce.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtiiuzowoh.html

[S21] C：字符类别判断
来源：http://hz.xziqi.cn/gtpvhqvyru.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.meibo888.top/gtzoljadhu.html

[S22] C：字符串转数字
来源：http://hz.havefunace.top/gtezgeefle.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ehwqpu.com/gtcncberkp.html

[S23] C：随机数
来源：http://hz.gogol.net.cn/gthdspwvph.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ywan-chungtsiang.top/gtjyvwckdv.html

[S24] C：获取本地时间
来源：http://hz.zhijiandao.cn/gtiioammoo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhixingplan.top/gtqgilovml.html

[S25] C：内存拷贝
来源：http://hz.hnxiangtu.top/gtcmjqlnms.html

memcpy(dst, src, n);
来源：http://hz.ywan-chungtsiang.top/gtwivktiwp.html

[S26] C：内存清零
来源：http://hz.cdnleiting.top/gtoxxbbhho.html

memset(a, 0, sizeof a);
来源：http://hz.cashguo.top/gtmruwywlq.html

[S27] C：定义常量
来源：http://hz.zhongyouzk.top/gtvzxatrnn.html

const double PI = 3.14159;
来源：http://hz.yj20258888.top/gtzndelcao.html

[S28] C：静态变量
来源：http://hz.gzhubu.top/gtkylgzwkq.html

static int counter = 0;
来源：http://hz.meibo888.top/gtufswfuze.html

[S29] C：变参函数
来源：http://hz.tanke756.top/gttospxupr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xinyue.icu/gtrsjntxhi.html

[S30] C：头文件保护
来源：http://hz.hywenlv.cn/gtuhtsxywm.html

#ifndef X_H
来源：http://hz.0kj1m.cn/gtaadshisq.html

#define X_H
来源：http://hz.svipenyu.cn/gtnasupscc.html

#endif
来源：http://hz.xziqi.cn/gtmpaonaje.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtgknpvfbi.html

#include <iostream>
来源：http://hz.shzxlz.cn/gtfjtkkhmv.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xingfuxueyuan.xyz/gtuekjjytv.html

[S32] C++：字符串
来源：http://hz.smart0.xyz/gtulqleykx.html

std::string s = "hi";  s += "!";
来源：http://hz.dianchejie.cn/gtepintiiv.html

[S33] C++：vector 增删
来源：http://hz.jinqigfzy.top/gtuavmferz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gotoacloud.top/gtzvpxedib.html

[S34] C++：遍历 vector
来源：http://hz.jinghuilouyu.cn/gtftwgqtsy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gogol.net.cn/gtdalmpdsx.html

[S35] C++：map
来源：http://hz.zhijiandao.cn/gtcdlsszva.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtvbmdmtzo.html

[S36] C++：unordered_map
来源：http://hz.xingfuxueyuan.xyz/gtztmdpmwz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenjidiqi.icu/gtjuftigbv.html

[S37] C++：set
来源：http://hz.andypj.xyz/gtvazjynsq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xingfuxueyuan.xyz/gtgoogxasy.html

[S38] C++：排序
来源：http://hz.zdqjudy.top/gteueocrxu.html

std::sort(v.begin(), v.end());
来源：http://hz.jinyuanbaomall.cn/gtpyduafcm.html

[S39] C++：自定义比较器排序
来源：http://hz.quarkkingdee.top/gtgkuiaani.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shzxlz.cn/gtbvuszmvs.html

[S40] C++：查找元素
来源：http://hz.guannengcc.top/gtuyqxornl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.vqdsnc.cn/gtgdzhnryj.html

[S41] C++：类与构造函数
来源：http://hz.bjfxy.top/gtlbxetxds.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuxming.cn/gtirsehojc.html

[S42] C++：继承与虚函数
来源：http://hz.smart0.xyz/gtugxjpdem.html

class B : public Base { public: void f() override {} };
来源：http://hz.ehwqpu.com/gthsxcqhjf.html

[S43] C++：智能指针
来源：http://hz.zycfv.cn/gtumqrcdqu.html

auto p = std::make_unique<int>(5);
来源：http://hz.yangfankeji.com/gtxmyryuor.html

[S44] C++：引用传参
来源：http://hz.nanxuanxn.top/gtgcqqegqo.html

void inc(int &x) { ++x; }
来源：http://hz.guannengcc.top/gtcdmoranj.html

[S45] C++：lambda
来源：http://hz.zhixingplan.top/gtiwziwcma.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xziqi.cn/gtxsqgxlrr.html

[S46] C++：函数模板
来源：http://hz.ywan-chungtsiang.top/gtvahnykfg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shangyingyoupin.top/gtqtfgjgkq.html

[S47] C++：结构化绑定遍历
来源：http://hz.smart0.xyz/gttwqkitff.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shanyushiyangkeji.top/gtwtetsckj.html

[S48] C++：逐行读文件
来源：http://hz.kuanghao11.cn/gtrjcnoyms.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtackzkvfy.html

while (std::getline(in, line)) { }
来源：http://hz.pengpengdd.cyou/gtaiyjyadk.html

[S49] C++：写文件
来源：http://hz.yangfankeji.com/gtionmhtss.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ywan-chungtsiang.top/gtuzdtxqow.html

[S50] C++：格式化数字
来源：http://hz.chenjidiqi.icu/gtinciujxi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenlongwang.top/gtrvogcwoh.html

[S51] C++：显式类型转换
来源：http://hz.cheryme.top/gtnsgbcxvk.html

static_cast<double>(a) / b
来源：http://hz.bjfxy.top/gtzqphmogp.html

[S52] C++：const 与 noexcept
来源：http://hz.snrcjt.cn/gtwpghnkth.html

int size() const noexcept { return n_; }
来源：http://hz.hongshengwenyu.top/gtrqdozflv.html

[S53] C++：移动语义
来源：http://hz.jianghu66.top/gtlearaufo.html

std::vector<int> w = std::move(v);
来源：http://hz.jinghuilouyu.cn/gtnnexncsw.html

[S54] C++：异常处理
来源：http://hz.hnxiangtu.top/gtiulodqhl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinqigfzy.top/gtxqlywfip.html

[S55] C++：结构化绑定
来源：http://hz.jlsjyb.cn/gtxvfmwtoq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hysaishi.cn/gtdqjtxxru.html

[S56] C++：optional
来源：http://hz.snrcjt.cn/gtsqtylccr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sxryk.cn/gtbhqcshpw.html

[S57] C++：编译期常量
来源：http://hz.hnqzz.top/gtctsoaian.html

constexpr int N = 10;
来源：http://hz.quarkkingdee.top/gtaggzgaht.html

[S58] C++：命名空间
来源：http://hz.yanxiufei.cn/gthqowptqg.html

namespace ns { int f() { return 1; } }
来源：http://hz.xuanzx.com/gtvdjxyhmu.html

[S59] C++：静态断言
来源：http://hz.quarkkingdee.top/gtvkhaopis.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xziqi.cn/gtbjmtarwm.html

[S60] C++：遍历并删除元素
来源：http://hz.52xcode.cn/gtxuforzlk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hfpthk.cn/gtiirhoszj.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtyqxrterm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yangfankeji.com/gtxcijinll.html

================================================================================
来源：http://hz.ydjk.org.cn/gtdvygprux.html

[T01] Kotlin：Hello World
来源：http://hz.haohaochexian.top/gtcciysczf.html

println("Hello")
来源：http://hz.gzhubu.top/gtcvcxemoa.html

[T02] Kotlin：变量
来源：http://hz.hfpthk.cn/gtgzlzjjnl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.fzhhl.top/gtjdvxavay.html

[T03] Kotlin：字符串模板
来源：http://hz.cdnleiting.top/gtndobqynl.html

"值: $b"
来源：http://hz.xziqi.cn/gtludkehcp.html

[T04] Kotlin：空安全
来源：http://hz.guannengcc.top/gtnpuuibti.html

val n: String? = null;  n?.length
来源：http://hz.zhijiandao.cn/gtbhfgmhqn.html

[T05] Kotlin：when 表达式
来源：http://hz.ydjk.org.cn/gticcasotb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shanyushiyangkeji.top/gtbvvvcxzs.html

[T06] Kotlin：集合映射
来源：http://hz.jqgfzy.top/gtpddfnric.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhongyouzk.top/gtzvgfvqgq.html

[T07] Kotlin：集合过滤
来源：http://hz.ivvv.top/gthmbggucg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yueranfly.top/gtvusvnxbv.html

[T08] Kotlin：数据类
来源：http://hz.haohaochexian.top/gtzqfrazpz.html

data class User(val name: String, val age: Int)
来源：http://hz.bjfxy.top/gtqrdbcxqw.html

[T09] Kotlin：扩展函数
来源：http://hz.ydzc1.top/gtbchbutve.html

fun String.exclaim() = this + "!"
来源：http://hz.wangshuangyany.cn/gtdthmiiow.html

[T10] Kotlin：默认参数
来源：http://hz.iojbl.cn/gtotbwubdd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.c1oappe.top/gtjimhrpzc.html

[T11] Kotlin：协程
来源：http://hz.aizwys.cn/gtntaoqyvw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sysykeji.top/gtieclwmdi.html

[T12] Kotlin：解构声明
来源：http://hz.zhiwuduotai.top/gtcoalussp.html

val (a, b) = Pair(1, 2)
来源：http://hz.ybcxt.top/gtjebalukx.html

[T13] Kotlin：只读 Map
来源：http://hz.gotoacloud.top/gtxorsdbft.html

val m = mapOf("a" to 1)
来源：http://hz.ywan-chungtsiang.top/gtlzcbthjv.html

[T14] Kotlin：循环
来源：http://hz.tianlin.xyz/gtpfthfdrn.html

for (i in 1..10) println(i)
来源：http://hz.vqdsnc.cn/gtexobmiqd.html

[T15] Kotlin：接口
来源：http://hz.jinghuilouyu.cn/gtszexyesi.html

interface Shape { fun area(): Double }
来源：http://hz.ppjwa.cn/gtjaypodpn.html

[T16] Swift：Hello World
来源：http://hz.cucudq.cn/gtljbswhcd.html

print("Hello")
来源：http://hz.jinghuilouyu.cn/gtvplscdlh.html

[T17] Swift：变量与常量
来源：http://hz.0kj1m.cn/gtmieqxpmp.html

var a = 1;  let b = 2
来源：http://hz.cashguo.top/gtiwwkjcvx.html

[T18] Swift：字符串插值
来源：http://hz.zhaomingkeji.xyz/gtbdvumsge.html

"值: \(b)"
来源：http://hz.pycfn.com/gtfatxuxah.html

[T19] Swift：可选绑定
来源：http://hz.cucudq.cn/gtemlagdkn.html

if let n = opt { print(n) }
来源：http://hz.xuanzx.com/gtktpaahtv.html

[T20] Swift：数组操作
来源：http://hz.yuxming.cn/gttfgpajxu.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.guowangkeji.top/gtotlbwjxk.html

[T21] Swift：遍历
来源：http://hz.kuanghao11.cn/gtunwzzhwa.html

for x in a { print(x) }
来源：http://hz.nanxinkj.top/gtaphyvdnb.html

[T22] Swift：字典
来源：http://hz.ppjwa.cn/gtkhkjdskt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hammf.cn/gttdyrltax.html

[T23] Swift：函数
来源：http://hz.guannengcc.top/gtcmqedwed.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sxryk.cn/gtevcwjqzq.html

[T24] Swift：闭包
来源：http://hz.yueranfly.top/gtbwhkjsxl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nwbrower.top/gtjwyhlxrq.html

[T25] Swift：结构体
来源：http://hz.gzhubu.top/gtxuapmyii.html

struct P { var x: Int }
来源：http://hz.gzhubu.top/gtjxkwzutr.html

[T26] Swift：类与重写
来源：http://hz.yvedp.cn/gtstcphuzm.html

class A: Base { override func f() {} }
来源：http://hz.jiagoushi.top/gtwtqfanlb.html

[T27] Swift：错误处理
来源：http://hz.hfpthk.cn/gtusmezwnj.html

do { try f() } catch { print(error) }
来源：http://hz.9152youxi.cn/gtghoentnh.html

[T28] Swift：枚举
来源：http://hz.dashuyun.cn/gtgxpbhfho.html

enum Color { case red, green }
来源：http://hz.gaohongyu789.top/gtzykwdwck.html

[T29] Swift：guard 提前返回
来源：http://hz.nwbrower.top/gtovieurhl.html

guard let x = opt else { return }
来源：http://hz.xziqi.cn/gtrofwespl.html

[T30] Swift：协议
来源：http://hz.snrcjt.cn/gtyzkumqim.html

protocol Shape { func area() -> Double }
来源：http://hz.aibaodan.cn/gtvzfhxznm.html

[T31] Lua：Hello World
来源：http://hz.dianchejie.cn/gtezfnpjzr.html

print("Hello")
来源：http://hz.ydjk.org.cn/gtvevfjmsq.html

[T32] Lua：局部变量
来源：http://hz.nwbrower.top/gtaobijuhs.html

local a = 1
来源：http://hz.zhixingplan.top/gtcthetjph.html

[T33] Lua：表（数组）
来源：http://hz.wangdashe.top/gtmtijswbk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yangfankeji.com/gtgwkruuht.html

[T34] Lua：遍历表
来源：http://hz.havefunace.top/gtvyjcdozx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.52xcode.cn/gtldagwdvd.html

[T35] Lua：字典表
来源：http://hz.kuanghao11.cn/gtjwkenenm.html

local d = { a = 1 };  d.b = 2
来源：http://hz.feifeiyinyue.top/gtoehxleve.html

[T36] Lua：函数
来源：http://hz.aibaodan.cn/gtdjkxsaju.html

function add(a, b) return a + b end
来源：http://hz.shzxlz.cn/gtdytopezb.html

[T37] Lua：字符串拼接
来源：http://hz.jiagoushi.top/gtzmjlbxrc.html

"a" .. "b"
来源：http://hz.shuidangran.top/gtayetovzg.html

[T38] Lua：条件
来源：http://hz.gaohongyu789.top/gtqdnrkwug.html

if x > 0 then print("正") end
来源：http://hz.tianlin.xyz/gtcvkupifx.html

[T39] Lua：模式匹配
来源：http://hz.wangshuangyany.cn/gtvagpdmgk.html

string.find(s, "%d+")
来源：http://hz.316326.xyz/gtdrykdbwh.html

[T40] Lua：元表
来源：http://hz.cdnleiting.top/gttysqqkfb.html

setmetatable({}, { __index = base })
来源：http://hz.fzhhl.top/gteqdkxvlz.html

[T41] Perl：Hello World
来源：http://hz.smart0.xyz/gtknuanqzh.html

print "Hello\n";
来源：http://hz.hnxiangtu.top/gtlgtybeco.html

[T42] Perl：变量类型
来源：http://hz.quarkkingdee.top/gttosdcbjd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhijiandao.cn/gtdvybvlov.html

[T43] Perl：字符串插值
来源：http://hz.pengpengdd.cyou/gtajwklfmh.html

"值: $a"
来源：http://hz.guannengcc.top/gtzewbpisl.html

[T44] Perl：条件
来源：http://hz.c1oappe.top/gtwkfpyyoe.html

if ($a > 0) { print "正"; }
来源：http://hz.nanxinkj.top/gtpgrgxgvy.html

[T45] Perl：数组遍历
来源：http://hz.gogol.net.cn/gtjtgdmrod.html

for my $x (@arr) { print $x; }
来源：http://hz.jiagoushi.top/gtxnggbvgd.html

[T46] Perl：哈希操作
来源：http://hz.tianlin.xyz/gtrzmkabew.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xuetiantiany.cn/gtfbedjfgt.html

[T47] Perl：正则捕获
来源：http://hz.tanke756.top/gtjlpwfori.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sxryk.cn/gtyqoimnsa.html

[T48] Perl：正则替换
来源：http://hz.gogol.net.cn/gtopzxztyb.html

$s =~ s/old/new/g;
来源：http://hz.ppjwa.cn/gtrxarafxf.html

[T49] Perl：函数
来源：http://hz.52xcode.cn/gtqtmylozt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gzhubu.top/gtkyuymxme.html

[T50] Perl：逐行读文件
来源：http://hz.meibo888.top/gtqqnjivam.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cucudq.cn/gtwhcqnwqt.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.birdmap.top/gtpbjmpkev.html

[T51] Scala：Hello World
来源：http://hz.mhx1999.top/gtdrhiuunh.html

println("Hello")
来源：http://hz.chenlongwang.top/gtsprwtwvo.html

[T52] Scala：变量
来源：http://hz.tianlin.xyz/gttjoejprg.html

val a = 1;  var b = 2
来源：http://hz.zhixingplan.top/gtkdfsirrd.html

[T53] Scala：字符串插值
来源：http://hz.dianchejie.cn/gtfepmhjgm.html

s"值: $b"
来源：http://hz.fzhhl.top/gtrzjtrplx.html

[T54] Scala：集合映射
来源：http://hz.shuidangran.top/gtcrkgwkrq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cqqwz.cn/gtiptmqerx.html

[T55] Scala：集合过滤
来源：http://hz.daxiang520.top/gtgmotvaqp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.guannengcc.top/gtututedea.html

[T56] Scala：样例类
来源：http://hz.jinghuilouyu.cn/gtcptyptid.html

case class User(name: String, age: Int)
来源：http://hz.ehwqpu.com/gtkmpeyvmz.html

[T57] Scala：模式匹配
来源：http://hz.52xcode.cn/gtvuskpfjo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zycfv.cn/gtqyabmjgf.html

[T58] Scala：函数定义
来源：http://hz.sweek.top/gtuwjuypmh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.daria6918.cn/gtglpearmb.html

[T59] Scala：循环
来源：http://hz.hywenlv.cn/gtpejcxjih.html

for (i <- 1 to 10) println(i)
来源：http://hz.xuetiantiany.cn/gtbyqobito.html

[T60] Scala：折叠
来源：http://hz.zhaomingkeji.xyz/gtybnruabv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yueranfly.top/gtwtpvesdi.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtuehmaygw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhijiandao.cn/gtjipbuimm.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtkijkyliz.html

[U01] Py：创建虚拟环境
来源：http://hz.daria6918.cn/gtsvtwpaxq.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhixingplan.top/gtjrhbqxoc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.birdmap.top/gtfhzofkrq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.vqdsnc.cn/gtrwmklune.html

[U03] Py：加载 .env 配置
来源：http://hz.hongshengwenyu.top/gtaenjsuvo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jqgfzy.top/gtaidoaqyw.html

[U04] Py：变量调试打印
来源：http://hz.zdqjudy.top/gtjowygyye.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.mhx1999.top/gtonfnasdc.html

[U05] Py：列表去重且保序
来源：http://hz.jqgufenzy.top/gtiesjxcek.html

list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtmuwvydtt.html

[U06] Py：合并两个字典
来源：http://hz.gzhubu.top/gthbuiqkcl.html

{**a, **b}
来源：http://hz.chenzaomai.com/gtezkxryif.html

[U07] Py：反转字典键值
来源：http://hz.chenlongwang.top/gtnxsvlwsc.html

{v: k for k, v in d.items()}
来源：http://hz.guowangkeji.top/gtlmaeyuok.html

[U08] Py：展平二维列表
来源：http://hz.yj20258.top/gtnfgpmsmu.html

[y for x in nested for y in x]
来源：http://hz.nanxinkj.top/gtwdtokhpl.html

[U09] Py：字典取最大值的键
来源：http://hz.jinqigfzy.top/gtvpxsuoil.html

max(d, key=d.get)
来源：http://hz.guannengcc.top/gtzcepusgw.html

[U10] Py：按值排序字典
来源：http://hz.shzxlz.cn/gtxwbpkgtb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.haohaochexian.top/gtzidacbut.html

[U11] Py：生成器表达式
来源：http://hz.jyoumei.cn/gtfwzyxrkw.html

(x * 2 for x in arr)
来源：http://hz.fengsongda.top/gtbcihclth.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.cheryme.top/gtajzzxlsh.html

Counter(arr).most_common(3)
来源：http://hz.ywan-chungtsiang.top/gtwqzdpgqo.html

[U13] Py：固定长度队列
来源：http://hz.52xcode.cn/gtizxbqvhb.html

deque(maxlen=10)
来源：http://hz.sysykeji.top/gtnjonlyzj.html

[U14] Py：分组收集到列表
来源：http://hz.jianghu66.top/gtxjjslisr.html

defaultdict(list)
来源：http://hz.hammf.cn/gtyfssbnfj.html

[U15] Py：高精度计时
来源：http://hz.nanxinkj.top/gtwjlmdlls.html

t = time.perf_counter()
来源：http://hz.tianlin.xyz/gtiehzjmto.html

[U16] Py：命令行参数解析
来源：http://hz.sweek.top/gtvrodwbiu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.pycfn.com/gtpgekzebh.html

[U17] Py：初始化日志
来源：http://hz.jinqigufen.top/gtrizbnyhs.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.9152youxi.cn/gtjcuzgepz.html

[U18] Py：预编译正则
来源：http://hz.hnqzz.top/gtqqoikors.html

pat = re.compile(r"\d+")
来源：http://hz.yvedp.cn/gtrriqtgsl.html

[U19] Py：正则替换带回调
来源：http://hz.mhx1999.top/gtirbcurgg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.gzhubu.top/gtqplwtlwx.html

[U20] Py：缓存函数结果
来源：http://hz.gzhubu.top/gtcamtksii.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yonumen.top/gtokxfbypq.html

[U21] Py：自定义上下文管理器
来源：http://hz.birdmap.top/gtbnkcdood.html

@contextlib.contextmanager
来源：http://hz.yj202588.top/gttlcevvjg.html

[U22] Py：矩阵转置
来源：http://hz.zhiwuduotai.top/gtqzlcfntp.html

list(zip(*m))
来源：http://hz.guowangkeji.top/gtrylizmhw.html

[U23] Py：分块读取大文件
来源：http://hz.yangfankeji.com/gtotggztcb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.tianlin.xyz/gtevdthsvx.html

[U24] Py：路径操作
来源：http://hz.aibaodan.cn/gtlhmjpisf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gaohongyu789.top/gtymvlimjd.html

[U25] Py：CSV 按字典读
来源：http://hz.yj20258888.top/gtrkkdgiji.html

csv.DictReader(f)
来源：http://hz.andypj.xyz/gtcenggsmm.html

[U26] Py：并发下载
来源：http://hz.ppjwa.cn/gtusfarmft.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.cdnleiting.top/gtlccuylbj.html

[U27] Py：异步 HTTP
来源：http://hz.wangdashe.top/gtohlybizh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.smart0.xyz/gtgemotopo.html

[U28] Py：类型别名
来源：http://hz.sxryk.cn/gtjazuegga.html

UserId = int
来源：http://hz.shanyushiyangkeji.top/gtdjnfpyfr.html

[U29] Py：属性校验
来源：http://hz.nanxinkj.top/gtredocojv.html

@property 与 @x.setter 配合
来源：http://hz.pengpengdd.cyou/gtdcwfousc.html

[U30] Py：数据类
来源：http://hz.vqdsnc.cn/gtqpzpcclq.html

@dataclass(slots=True)
来源：http://hz.9152youxi.cn/gtwfvcpjwh.html

[U31] Py：单测
来源：http://hz.yangfankeji.com/gtftatlwee.html

python -m pytest -q
来源：http://hz.cqqwz.cn/gtnfdqzenx.html

[U32] Py：代码格式化
来源：http://hz.yj20258.top/gtntdctgzx.html

ruff format . && ruff check --fix .
来源：http://hz.hywenlv.cn/gtrepcconz.html

[U33] Py：打包发布
来源：http://hz.nwbrower.top/gttljbyhve.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.kuanghao11.cn/gtfucouwes.html

[U34] Py：判断编码
来源：http://hz.jinyuanbaomall.cn/gtaqogifuk.html

chardet.detect(raw)
来源：http://hz.nwbrower.top/gtsgvvozpm.html

[U35] Py：发送邮件
来源：http://hz.aizwys.cn/gtvxoijjdq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.tian-w.cn/gtvmebyswj.html

[U36] Py：定时任务
来源：http://hz.fengsongda.top/gtofanfdlg.html

schedule.every(10).minutes.do(job)
来源：http://hz.xuetiantiany.cn/gtqmfujcfh.html


<!-- 参考信息 -->