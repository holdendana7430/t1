代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://hz.hammf.cn/gthvarivjp.html

[S15] C：类型转换
来源：http://hz.cheryme.top/gtmrlkgipa.html

(double) a / b
来源：http://hz.hammf.cn/gtxsxaolbf.html

[S16] C：位操作置位
来源：http://hz.zhijiandao.cn/gtuhcbtkby.html

x |= (1 << 3);
来源：http://hz.xuanzx.com/gtfrnkylww.html

[S17] C：安全拼接字符串
来源：http://hz.havefunace.top/gtgpiruuwv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydzc1.top/gtrpljynyd.html

[S18] C：命令行参数
来源：http://hz.dianchejie.cn/gthftpjera.html

int main(int argc, char **argv)
来源：http://hz.nanxinkj.top/gtvqnewerb.html

[S19] C：快速排序
来源：http://hz.yj20258.top/gtzuztcguk.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtjypeuoth.html

[S20] C：二分查找
来源：http://hz.dianchejie.cn/gtlyfnormm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtnrmrrwjk.html

[S21] C：字符类别判断
来源：http://hz.jinghuilouyu.cn/gtkzwxiyft.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.snrcjt.cn/gtjxryqzil.html

[S22] C：字符串转数字
来源：http://hz.iojbl.cn/gthhhsynbg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhijiandao.cn/gtcuhefsvg.html

[S23] C：随机数
来源：http://hz.svipenyu.cn/gtlyjxhdag.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cucudq.cn/gtzabgmfqn.html

[S24] C：获取本地时间
来源：http://hz.yj20258.top/gtlmmqlqkn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sysykeji.top/gtmcxogddi.html

[S25] C：内存拷贝
来源：http://hz.jinqigfzy.top/gtlbselrab.html

memcpy(dst, src, n);
来源：http://hz.smart0.xyz/gtariigzbn.html

[S26] C：内存清零
来源：http://hz.shanyushiyangtech.top/gttybisoqf.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gtekjwuuiy.html

[S27] C：定义常量
来源：http://hz.c1oappe.top/gtwlsyibme.html

const double PI = 3.14159;
来源：http://hz.cashguo.top/gtygjpsbxu.html

[S28] C：静态变量
来源：http://hz.sxryk.cn/gtemmsybpu.html

static int counter = 0;
来源：http://hz.yongpay.top/gtpogvsnxp.html

[S29] C：变参函数
来源：http://hz.ehwqpu.com/gtcnoxifpz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.mhx1999.top/gtcsnpbugf.html

[S30] C：头文件保护
来源：http://hz.meibo888.top/gtepewsgcs.html

#ifndef X_H
来源：http://hz.316326.xyz/gtsnekkjpn.html

#define X_H
来源：http://hz.ywan-chungtsiang.top/gtfofmevhr.html

#endif
来源：http://hz.sweek.top/gtzyaiandb.html

[S31] C++：Hello World
来源：http://hz.pengpengdd.cyou/gtjujrgqfg.html

#include <iostream>
来源：http://hz.yj202588.top/gtwidlqjqi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.wangdashe.top/gtyunltikk.html

[S32] C++：字符串
来源：http://hz.iojbl.cn/gtnxypejqx.html

std::string s = "hi";  s += "!";
来源：http://hz.zhixingplan.top/gtxcoutpje.html

[S33] C++：vector 增删
来源：http://hz.nanxinkj.top/gtysaoydrb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yongpay.top/gthftlbztl.html

[S34] C++：遍历 vector
来源：http://hz.hnxiangtu.top/gtulpmxgrf.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shangyingyoupin.top/gtuxqvrwye.html

[S35] C++：map
来源：http://hz.hnqzz.top/gtnjkwrosh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gtnuxjpeob.html

[S36] C++：unordered_map
来源：http://hz.hysaishi.cn/gtyvkmqdgu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtjtdtrikx.html

[S37] C++：set
来源：http://hz.nwbrower.top/gtrnmsfwmf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xylfe.cn/gtzvusbmiu.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gtpbenrdjw.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258.top/gttgfexrsh.html

[S39] C++：自定义比较器排序
来源：http://hz.wangshuangyany.cn/gtavogvvlm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.havefunace.top/gtskqpjvlt.html

[S40] C++：查找元素
来源：http://hz.shzxlz.cn/gtwnsprsen.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigfzy.top/gtdybxaxqj.html

