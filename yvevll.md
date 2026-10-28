代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://hz.cqqwz.cn/gtzrkribkh.html

[S15] C：类型转换
来源：http://hz.zhijiandao.cn/gtfjqpphne.html

(double) a / b
来源：http://hz.yanxiufei.cn/gtidyrskgk.html

[S16] C：位操作置位
来源：http://hz.hywenlv.cn/gtldjgyyeq.html

x |= (1 << 3);
来源：http://hz.xuanzx.com/gtqxncltev.html

[S17] C：安全拼接字符串
来源：http://hz.ehwqpu.com/gtiyjwxdty.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sweek.top/gtdtzlujvi.html

[S18] C：命令行参数
来源：http://hz.redwolf501.top/gtwacayilx.html

int main(int argc, char **argv)
来源：http://hz.nanxuanxn.top/gtheeaqtzf.html

[S19] C：快速排序
来源：http://hz.chenjidiqi.icu/gtzlhrvvii.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtypntmduo.html

[S20] C：二分查找
来源：http://hz.yonumen.top/gtkhnhasnh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xziqi.cn/gtnyzhskde.html

[S21] C：字符类别判断
来源：http://hz.xziqi.cn/gtssbdtyqg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guowangkeji.top/gtsukhgbpf.html

[S22] C：字符串转数字
来源：http://hz.pycfn.com/gtzenoppuu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jqgfzy.top/gtyhkzmmvs.html

[S23] C：随机数
来源：http://hz.smart0.xyz/gtngnsvnhz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtnuuxhmsa.html

[S24] C：获取本地时间
来源：http://hz.yueranfly.top/gtbapltvbm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhaomingkeji.xyz/gtusqgxiys.html

[S25] C：内存拷贝
来源：http://hz.hysaishi.cn/gtywwbwcms.html

memcpy(dst, src, n);
来源：http://hz.hywenlv.cn/gtdwezclgz.html

[S26] C：内存清零
来源：http://hz.zhijiandao.cn/gtqehblurv.html

memset(a, 0, sizeof a);
来源：http://hz.jlsjyb.cn/gtptqxyiid.html

[S27] C：定义常量
来源：http://hz.yuxming.cn/gtiejuqmst.html

const double PI = 3.14159;
来源：http://hz.havefunace.top/gtdosailjq.html

[S28] C：静态变量
来源：http://hz.zhijiandao.cn/gtykiticzk.html

static int counter = 0;
来源：http://hz.meibo888.top/gtucqfjcpy.html

[S29] C：变参函数
来源：http://hz.xuanzx.com/gtsnwcwqfv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.9152youxi.cn/gtyorcbcum.html

[S30] C：头文件保护
来源：http://hz.tanke756.top/gtbnplxnau.html

#ifndef X_H
来源：http://hz.iojbl.cn/gtltjbbyot.html

#define X_H
来源：http://hz.cashguo.top/gtaazpxfay.html

#endif
来源：http://hz.yuanzhike.top/gtlmcvycww.html

[S31] C++：Hello World
来源：http://hz.daxiang520.top/gtzwretcee.html

#include <iostream>
来源：http://hz.shuidangran.top/gtcjmoaiya.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenlongwang.top/gtynresyrj.html

[S32] C++：字符串
来源：http://hz.zhaomingkeji.xyz/gtxghmmlck.html

std::string s = "hi";  s += "!";
来源：http://hz.shzxlz.cn/gtrjmndsjo.html

[S33] C++：vector 增删
来源：http://hz.xinyue.icu/gtxfthkwnz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xylfe.cn/gtfudacnqm.html

[S34] C++：遍历 vector
来源：http://hz.guannengcc.top/gtzwrtqsrm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ywan-chungtsiang.top/gtvugswaph.html

[S35] C++：map
来源：http://hz.yj20258.top/gtrxzaenyf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hysaishi.cn/gtymletxmy.html

[S36] C++：unordered_map
来源：http://hz.yangfankeji.com/gthodazbgu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtuobghlha.html

[S37] C++：set
来源：http://hz.dashuyun.cn/gtllfqoyhp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jianghu66.top/gtadmiarem.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gttzytykcn.html

std::sort(v.begin(), v.end());
来源：http://hz.c1oappe.top/gtsfsrfdut.html

[S39] C++：自定义比较器排序
来源：http://hz.jinqigufen.top/gtuubbbwlk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nwbrower.top/gtlvswmnif.html