[S41] C++：类与构造函数
来源：http://hz.zycfv.cn/gtmzejnqip.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhoulong.xyz/gtowegzkwh.html

[S42] C++：继承与虚函数
来源：http://hz.jqgfzy.top/gtdieqodby.html

class B : public Base { public: void f() override {} };
来源：http://hz.smart0.xyz/gtucklvejn.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gttnofgknr.html

auto p = std::make_unique<int>(5);
来源：http://hz.sysykeji.top/gtrswuoibg.html

[S44] C++：引用传参
来源：http://hz.xinyue.icu/gtqmuuudau.html

void inc(int &x) { ++x; }
来源：http://hz.chenzaomai.com/gtwcbxssxz.html

[S45] C++：lambda
来源：http://hz.jinghuilouyu.cn/gtbyibmpls.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hammf.cn/gtnixbhrmz.html

[S46] C++：函数模板
来源：http://hz.sufxvd.cn/gtflcgnotn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cashguo.top/gtrgjqvcns.html

[S47] C++：结构化绑定遍历
来源：http://hz.hammf.cn/gtkaslbuun.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.c1oappe.top/gtbonxvwdo.html

[S48] C++：逐行读文件
来源：http://hz.zdqjudy.top/gtfdpncxwu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenlongwang.top/gtdotyllnx.html

while (std::getline(in, line)) { }
来源：http://hz.fengsongda.top/gtosuygedo.html

[S49] C++：写文件
来源：http://hz.fengsongda.top/gtwogohmnb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.0kj1m.cn/gtwudrgpwb.html

[S50] C++：格式化数字
来源：http://hz.zhaomingkeji.xyz/gtpjxohnqr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj202588.top/gtpnymwwzg.html

[S51] C++：显式类型转换
来源：http://hz.0kj1m.cn/gtlggonpio.html

static_cast<double>(a) / b
来源：http://hz.zhixingplan.top/gtdqbdkcvz.html

[S52] C++：const 与 noexcept
来源：http://hz.chenzaomai.com/gthqbzotqz.html

int size() const noexcept { return n_; }
来源：http://hz.chenzaomai.com/gtypzlgoqt.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gtewvwdaaq.html

std::vector<int> w = std::move(v);
来源：http://hz.zhiwuduotai.top/gtnkgibdou.html

[S54] C++：异常处理
来源：http://hz.jqgfzy.top/gtinassrti.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xylfe.cn/gtsmcgfokk.html

[S55] C++：结构化绑定
来源：http://hz.ehwqpu.com/gtzbvectpk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinghuilouyu.cn/gtozyyvqbl.html

[S56] C++：optional
来源：http://hz.ywan-chungtsiang.top/gtgfllkmpq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sysykeji.top/gtrwmtympv.html

[S57] C++：编译期常量
来源：http://hz.xinyue.icu/gtfmvqrsty.html

constexpr int N = 10;
来源：http://hz.zhengqikj.top/gtwglxjolo.html

[S58] C++：命名空间
来源：http://hz.ivvv.top/gtigprmzrc.html

namespace ns { int f() { return 1; } }
来源：http://hz.yuanzhike.top/gtgpvescgc.html

[S59] C++：静态断言
来源：http://hz.ydzc1.top/gtrfxpzldq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhengqikj.top/gtnoagfezj.html

[S60] C++：遍历并删除元素
来源：http://hz.tianlin.xyz/gtlozivjxh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zdqjudy.top/gtskgwwwlk.html

================================================================================
来源：http://hz.dianchejie.cn/gtqmvtnxkz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yvedp.cn/gtvpqyeymm.html

================================================================================
来源：http://hz.ydzc1.top/gtzacgppyb.html

[T01] Kotlin：Hello World
来源：http://hz.jqgfzy.top/gtagczwzyh.html

println("Hello")
来源：http://hz.xuetiantiany.cn/gthjcnhbvx.html

[T02] Kotlin：变量
来源：http://hz.sxryk.cn/gtigmupnlz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.pengpengdd.cyou/gtpazlbtkn.html

[T03] Kotlin：字符串模板
来源：http://hz.yueranfly.top/gtohkjuary.html

"值: $b"
来源：http://hz.xziqi.cn/gtogevjduz.html

[T04] Kotlin：空安全
来源：http://hz.yj20258888.top/gthhfknihv.html