[S40] C++：查找元素
来源：http://hz.quarkkingdee.top/gttmmxzjcc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.andypj.xyz/gtcgqthrpc.html

[S41] C++：类与构造函数
来源：http://hz.xinyue.icu/gtwlplfaru.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jqgufenzy.top/gtrglkwqww.html

[S42] C++：继承与虚函数
来源：http://hz.jianghu66.top/gthhiahpsd.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangkeji.top/gtcttnuhza.html

[S43] C++：智能指针
来源：http://hz.yangfankeji.com/gtpewrebof.html

auto p = std::make_unique<int>(5);
来源：http://hz.9152youxi.cn/gtfvzgdkvc.html

[S44] C++：引用传参
来源：http://hz.bjfxy.top/gtnscvtbcz.html

void inc(int &x) { ++x; }
来源：http://hz.9152youxi.cn/gtflpggrxd.html

[S45] C++：lambda
来源：http://hz.jyoumei.cn/gtceehmstb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yongpay.top/gtdmwlofxv.html

[S46] C++：函数模板
来源：http://hz.xziqi.cn/gthgggvcto.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pycfn.com/gtvwpbxwco.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinghuilouyu.cn/gtokmtomhk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gogol.net.cn/gtlrswoken.html

[S48] C++：逐行读文件
来源：http://hz.ybcxt.top/gtqbfexwst.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.aizwys.cn/gtvsyxhywk.html

while (std::getline(in, line)) { }
来源：http://hz.daxiang520.top/gtwyndoltm.html

[S49] C++：写文件
来源：http://hz.hywenlv.cn/gtebzkmpwl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xuetiantiany.cn/gtvkypjhzj.html

[S50] C++：格式化数字
来源：http://hz.zhengqikj.top/gtzoxqsffx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxinkj.top/gtdwycylif.html

[S51] C++：显式类型转换
来源：http://hz.yj20258888.top/gtsahhlaih.html

static_cast<double>(a) / b
来源：http://hz.shanyushiyangtech.top/gtrtyirxbz.html

[S52] C++：const 与 noexcept
来源：http://hz.jinghuilouyu.cn/gtjgigzxgm.html

int size() const noexcept { return n_; }
来源：http://hz.nanxuanxn.top/gtgsditcnl.html

[S53] C++：移动语义
来源：http://hz.hongshengwenyu.top/gtjoyecmjq.html

std::vector<int> w = std::move(v);
来源：http://hz.redwolf501.top/gtefbesrab.html

[S54] C++：异常处理
来源：http://hz.jyoumei.cn/gtcblvlsco.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hammf.cn/gtebzhajms.html

[S55] C++：结构化绑定
来源：http://hz.cqqwz.cn/gtcvtaufwg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhoulong.xyz/gtrcayseze.html

[S56] C++：optional
来源：http://hz.vqdsnc.cn/gtiuqmjopj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gogol.net.cn/gtfxiancwn.html

[S57] C++：编译期常量
来源：http://hz.ehwqpu.com/gtlouaakrn.html

constexpr int N = 10;
来源：http://hz.cashguo.top/gtbqyrctau.html

[S58] C++：命名空间
来源：http://hz.svipenyu.cn/gtuhtcbhmx.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangdashe.top/gtragenngq.html

[S59] C++：静态断言
来源：http://hz.ehwqpu.com/gtgwaqnwej.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gogol.net.cn/gtivcihpdb.html

[S60] C++：遍历并删除元素
来源：http://hz.chenjidiqi.icu/gtbgzbldra.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinghuilouyu.cn/gtzioratzo.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtwmoccjus.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.tian-w.cn/gtnyuwkadk.html

================================================================================
来源：http://hz.0kj1m.cn/gtocxoduvw.html

[T01] Kotlin：Hello World
来源：http://hz.jqgfzy.top/gtvuwiskvo.html

println("Hello")
来源：http://hz.yj20258888.top/gtmzeczfpv.html

[T02] Kotlin：变量
来源：http://hz.yuxming.cn/gtkxlnofgw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gaohongyu789.top/gtsyloqdct.html

[T03] Kotlin：字符串模板
来源：http://hz.cucudq.cn/gtkmsmnmjq.html

"值: $b"
来源：http://hz.nwbrower.top/gtbxnmtkrg.html

[T04] Kotlin：空安全
来源：http://hz.zhiwuduotai.top/gtrkfrmrzs.html

val n: String? = null;  n?.length
来源：http://hz.tanke756.top/gtuppmdafr.html

[T05] Kotlin：when 表达式
来源：http://hz.yj202588.top/gttxcodzsx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ybcxt.top/gtjhzlexom.html

[T06] Kotlin：集合映射
来源：http://hz.zhaomingkeji.xyz/gtmkieztyq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.meibo888.top/gtqgulynqx.html

[T07] Kotlin：集合过滤
来源：http://hz.cheryme.top/gtzhjutqia.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xingfuxueyuan.xyz/gtxuhhohaf.html

[T08] Kotlin：数据类
来源：http://hz.yvedp.cn/gtcqtsrsmc.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gtcalaelxi.html

[T09] Kotlin：扩展函数
来源：http://hz.ywan-chungtsiang.top/gtuzpqfnoe.html

fun String.exclaim() = this + "!"
来源：http://hz.shzxlz.cn/gticmdbyaz.html

[T10] Kotlin：默认参数
来源：http://hz.ppjwa.cn/gtrdimxfbo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinghuilouyu.cn/gtgqkosdui.html

[T11] Kotlin：协程
来源：http://hz.hywenlv.cn/gttpxhvfnp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.dashuyun.cn/gtfraktooo.html

[T12] Kotlin：解构声明
来源：http://hz.jinqigfzy.top/gtqyropjsy.html

val (a, b) = Pair(1, 2)
来源：http://hz.yvedp.cn/gtwhnyadnr.html

[T13] Kotlin：只读 Map
来源：http://hz.hnxiangtu.top/gtmlhupuvj.html

val m = mapOf("a" to 1)
来源：http://hz.guowangkeji.top/gtseuofeit.html

[T14] Kotlin：循环
来源：http://hz.chenzaomai.com/gtmthukpue.html

for (i in 1..10) println(i)
来源：http://hz.ivvv.top/gtwgrynijp.html

[T15] Kotlin：接口
来源：http://hz.redwolf501.top/gtdevccttb.html

interface Shape { fun area(): Double }
来源：http://hz.yueranfly.top/gtgahdafxt.html

[T16] Swift：Hello World
来源：http://hz.shzxlz.cn/gtneylkyva.html

print("Hello")
来源：http://hz.daxiang520.top/gtpniyfmfp.html

[T17] Swift：变量与常量
来源：http://hz.gotoacloud.top/gtuzbyvesa.html

var a = 1;  let b = 2
来源：http://hz.guannengcc.top/gtxgeycmnv.html

[T18] Swift：字符串插值
来源：http://hz.gzhubu.top/gtgqtiuffp.html

"值: \(b)"
来源：http://hz.yongpay.top/gtxmuobxbl.html

[T19] Swift：可选绑定
来源：http://hz.yueranfly.top/gtqokusefe.html

if let n = opt { print(n) }
来源：http://hz.yj20258888.top/gtrbicyisp.html

[T20] Swift：数组操作
来源：http://hz.ehwqpu.com/gtmfhtghlg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhaomingkeji.xyz/gtxzieydlt.html

[T21] Swift：遍历
来源：http://hz.shangyingyoupin.top/gtgyjwpkpc.html

for x in a { print(x) }
来源：http://hz.havefunace.top/gtdxhhhoqm.html

[T22] Swift：字典
来源：http://hz.bjfxy.top/gtjlgvgdap.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sweek.top/gtksporewu.html

[T23] Swift：函数
来源：http://hz.cashguo.top/gtsejygmcn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.fzhhl.top/gtcfibtiqx.html

[T24] Swift：闭包
来源：http://hz.yuanzhike.top/gtzvheytvb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ybcxt.top/gtyfgywhrb.html

[T25] Swift：结构体
来源：http://hz.xingfuxueyuan.xyz/gtvaanhnko.html

struct P { var x: Int }
来源：http://hz.nanxuanxn.top/gtjotprnzs.html

[T26] Swift：类与重写
来源：http://hz.shzxlz.cn/gtgqxrnvfm.html

class A: Base { override func f() {} }
来源：http://hz.cheryme.top/gtfvjoojmz.html

[T27] Swift：错误处理
来源：http://hz.zhiwuduotai.top/gtvzzomkli.html

do { try f() } catch { print(error) }
来源：http://hz.yangfankeji.com/gtopqvufpu.html

[T28] Swift：枚举
来源：http://hz.yongpay.top/gtkfvammhn.html