val n: String? = null;  n?.length
来源：http://hz.gzhubu.top/gtkfqptena.html

[T05] Kotlin：when 表达式
来源：http://hz.pycfn.com/gttgexknba.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.kuanghao11.cn/gtzkmcunup.html

[T06] Kotlin：集合映射
来源：http://hz.shangyingyoupin.top/gtfbxzfpts.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.fzhhl.top/gtlwedofnv.html

[T07] Kotlin：集合过滤
来源：http://hz.tianlin.xyz/gtldzqnnwb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tianlin.xyz/gtdftftlfc.html

[T08] Kotlin：数据类
来源：http://hz.havefunace.top/gtxjtuqdld.html

data class User(val name: String, val age: Int)
来源：http://hz.ppjwa.cn/gtysvhcqzk.html

[T09] Kotlin：扩展函数
来源：http://hz.feifeiyinyue.top/gtqcxbzljo.html

fun String.exclaim() = this + "!"
来源：http://hz.aibaodan.cn/gtoizagbgz.html

[T10] Kotlin：默认参数
来源：http://hz.xingfuxueyuan.xyz/gtyllhyned.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.0kj1m.cn/gtvtljdftb.html

[T11] Kotlin：协程
来源：http://hz.nwbrower.top/gtmhyojimv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yangfankeji.com/gtevwjgmua.html

[T12] Kotlin：解构声明
来源：http://hz.xuanzx.com/gtadpbfjul.html

val (a, b) = Pair(1, 2)
来源：http://hz.yangfankeji.com/gtjnvucucw.html

[T13] Kotlin：只读 Map
来源：http://hz.yanxiufei.cn/gtgnfmmzlg.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtwkopmxqv.html

[T14] Kotlin：循环
来源：http://hz.chenlongwang.top/gtstfdzuwc.html

for (i in 1..10) println(i)
来源：http://hz.wangshuangyany.cn/gtyvjtjfff.html

[T15] Kotlin：接口
来源：http://hz.jinqigufen.top/gtxhdimgtm.html

interface Shape { fun area(): Double }
来源：http://hz.hnqzz.top/gtcwycmqca.html

[T16] Swift：Hello World
来源：http://hz.cheryme.top/gtujsthqsj.html

print("Hello")
来源：http://hz.yj202588.top/gtyogckqet.html

[T17] Swift：变量与常量
来源：http://hz.shzxlz.cn/gtdbgiylue.html

var a = 1;  let b = 2
来源：http://hz.9152youxi.cn/gtxcbzllfd.html

[T18] Swift：字符串插值
来源：http://hz.zhengqikj.top/gtvilnghwa.html

"值: \(b)"
来源：http://hz.nwbrower.top/gtzwmmzspy.html

[T19] Swift：可选绑定
来源：http://hz.wangshuangyany.cn/gthzjblrbn.html

if let n = opt { print(n) }
来源：http://hz.shuidangran.top/gtvswwoumv.html

[T20] Swift：数组操作
来源：http://hz.xingfuxueyuan.xyz/gtutswnlcd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ydzc1.top/gthowlltmd.html

[T21] Swift：遍历
来源：http://hz.nanxinkj.top/gtmgpsizlq.html

for x in a { print(x) }
来源：http://hz.zhixingplan.top/gtluxalgqz.html

[T22] Swift：字典
来源：http://hz.gzhubu.top/gtpxaxgxkh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xingfuxueyuan.xyz/gtrbvfgyle.html

[T23] Swift：函数
来源：http://hz.tianlin.xyz/gtqzomabys.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tianlin.xyz/gtjxopsxks.html

[T24] Swift：闭包
来源：http://hz.tanke756.top/gtnykofmkr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.haohaochexian.top/gtvxnmncym.html

[T25] Swift：结构体
来源：http://hz.hfpthk.cn/gtulmoaklh.html

struct P { var x: Int }
来源：http://hz.chenlongwang.top/gtavwyftpf.html

[T26] Swift：类与重写
来源：http://hz.9152youxi.cn/gttbpsygfs.html

class A: Base { override func f() {} }
来源：http://hz.chenlongwang.top/gtiegnoymc.html

[T27] Swift：错误处理
来源：http://hz.0kj1m.cn/gtdpzungcl.html

do { try f() } catch { print(error) }
来源：http://hz.meibo888.top/gtztsnbmrq.html