enum Color { case red, green }
来源：http://hz.iojbl.cn/gtlyjvmsqz.html

[T29] Swift：guard 提前返回
来源：http://hz.yj20258.top/gtuxisaugw.html

guard let x = opt else { return }
来源：http://hz.dianchejie.cn/gtryensahl.html

[T30] Swift：协议
来源：http://hz.xingfuxueyuan.xyz/gtxcpsuhwg.html

protocol Shape { func area() -> Double }
来源：http://hz.hnxiangtu.top/gtsydylqfj.html

[T31] Lua：Hello World
来源：http://hz.quarkkingdee.top/gtsmylmatd.html

print("Hello")
来源：http://hz.chenzaomai.com/gtyukwecnv.html

[T32] Lua：局部变量
来源：http://hz.fengsongda.top/gtipdzqmvb.html

local a = 1
来源：http://hz.nanxinkj.top/gtagdvfiwd.html

[T33] Lua：表（数组）
来源：http://hz.sysykeji.top/gtszaochdw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj20258888.top/gtutuwkhzs.html

[T34] Lua：遍历表
来源：http://hz.jinqigfzy.top/gtfxgevpkx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jyoumei.cn/gtnjqwkjmd.html

[T35] Lua：字典表
来源：http://hz.yvedp.cn/gtfmjrgnjw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj20258.top/gtllcmfwxw.html

[T36] Lua：函数
来源：http://hz.ppjwa.cn/gtiwaqgahy.html

function add(a, b) return a + b end
来源：http://hz.xziqi.cn/gtkxqpmplo.html

[T37] Lua：字符串拼接
来源：http://hz.tanke756.top/gtbtgahvyy.html

"a" .. "b"
来源：http://hz.havefunace.top/gtwuidfwyn.html

[T38] Lua：条件
来源：http://hz.yonumen.top/gtfyqdkotm.html

if x > 0 then print("正") end
来源：http://hz.jinqigfzy.top/gtfuixpnra.html

[T39] Lua：模式匹配
来源：http://hz.chenjidiqi.icu/gteqbngows.html

string.find(s, "%d+")
来源：http://hz.yj202588.top/gtxgzjogpl.html

[T40] Lua：元表
来源：http://hz.meibo888.top/gtwieulbma.html

setmetatable({}, { __index = base })
来源：http://hz.snrcjt.cn/gtgtntlqre.html

[T41] Perl：Hello World
来源：http://hz.0kj1m.cn/gtuoumkaeg.html

print "Hello\n";
来源：http://hz.cucudq.cn/gtwubtqzoo.html

[T42] Perl：变量类型
来源：http://hz.yuxming.cn/gttfdkjcrs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shanyushiyangtech.top/gtptqietof.html

[T43] Perl：字符串插值
来源：http://hz.zhengqikj.top/gtjczjqvtn.html

"值: $a"
来源：http://hz.jyoumei.cn/gtfdwschdw.html

[T44] Perl：条件
来源：http://hz.jiagoushi.top/gtojzjhbhw.html

if ($a > 0) { print "正"; }
来源：http://hz.guannengcc.top/gteocwwzdu.html

[T45] Perl：数组遍历
来源：http://hz.zhongyouzk.top/gtllkomqzf.html

for my $x (@arr) { print $x; }
来源：http://hz.zhoulong.xyz/gtmzmithog.html

[T46] Perl：哈希操作
来源：http://hz.zhaomingkeji.xyz/gtcauwmuwe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhijiandao.cn/gtpwagbwly.html

[T47] Perl：正则捕获
来源：http://hz.ppjwa.cn/gtvddwziyg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangtech.top/gtsifzydsv.html

[T48] Perl：正则替换
来源：http://hz.hnxiangtu.top/gtmfoffnsx.html

$s =~ s/old/new/g;
来源：http://hz.fengsongda.top/gtwsvtlgvu.html

[T49] Perl：函数
来源：http://hz.xingfuxueyuan.xyz/gtryruworg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xylfe.cn/gtowfohaxx.html

[T50] Perl：逐行读文件
来源：http://hz.chenzaomai.com/gtuwrreifr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.guannengcc.top/gthvgmmhyj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.haohaochexian.top/gthgahpzes.html

[T51] Scala：Hello World
来源：http://hz.yonumen.top/gtwdyurayi.html

println("Hello")
来源：http://hz.fzhhl.top/gtnnphinkb.html