[T28] Swift：枚举
来源：http://hz.hnqzz.top/gtqyjouorz.html

enum Color { case red, green }
来源：http://hz.zhaomingkeji.xyz/gtljilnujc.html

[T29] Swift：guard 提前返回
来源：http://hz.zhongyouzk.top/gtlegmzyqi.html

guard let x = opt else { return }
来源：http://hz.ehwqpu.com/gtjhzronth.html

[T30] Swift：协议
来源：http://hz.ehwqpu.com/gtwszmipvd.html

protocol Shape { func area() -> Double }
来源：http://hz.cdnleiting.top/gthgmeceec.html

[T31] Lua：Hello World
来源：http://hz.zhoulong.xyz/gttjllwhbc.html

print("Hello")
来源：http://hz.hysaishi.cn/gtrndsymvc.html

[T32] Lua：局部变量
来源：http://hz.birdmap.top/gtwqzwwiqm.html

local a = 1
来源：http://hz.cucudq.cn/gtdtvzdacq.html

[T33] Lua：表（数组）
来源：http://hz.9152youxi.cn/gtsdnnvxkg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yanxiufei.cn/gtvcavmvvd.html

[T34] Lua：遍历表
来源：http://hz.yuxming.cn/gtbudwwzxx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.aibaodan.cn/gtgbhrgrea.html

[T35] Lua：字典表
来源：http://hz.kuanghao11.cn/gtottwhvlv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhoulong.xyz/gtbcbfxngt.html

[T36] Lua：函数
来源：http://hz.haohaochexian.top/gtczastxwq.html

function add(a, b) return a + b end
来源：http://hz.pengpengdd.cyou/gtekbkgbox.html

[T37] Lua：字符串拼接
来源：http://hz.wangdashe.top/gtkjrigiuz.html

"a" .. "b"
来源：http://hz.shanyushiyangtech.top/gtytaaukjq.html

[T38] Lua：条件
来源：http://hz.pengpengdd.cyou/gthdymfpil.html

if x > 0 then print("正") end
来源：http://hz.yueranfly.top/gtllmvmobz.html

[T39] Lua：模式匹配
来源：http://hz.xylfe.cn/gtkgvdxhap.html

string.find(s, "%d+")
来源：http://hz.cheryme.top/gtzwodawgw.html

[T40] Lua：元表
来源：http://hz.shanyushiyangtech.top/gtjhcvwdni.html

setmetatable({}, { __index = base })
来源：http://hz.yueranfly.top/gtjizbglxh.html

[T41] Perl：Hello World
来源：http://hz.svipenyu.cn/gtahxpsvpe.html

print "Hello\n";
来源：http://hz.zycfv.cn/gtmyzjiaug.html

[T42] Perl：变量类型
来源：http://hz.jiagoushi.top/gtdyrwehef.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gotoacloud.top/gteibupeyc.html

[T43] Perl：字符串插值
来源：http://hz.hammf.cn/gtqvuzxrki.html

"值: $a"
来源：http://hz.pengpengdd.cyou/gtrczbncfb.html

[T44] Perl：条件
来源：http://hz.hammf.cn/gtuilapwwk.html

if ($a > 0) { print "正"; }
来源：http://hz.yonumen.top/gtpjkhrbpq.html

[T45] Perl：数组遍历
来源：http://hz.xziqi.cn/gtsyacthqf.html

for my $x (@arr) { print $x; }
来源：http://hz.hfpthk.cn/gtdsehklmz.html

[T46] Perl：哈希操作
来源：http://hz.svipenyu.cn/gtkjlugceb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.fengsongda.top/gthdlyyhwc.html

[T47] Perl：正则捕获
来源：http://hz.jyoumei.cn/gtumyozrbf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nanxinkj.top/gtymshjnrv.html

[T48] Perl：正则替换
来源：http://hz.hammf.cn/gthheugjqh.html

$s =~ s/old/new/g;
来源：http://hz.smart0.xyz/gtplzzlxfo.html

[T49] Perl：函数
来源：http://hz.guannengcc.top/gtxkvpbjjw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hfpthk.cn/gtlafglkju.html

[T50] Perl：逐行读文件
来源：http://hz.ehwqpu.com/gtlxvkbmzb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cheryme.top/gtpfdyhmxd.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuanzx.com/gtoemjlkep.html

[T51] Scala：Hello World
来源：http://hz.ydjk.org.cn/gtuuspokym.html