[T52] Scala：变量
来源：http://hz.jianghu66.top/gtvebqzefv.html

val a = 1;  var b = 2
来源：http://hz.dashuyun.cn/gtumsdmgwd.html

[T53] Scala：字符串插值
来源：http://hz.kuanghao11.cn/gtxqpzstmp.html

s"值: $b"
来源：http://hz.yvedp.cn/gtalvswwga.html

[T54] Scala：集合映射
来源：http://hz.yj202588.top/gtdvdfnmek.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hongshengwenyu.top/gtrgyefrka.html

[T55] Scala：集合过滤
来源：http://hz.sysykeji.top/gtdsomcmbx.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xziqi.cn/gtadqusdef.html

[T56] Scala：样例类
来源：http://hz.hysaishi.cn/gtdrgdxozp.html

case class User(name: String, age: Int)
来源：http://hz.chenjidiqi.icu/gtewrmonrr.html

[T57] Scala：模式匹配
来源：http://hz.jyoumei.cn/gtsjboubmh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zdqjudy.top/gthcumjneb.html

[T58] Scala：函数定义
来源：http://hz.ppjwa.cn/gtqdchbomr.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinghuilouyu.cn/gtlfqkxowb.html

[T59] Scala：循环
来源：http://hz.tianlin.xyz/gtketoucst.html

for (i <- 1 to 10) println(i)
来源：http://hz.yonumen.top/gtquzdkjpl.html

[T60] Scala：折叠
来源：http://hz.shanyushiyangtech.top/gtqmfruwtx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sweek.top/gtqvjvzjqy.html

================================================================================
来源：http://hz.smart0.xyz/gtrdelqelw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.0kj1m.cn/gtkcszvncj.html

================================================================================
来源：http://hz.cqqwz.cn/gtvolfkpgg.html

[U01] Py：创建虚拟环境
来源：http://hz.mhx1999.top/gtdxxtmqzg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.gaohongyu789.top/gtfdodznfy.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ydjk.org.cn/gtlrrsqctt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xziqi.cn/gtmwynykyo.html

[U03] Py：加载 .env 配置
来源：http://hz.tanke756.top/gtdjsxbpcn.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jianghu66.top/gtftehetrm.html

[U04] Py：变量调试打印
来源：http://hz.hywenlv.cn/gttvkycvqr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gotoacloud.top/gtmtiwmpld.html

[U05] Py：列表去重且保序
来源：http://hz.jyoumei.cn/gtocpvnztg.html

list(dict.fromkeys(arr))
来源：http://hz.yj202588.top/gtdlsjxxtn.html

[U06] Py：合并两个字典
来源：http://hz.birdmap.top/gtkbetifhh.html

{**a, **b}
来源：http://hz.yanxiufei.cn/gtadatrozk.html

[U07] Py：反转字典键值
来源：http://hz.jianghu66.top/gtjqahyudu.html

{v: k for k, v in d.items()}
来源：http://hz.cqqwz.cn/gtsschrsti.html

[U08] Py：展平二维列表
来源：http://hz.ywan-chungtsiang.top/gtswctzojd.html

[y for x in nested for y in x]
来源：http://hz.xylfe.cn/gtwrkzfwgd.html

[U09] Py：字典取最大值的键
来源：http://hz.yj20258.top/gtatqboaxp.html

max(d, key=d.get)
来源：http://hz.yonumen.top/gtevecmnos.html

[U10] Py：按值排序字典
来源：http://hz.aizwys.cn/gtvdiuqfyj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.guannengcc.top/gtyghbkxjl.html

[U11] Py：生成器表达式
来源：http://hz.hysaishi.cn/gttupzjipi.html

(x * 2 for x in arr)
来源：http://hz.jyoumei.cn/gteezyfwjj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.shuidangran.top/gtciwlrbeg.html

Counter(arr).most_common(3)
来源：http://hz.jinqigfzy.top/gtibaxnuvd.html

[U13] Py：固定长度队列
来源：http://hz.nanxuanxn.top/gtunkgdnvd.html

deque(maxlen=10)
来源：http://hz.zhongyouzk.top/gtaxlrdzio.html

[U14] Py：分组收集到列表
来源：http://hz.gotoacloud.top/gtoumaounf.html

defaultdict(list)
来源：http://hz.nanxuanxn.top/gtzivqbsxq.html

[U15] Py：高精度计时
来源：http://hz.dashuyun.cn/gtijwbfkfc.html

t = time.perf_counter()
来源：http://hz.jinqigufen.top/gtdpmvkvdf.html

[U16] Py：命令行参数解析
来源：http://hz.jqgfzy.top/gtbmmtthvr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.wangshuangyany.cn/gtepnncxaz.html

[U17] Py：初始化日志
来源：http://hz.ppjwa.cn/gthslbjrys.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shanyushiyangtech.top/gtbdxizstk.html

[U18] Py：预编译正则
来源：http://hz.chenzaomai.com/gtclzukkma.html

pat = re.compile(r"\d+")
来源：http://hz.yongpay.top/gtfgrzxkgj.html

[U19] Py：正则替换带回调
来源：http://hz.xingfuxueyuan.xyz/gtfehupxuz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yonumen.top/gtvmlsxhnn.html

[U20] Py：缓存函数结果
来源：http://hz.yvedp.cn/gtotqxhqzu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.hfpthk.cn/gtghhymqvb.html

[U21] Py：自定义上下文管理器
来源：http://hz.ywan-chungtsiang.top/gtqwspoial.html

@contextlib.contextmanager
来源：http://hz.xziqi.cn/gtokqigyoe.html

[U22] Py：矩阵转置
来源：http://hz.zhengqikj.top/gtbxqcmxmm.html

list(zip(*m))
来源：http://hz.vqdsnc.cn/gtiphelnux.html

[U23] Py：分块读取大文件
来源：http://hz.yuxming.cn/gtmmdbnlep.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yanxiufei.cn/gtqmjtelkn.html

[U24] Py：路径操作
来源：http://hz.yueranfly.top/gthvwuwpgh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinqigufen.top/gtikopinru.html

[U25] Py：CSV 按字典读
来源：http://hz.hfpthk.cn/gtvpschwhu.html

csv.DictReader(f)
来源：http://hz.kuanghao11.cn/gtyhadbmcg.html

[U26] Py：并发下载
来源：http://hz.hnqzz.top/gtcjdctinr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jiagoushi.top/gtzhxfrevf.html

[U27] Py：异步 HTTP
来源：http://hz.zhaomingkeji.xyz/gtptkhqgcs.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.feifeiyinyue.top/gtvmhljzuc.html

[U28] Py：类型别名
来源：http://hz.xuetiantiany.cn/gtvyqzryzq.html

UserId = int
来源：http://hz.guowangkeji.top/gtxrujgvsr.html

[U29] Py：属性校验
来源：http://hz.jinyuanbaomall.cn/gtkpogmygw.html

@property 与 @x.setter 配合
来源：http://hz.tian-w.cn/gtzkxwiwek.html

[U30] Py：数据类
来源：http://hz.ivvv.top/gtvgpwknyf.html

@dataclass(slots=True)
来源：http://hz.tanke756.top/gttizhekis.html

[U31] Py：单测
来源：http://hz.hysaishi.cn/gtrtkrwcue.html

python -m pytest -q
来源：http://hz.meibo888.top/gtozcoyfto.html

[U32] Py：代码格式化
来源：http://hz.zhixingplan.top/gtszaftdje.html

ruff format . && ruff check --fix .
来源：http://hz.gaohongyu789.top/gtvrcujajk.html

[U33] Py：打包发布
来源：http://hz.guowangkeji.top/gtxnnoiktb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shuidangran.top/gtaolzftue.html

[U34] Py：判断编码
来源：http://hz.hammf.cn/gtumvnkdhu.html

chardet.detect(raw)
来源：http://hz.mhx1999.top/gtjzkgiukp.html

[U35] Py：发送邮件
来源：http://hz.shuidangran.top/gtbdzumzwd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zdqjudy.top/gtlzpolqie.html

[U36] Py：定时任务
来源：http://hz.shuidangran.top/gtrjwhhzvz.html

schedule.every(10).minutes.do(job)
来源：http://hz.hongshengwenyu.top/gtzbhyixor.html

[U37] Py：读写 Excel
来源：http://hz.cucudq.cn/gtasjrguqy.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhoulong.xyz/gtisscotxr.html

[U38] Py：获取脚本所在目录
来源：http://hz.vqdsnc.cn/gthlfvcwwl.html

Path(__file__).resolve().parent
来源：http://hz.cdnleiting.top/gtuwqycgqe.html


<!-- 参考信息 -->