println("Hello")
来源：http://hz.yj20258.top/gtsnrxwcmu.html

[T52] Scala：变量
来源：http://hz.daria6918.cn/gttewqulrw.html

val a = 1;  var b = 2
来源：http://hz.guowangkeji.top/gtegyykrxx.html

[T53] Scala：字符串插值
来源：http://hz.shangyingyoupin.top/gthaytykbm.html

s"值: $b"
来源：http://hz.chenlongwang.top/gtqgzaxlaa.html

[T54] Scala：集合映射
来源：http://hz.zhiwuduotai.top/gtkkmmipbi.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jinqigfzy.top/gtihhkhhiz.html

[T55] Scala：集合过滤
来源：http://hz.zhiwuduotai.top/gtfviuyylf.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jiagoushi.top/gtfovclvtk.html

[T56] Scala：样例类
来源：http://hz.jqgfzy.top/gtxlfhhuwi.html

case class User(name: String, age: Int)
来源：http://hz.gotoacloud.top/gtyvbmwmcm.html

[T57] Scala：模式匹配
来源：http://hz.kuanghao11.cn/gtabjovmmp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.wangdashe.top/gtvhgaxjur.html

[T58] Scala：函数定义
来源：http://hz.yj20258.top/gtkhslsxgf.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jqgfzy.top/gtbdspfnmo.html

[T59] Scala：循环
来源：http://hz.nanxinkj.top/gtluhadbix.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnqzz.top/gtttgjmmrb.html

[T60] Scala：折叠
来源：http://hz.tanke756.top/gtglolkben.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hywenlv.cn/gtbxftusrm.html

================================================================================
来源：http://hz.svipenyu.cn/gtjrfurlul.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.mhx1999.top/gtjpeicovz.html

================================================================================
来源：http://hz.cqqwz.cn/gtlowevsln.html

[U01] Py：创建虚拟环境
来源：http://hz.sufxvd.cn/gtuagvcwft.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tianlin.xyz/gtrvqkznea.html

[U02] Py：导出 / 安装依赖
来源：http://hz.daria6918.cn/gtebxvxfrl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydjk.org.cn/gtoehjuopp.html

[U03] Py：加载 .env 配置
来源：http://hz.nwbrower.top/gtjbhmkhkz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.guowangkeji.top/gtecfytqcn.html

[U04] Py：变量调试打印
来源：http://hz.zhijiandao.cn/gtgyusqmuk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yanxiufei.cn/gtikmvzplk.html

[U05] Py：列表去重且保序
来源：http://hz.guowangkeji.top/gtenfnncsg.html

list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gteuherztt.html

[U06] Py：合并两个字典
来源：http://hz.shanyushiyangtech.top/gttmfkybuc.html

{**a, **b}
来源：http://hz.bjfxy.top/gtwgqjcink.html

[U07] Py：反转字典键值
来源：http://hz.andypj.xyz/gtscvujfoz.html

{v: k for k, v in d.items()}
来源：http://hz.bjfxy.top/gtaudjmbsi.html

[U08] Py：展平二维列表
来源：http://hz.fengsongda.top/gtvinnrgyq.html

[y for x in nested for y in x]
来源：http://hz.shuidangran.top/gtdwwfnlql.html

[U09] Py：字典取最大值的键
来源：http://hz.birdmap.top/gtecszhfjs.html

max(d, key=d.get)
来源：http://hz.hysaishi.cn/gtloaaibrl.html

[U10] Py：按值排序字典
来源：http://hz.sxryk.cn/gthduvlnet.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.tanke756.top/gthpassahh.html

[U11] Py：生成器表达式
来源：http://hz.quarkkingdee.top/gtfwfmqaqa.html

(x * 2 for x in arr)
来源：http://hz.shanyushiyangkeji.top/gtbfibucfe.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hnqzz.top/gtammucclx.html

Counter(arr).most_common(3)
来源：http://hz.hysaishi.cn/gtysylkhql.html

[U13] Py：固定长度队列
来源：http://hz.xylfe.cn/gtulmtcqao.html

deque(maxlen=10)
来源：http://hz.smart0.xyz/gtjfsphyvq.html

[U14] Py：分组收集到列表
来源：http://hz.c1oappe.top/gtxeomaunr.html

defaultdict(list)
来源：http://hz.pycfn.com/gtynfpfedk.html

[U15] Py：高精度计时
来源：http://hz.mhx1999.top/gtvpblbroz.html

t = time.perf_counter()
来源：http://hz.daxiang520.top/gtpkzrrtbr.html

[U16] Py：命令行参数解析
来源：http://hz.wangdashe.top/gtaukyqhsn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gaohongyu789.top/gtjsmietpd.html

[U17] Py：初始化日志
来源：http://hz.sxryk.cn/gtcqddegdr.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.smart0.xyz/gtdqxyvjbi.html

[U18] Py：预编译正则
来源：http://hz.jianghu66.top/gtzametcgp.html

pat = re.compile(r"\d+")
来源：http://hz.fzhhl.top/gtlozssjcz.html

[U19] Py：正则替换带回调
来源：http://hz.redwolf501.top/gtxvtgasgm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhongyouzk.top/gtmcsjynml.html

[U20] Py：缓存函数结果
来源：http://hz.yvedp.cn/gtvotcecqp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yj20258888.top/gtovdqwcpy.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinqigufen.top/gtvemxtjze.html

@contextlib.contextmanager
来源：http://hz.yj202588.top/gtfvrnrrwk.html

[U22] Py：矩阵转置
来源：http://hz.xinyue.icu/gtubtmaqbr.html

list(zip(*m))
来源：http://hz.xuanzx.com/gtkocmebiw.html

[U23] Py：分块读取大文件
来源：http://hz.zhixingplan.top/gtifegjmij.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shzxlz.cn/gtexhfkoin.html

[U24] Py：路径操作
来源：http://hz.shanyushiyangtech.top/gtjfpzzhvc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhongyouzk.top/gtsgqfrgqy.html

[U25] Py：CSV 按字典读
来源：http://hz.ywan-chungtsiang.top/gtagxvbfsh.html

csv.DictReader(f)
来源：http://hz.andypj.xyz/gtmmjgwgqx.html

[U26] Py：并发下载
来源：http://hz.bjfxy.top/gtlqixbppi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.fengsongda.top/gtflbofwmw.html

[U27] Py：异步 HTTP
来源：http://hz.gzhubu.top/gtryhdqqxh.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zycfv.cn/gttbitwwqe.html

[U28] Py：类型别名
来源：http://hz.jlsjyb.cn/gtmxqgsnpo.html

UserId = int
来源：http://hz.ppjwa.cn/gtinbfgfgp.html

[U29] Py：属性校验
来源：http://hz.chenzaomai.com/gtmnkfrevx.html

@property 与 @x.setter 配合
来源：http://hz.bjfxy.top/gtnvefnfun.html

[U30] Py：数据类
来源：http://hz.shanyushiyangtech.top/gteokfeekn.html

@dataclass(slots=True)
来源：http://hz.guannengcc.top/gthgbsikih.html

[U31] Py：单测
来源：http://hz.zhixingplan.top/gtonvwisqm.html

python -m pytest -q
来源：http://hz.gogol.net.cn/gthlrelahf.html

[U32] Py：代码格式化
来源：http://hz.xingfuxueyuan.xyz/gtxopiwuvp.html

ruff format . && ruff check --fix .
来源：http://hz.xylfe.cn/gtiptwjgxj.html

[U33] Py：打包发布
来源：http://hz.shuidangran.top/gtdtoryekg.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.yvedp.cn/gtlhflpzje.html

[U34] Py：判断编码
来源：http://hz.jinyuanbaomall.cn/gtsnfkptsc.html

chardet.detect(raw)
来源：http://hz.yuxming.cn/gtrhltbgos.html

[U35] Py：发送邮件
来源：http://hz.xuanzx.com/gtewwxdidj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhoulong.xyz/gtqrlwibqv.html

[U36] Py：定时任务
来源：http://hz.cashguo.top/gtgreahwhf.html

schedule.every(10).minutes.do(job)
来源：http://hz.haohaochexian.top/gttyedltmp.html

[U37] Py：读写 Excel
来源：http://hz.ppjwa.cn/gthtgbpjpb.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.wangshuangyany.cn/gtlphedrrz.html

[U38] Py：获取脚本所在目录
来源：http://hz.andypj.xyz/gttgtytjvi.html

Path(__file__).resolve().parent
来源：http://hz.redwolf501.top/gtudfmoryn.html


<!-- 参考信息 -->