代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.redwolf501.top/gtuaxarbeb.html

[S25] C：内存拷贝
来源：http://hz.havefunace.top/gtwvadhusv.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtwzugjshf.html

[S26] C：内存清零
来源：http://hz.dianchejie.cn/gtgearyqyh.html

memset(a, 0, sizeof a);
来源：http://hz.cucudq.cn/gtmeeitbhk.html

[S27] C：定义常量
来源：http://hz.jinqigfzy.top/gtlysnsyfd.html

const double PI = 3.14159;
来源：http://hz.jinqigfzy.top/gtinluteya.html

[S28] C：静态变量
来源：http://hz.vqdsnc.cn/gtblasqgzc.html

static int counter = 0;
来源：http://hz.haohaochexian.top/gtclgmrdeu.html

[S29] C：变参函数
来源：http://hz.gaohongyu789.top/gtulqkrheb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gtmbwazbyc.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtjcaaoymg.html

#ifndef X_H
来源：http://hz.nwbrower.top/gtjyowibga.html

#define X_H
来源：http://hz.svipenyu.cn/gtznwzujlj.html

#endif
来源：http://hz.quarkkingdee.top/gtmghcwnfi.html

[S31] C++：Hello World
来源：http://hz.chenzaomai.com/gtnpwpkckh.html

#include <iostream>
来源：http://hz.zhongyouzk.top/gtnivglthi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.kuanghao11.cn/gtbaieonvb.html

[S32] C++：字符串
来源：http://hz.aibaodan.cn/gthtbubovn.html

std::string s = "hi";  s += "!";
来源：http://hz.bjfxy.top/gtbimitnim.html

[S33] C++：vector 增删
来源：http://hz.shuidangran.top/gturxjekgv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgfzy.top/gtosmvxiat.html

[S34] C++：遍历 vector
来源：http://hz.iojbl.cn/gtsplhxnfg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj20258.top/gtpkooiqes.html

[S35] C++：map
来源：http://hz.yongpay.top/gtqvimjipx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtlksgajlq.html

[S36] C++：unordered_map
来源：http://hz.nwbrower.top/gtmfphrirb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fzhhl.top/gtfeoftoaz.html

[S37] C++：set
来源：http://hz.gzhubu.top/gtzsiwgzmx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuanzx.com/gthlrvjcen.html

[S38] C++：排序
来源：http://hz.yongpay.top/gthlumhtqv.html

std::sort(v.begin(), v.end());
来源：http://hz.pengpengdd.cyou/gtmalmrczv.html

[S39] C++：自定义比较器排序
来源：http://hz.0kj1m.cn/gtthxiqtkz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cqqwz.cn/gtpknmtoxc.html

[S40] C++：查找元素
来源：http://hz.zycfv.cn/gtirkfwzbx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hongshengwenyu.top/gtzzuacqkq.html

[S41] C++：类与构造函数
来源：http://hz.jinyuanbaomall.cn/gtzdmklnlh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yongpay.top/gtdvbjkpip.html

[S42] C++：继承与虚函数
来源：http://hz.xuanzx.com/gtrcgfdqks.html

class B : public Base { public: void f() override {} };
来源：http://hz.sxryk.cn/gtptdrgued.html

[S43] C++：智能指针
来源：http://hz.hammf.cn/gtfcexqbme.html

auto p = std::make_unique<int>(5);
来源：http://hz.dashuyun.cn/gtqdelzcek.html

[S44] C++：引用传参
来源：http://hz.jqgufenzy.top/gtuwvgjtlu.html

void inc(int &x) { ++x; }
来源：http://hz.aizwys.cn/gtpnishkbt.html

[S45] C++：lambda
来源：http://hz.daxiang520.top/gtaafuqrxr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.52xcode.cn/gtilkvgwgm.html

[S46] C++：函数模板
来源：http://hz.aibaodan.cn/gtvfqepwwb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hywenlv.cn/gttufzilxp.html

[S47] C++：结构化绑定遍历
来源：http://hz.dianchejie.cn/gtzfreebvn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gotoacloud.top/gtzmgwnqpq.html

[S48] C++：逐行读文件
来源：http://hz.hysaishi.cn/gtqwrklhdy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangshuangyany.cn/gtnkowpfih.html

while (std::getline(in, line)) { }
来源：http://hz.xuetiantiany.cn/gtyyagbdaj.html

[S49] C++：写文件
来源：http://hz.jinqigfzy.top/gtfrpkkmzr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ydjk.org.cn/gtiztmzpnr.html

[S50] C++：格式化数字
来源：http://hz.yj20258.top/gtmauornou.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinqigfzy.top/gtcfurjzsv.html

[S51] C++：显式类型转换
来源：http://hz.jinqigfzy.top/gtiqpgtgdq.html

static_cast<double>(a) / b
来源：http://hz.guannengcc.top/gtopqqqmgt.html

[S52] C++：const 与 noexcept
来源：http://hz.zhengqikj.top/gtceesxbfo.html

int size() const noexcept { return n_; }
来源：http://hz.sweek.top/gtxhbmrjkl.html

[S53] C++：移动语义
来源：http://hz.daria6918.cn/gtzgsfsmwz.html

std::vector<int> w = std::move(v);
来源：http://hz.xuetiantiany.cn/gtvbrtxtok.html

[S54] C++：异常处理
来源：http://hz.shzxlz.cn/gtkhrcrlbp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuetiantiany.cn/gtuabeybtn.html

[S55] C++：结构化绑定
来源：http://hz.zhijiandao.cn/gtiymxxsev.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cdnleiting.top/gtqjjdwwgj.html

[S56] C++：optional
来源：http://hz.sufxvd.cn/gtqrflnkfo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dianchejie.cn/gtwuesevqi.html

[S57] C++：编译期常量
来源：http://hz.chenjidiqi.icu/gtussabhug.html

constexpr int N = 10;
来源：http://hz.jinqigufen.top/gtetbpxmsf.html

[S58] C++：命名空间
来源：http://hz.kuanghao11.cn/gtsalalqdy.html

namespace ns { int f() { return 1; } }
来源：http://hz.hywenlv.cn/gtqmemzwwq.html

[S59] C++：静态断言
来源：http://hz.yj20258.top/gtavnwhbvq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.snrcjt.cn/gtjgfgmlkp.html

[S60] C++：遍历并删除元素
来源：http://hz.aibaodan.cn/gtfluocoum.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.316326.xyz/gtlzldikbj.html

================================================================================
来源：http://hz.cqqwz.cn/gtazewqaph.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jyoumei.cn/gttmsqpqfn.html

================================================================================
来源：http://hz.mhx1999.top/gtaczmdldo.html

[T01] Kotlin：Hello World
来源：http://hz.yonumen.top/gtvaafksjq.html

println("Hello")
来源：http://hz.wangdashe.top/gtkfxrymuo.html

[T02] Kotlin：变量
来源：http://hz.daria6918.cn/gtxgwdzuvm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.tian-w.cn/gtllbimdti.html

[T03] Kotlin：字符串模板
来源：http://hz.nwbrower.top/gtltkygtpd.html

"值: $b"
来源：http://hz.yuanzhike.top/gtvdlxdpwx.html

[T04] Kotlin：空安全
来源：http://hz.havefunace.top/gtzesmnvmy.html

val n: String? = null;  n?.length
来源：http://hz.52xcode.cn/gtvdeoyipe.html

[T05] Kotlin：when 表达式
来源：http://hz.xziqi.cn/gtfqprogxf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.fengsongda.top/gthnhdvfex.html

[T06] Kotlin：集合映射
来源：http://hz.ivvv.top/gtuiwbduyb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jlsjyb.cn/gthydrkrcc.html

[T07] Kotlin：集合过滤
来源：http://hz.zhaomingkeji.xyz/gtjadroxtf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sxryk.cn/gtbdsfgbno.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangkeji.top/gtginzucnw.html

data class User(val name: String, val age: Int)
来源：http://hz.yanxiufei.cn/gtaryterxm.html

[T09] Kotlin：扩展函数
来源：http://hz.fzhhl.top/gtfzqsfhgj.html

fun String.exclaim() = this + "!"
来源：http://hz.snrcjt.cn/gtyreswucd.html

[T10] Kotlin：默认参数
来源：http://hz.shzxlz.cn/gttuxibaig.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zycfv.cn/gtghjulkyg.html

[T11] Kotlin：协程
来源：http://hz.guannengcc.top/gtyamkpnnk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.316326.xyz/gtftyyrghc.html

[T12] Kotlin：解构声明
来源：http://hz.jyoumei.cn/gtesouoyxw.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydjk.org.cn/gtdugshhcc.html

[T13] Kotlin：只读 Map
来源：http://hz.cqqwz.cn/gtxktdtswu.html

val m = mapOf("a" to 1)
来源：http://hz.gotoacloud.top/gtnvzrssfk.html

[T14] Kotlin：循环
来源：http://hz.yanxiufei.cn/gtadojszwg.html

for (i in 1..10) println(i)
来源：http://hz.havefunace.top/gtmrsyehbs.html

[T15] Kotlin：接口
来源：http://hz.jyoumei.cn/gtdvktveau.html

interface Shape { fun area(): Double }
来源：http://hz.aibaodan.cn/gtjmndcpor.html

[T16] Swift：Hello World
来源：http://hz.xuetiantiany.cn/gtpdumxtjb.html

print("Hello")
来源：http://hz.chenjidiqi.icu/gtsovsmbfy.html

[T17] Swift：变量与常量
来源：http://hz.yuxming.cn/gtxlgyzwaz.html

var a = 1;  let b = 2
来源：http://hz.52xcode.cn/gtiltnicmu.html

[T18] Swift：字符串插值
来源：http://hz.hammf.cn/gtijbdvmml.html

"值: \(b)"
来源：http://hz.sysykeji.top/gtopnrneal.html

[T19] Swift：可选绑定
来源：http://hz.wangdashe.top/gthrulfbzb.html

if let n = opt { print(n) }
来源：http://hz.0kj1m.cn/gthddpxber.html

[T20] Swift：数组操作
来源：http://hz.wangshuangyany.cn/gtkuzqlsgq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sysykeji.top/gtyxqmjtis.html

[T21] Swift：遍历
来源：http://hz.yongpay.top/gtgnehblnw.html

for x in a { print(x) }
来源：http://hz.hongshengwenyu.top/gtbzpiohxw.html

[T22] Swift：字典
来源：http://hz.andypj.xyz/gtnrcdqvzn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shangyingyoupin.top/gtqiixjpkg.html

[T23] Swift：函数
来源：http://hz.xziqi.cn/gtkujnkaiq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cdnleiting.top/gtixveyubx.html

[T24] Swift：闭包
来源：http://hz.xingfuxueyuan.xyz/gtismjhrry.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hammf.cn/gtwpticryx.html

[T25] Swift：结构体
来源：http://hz.wangdashe.top/gteltopelx.html

struct P { var x: Int }
来源：http://hz.xinyue.icu/gtszcmwhbf.html

[T26] Swift：类与重写
来源：http://hz.birdmap.top/gtgswthony.html

class A: Base { override func f() {} }
来源：http://hz.shangyingyoupin.top/gtcbewhjwb.html

[T27] Swift：错误处理
来源：http://hz.cdnleiting.top/gtyxdorous.html

do { try f() } catch { print(error) }
来源：http://hz.sufxvd.cn/gtfvvyhbqm.html

[T28] Swift：枚举
来源：http://hz.vqdsnc.cn/gthtxfgsug.html

enum Color { case red, green }
来源：http://hz.yj20258888.top/gtjnbvuroz.html

[T29] Swift：guard 提前返回
来源：http://hz.birdmap.top/gtepjjibav.html

guard let x = opt else { return }
来源：http://hz.ppjwa.cn/gttplvxsrc.html

[T30] Swift：协议
来源：http://hz.xziqi.cn/gtefrcechk.html

protocol Shape { func area() -> Double }
来源：http://hz.sxryk.cn/gtuyxakwbn.html

[T31] Lua：Hello World
来源：http://hz.smart0.xyz/gtuasyuqbd.html

print("Hello")
来源：http://hz.hammf.cn/gthuksczaq.html

[T32] Lua：局部变量
来源：http://hz.ydzc1.top/gtobmlaest.html

local a = 1
来源：http://hz.birdmap.top/gtdquynfyc.html

[T33] Lua：表（数组）
来源：http://hz.yj20258888.top/gtstkzvpsb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xziqi.cn/gteqweqipn.html

[T34] Lua：遍历表
来源：http://hz.daria6918.cn/gtoabqmqhp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xziqi.cn/gtosgjzcol.html

[T35] Lua：字典表
来源：http://hz.0kj1m.cn/gtnhiydupc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.iojbl.cn/gtvkliuobr.html

[T36] Lua：函数
来源：http://hz.xylfe.cn/gtzzacjxcd.html

function add(a, b) return a + b end
来源：http://hz.yangfankeji.com/gtwfauwxnt.html

[T37] Lua：字符串拼接
来源：http://hz.shuidangran.top/gtbmpyyzfh.html

"a" .. "b"
来源：http://hz.shanyushiyangkeji.top/gtcxjiwmdh.html

[T38] Lua：条件
来源：http://hz.cucudq.cn/gtrqvyqsra.html

if x > 0 then print("正") end
来源：http://hz.tian-w.cn/gtfquixfot.html

[T39] Lua：模式匹配
来源：http://hz.hywenlv.cn/gtputkczsb.html

string.find(s, "%d+")
来源：http://hz.feifeiyinyue.top/gtizeksbys.html

[T40] Lua：元表
来源：http://hz.xuanzx.com/gtpzacuvmr.html

setmetatable({}, { __index = base })
来源：http://hz.hammf.cn/gttttedilu.html

[T41] Perl：Hello World
来源：http://hz.tianlin.xyz/gtqfldchaz.html

print "Hello\n";
来源：http://hz.ivvv.top/gttnnnyaha.html

[T42] Perl：变量类型
来源：http://hz.sufxvd.cn/gtsgvegvke.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.aizwys.cn/gtrxjjndsj.html

[T43] Perl：字符串插值
来源：http://hz.tian-w.cn/gtryotlstx.html

"值: $a"
来源：http://hz.fengsongda.top/gtpuohbrqd.html

[T44] Perl：条件
来源：http://hz.yj202588.top/gtddckaacg.html

if ($a > 0) { print "正"; }
来源：http://hz.wangdashe.top/gthdawndyg.html

[T45] Perl：数组遍历
来源：http://hz.snrcjt.cn/gthecvmpnl.html

for my $x (@arr) { print $x; }
来源：http://hz.dashuyun.cn/gtnkcbhuyq.html

[T46] Perl：哈希操作
来源：http://hz.andypj.xyz/gtymzaoqgb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gaohongyu789.top/gtroqtimtj.html

[T47] Perl：正则捕获
来源：http://hz.xuetiantiany.cn/gtowiaxixb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.316326.xyz/gthfbsndxt.html

[T48] Perl：正则替换
来源：http://hz.aibaodan.cn/gtcyvbbxai.html

$s =~ s/old/new/g;
来源：http://hz.yj20258888.top/gtwjddanch.html

[T49] Perl：函数
来源：http://hz.shangyingyoupin.top/gteuqvdeqc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hfpthk.cn/gtzacqszbq.html

[T50] Perl：逐行读文件
来源：http://hz.zycfv.cn/gttykfllxt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.birdmap.top/gtyrhiteqz.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.nwbrower.top/gtorqngioc.html

[T51] Scala：Hello World
来源：http://hz.iojbl.cn/gtaphbhxwc.html

println("Hello")
来源：http://hz.xziqi.cn/gtansshcuz.html

[T52] Scala：变量
来源：http://hz.smart0.xyz/gtelguvtru.html

val a = 1;  var b = 2
来源：http://hz.zhijiandao.cn/gtkmxfdjys.html

[T53] Scala：字符串插值
来源：http://hz.shangyingyoupin.top/gtcnlsdblp.html

s"值: $b"
来源：http://hz.feifeiyinyue.top/gtrecvynzy.html

[T54] Scala：集合映射
来源：http://hz.316326.xyz/gtlwcfyzcl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.dianchejie.cn/gtppthgyjy.html

[T55] Scala：集合过滤
来源：http://hz.guannengcc.top/gtbpwzxvlq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.vqdsnc.cn/gtkaahfahr.html

[T56] Scala：样例类
来源：http://hz.bjfxy.top/gthcvbrqhe.html

case class User(name: String, age: Int)
来源：http://hz.chenjidiqi.icu/gterxyvmop.html

[T57] Scala：模式匹配
来源：http://hz.cucudq.cn/gtqnwyjqzu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ydzc1.top/gtbpkkwsbt.html

[T58] Scala：函数定义
来源：http://hz.fzhhl.top/gtbpekgwvu.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jqgfzy.top/gtruidjvam.html

[T59] Scala：循环
来源：http://hz.tanke756.top/gtfisojnmm.html

for (i <- 1 to 10) println(i)
来源：http://hz.316326.xyz/gtmmlyecbe.html

[T60] Scala：折叠
来源：http://hz.cqqwz.cn/gtzovesseg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ehwqpu.com/gtsxpgyqnx.html

================================================================================
来源：http://hz.nanxinkj.top/gtftiudmrp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.ywan-chungtsiang.top/gtdllvcjso.html

================================================================================
来源：http://hz.guowangkeji.top/gtqafjaoyy.html

[U01] Py：创建虚拟环境
来源：http://hz.xinyue.icu/gtfxodgswn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.smart0.xyz/gtlumvkmmj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yj20258.top/gtgmxyexab.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.andypj.xyz/gtqtlrfijg.html

[U03] Py：加载 .env 配置
来源：http://hz.jlsjyb.cn/gtcaycukoq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.meibo888.top/gtggzefdhq.html

[U04] Py：变量调试打印
来源：http://hz.sweek.top/gtrnnnboqj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.tanke756.top/gtvhkysdmt.html

[U05] Py：列表去重且保序
来源：http://hz.ydjk.org.cn/gtgudtgfpm.html

list(dict.fromkeys(arr))
来源：http://hz.tianlin.xyz/gtetgyrqim.html

[U06] Py：合并两个字典
来源：http://hz.haohaochexian.top/gtulbfydqi.html

{**a, **b}
来源：http://hz.jyoumei.cn/gtaniqbxij.html

[U07] Py：反转字典键值
来源：http://hz.ydjk.org.cn/gtlmegzulb.html

{v: k for k, v in d.items()}
来源：http://hz.zhaomingkeji.xyz/gtvkhwonho.html

[U08] Py：展平二维列表
来源：http://hz.aizwys.cn/gteslidwat.html

[y for x in nested for y in x]
来源：http://hz.ivvv.top/gtyznukqkt.html

[U09] Py：字典取最大值的键
来源：http://hz.jqgfzy.top/gtnzlggnly.html

max(d, key=d.get)
来源：http://hz.cheryme.top/gtjarqneoy.html

[U10] Py：按值排序字典
来源：http://hz.jinqigfzy.top/gthmfzsocy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shangyingyoupin.top/gthhwcerqd.html

[U11] Py：生成器表达式
来源：http://hz.ehwqpu.com/gtaixvhbdt.html

(x * 2 for x in arr)
来源：http://hz.jqgfzy.top/gtstvseypj.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.svipenyu.cn/gtdbnqozqx.html

Counter(arr).most_common(3)
来源：http://hz.nwbrower.top/gtlfladwtg.html

[U13] Py：固定长度队列
来源：http://hz.yuxming.cn/gtnszkhatd.html

deque(maxlen=10)
来源：http://hz.0kj1m.cn/gtbhhyjsmy.html

[U14] Py：分组收集到列表
来源：http://hz.cdnleiting.top/gtpduqlbdl.html

defaultdict(list)
来源：http://hz.zycfv.cn/gttarynciz.html

[U15] Py：高精度计时
来源：http://hz.hammf.cn/gtnxuanzhq.html

t = time.perf_counter()
来源：http://hz.jianghu66.top/gtkhkprzrh.html

[U16] Py：命令行参数解析
来源：http://hz.hnqzz.top/gtleysgvcu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.jlsjyb.cn/gtzuwoozkt.html

[U17] Py：初始化日志
来源：http://hz.andypj.xyz/gtcvceducd.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.shuidangran.top/gtaupdbozn.html

[U18] Py：预编译正则
来源：http://hz.bjfxy.top/gtbhkzkyop.html

pat = re.compile(r"\d+")
来源：http://hz.wangshuangyany.cn/gtrvbnuoxb.html

[U19] Py：正则替换带回调
来源：http://hz.svipenyu.cn/gtaxfdpeyp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.chenzaomai.com/gtzvckuwee.html

[U20] Py：缓存函数结果
来源：http://hz.chenjidiqi.icu/gthvryytql.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xinyue.icu/gtguybdhaw.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhoulong.xyz/gtugqtrnio.html

@contextlib.contextmanager
来源：http://hz.cheryme.top/gtmhkkonzk.html

[U22] Py：矩阵转置
来源：http://hz.xuetiantiany.cn/gtyagioqnb.html

list(zip(*m))
来源：http://hz.aibaodan.cn/gtgdbssiwp.html

[U23] Py：分块读取大文件
来源：http://hz.daxiang520.top/gtailazvag.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.wangshuangyany.cn/gtjdjbmnjy.html

[U24] Py：路径操作
来源：http://hz.yangfankeji.com/gtaktlslom.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.smart0.xyz/gtorlkkiip.html

[U25] Py：CSV 按字典读
来源：http://hz.ydzc1.top/gttxmsfxem.html

csv.DictReader(f)
来源：http://hz.hysaishi.cn/gtjlubvnzx.html

[U26] Py：并发下载
来源：http://hz.yj20258888.top/gtjzufkzxl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhiwuduotai.top/gtrbgzejux.html

[U27] Py：异步 HTTP
来源：http://hz.chenlongwang.top/gtqucnafxj.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hammf.cn/gtgfkjgmfs.html

[U28] Py：类型别名
来源：http://hz.jqgufenzy.top/gtwqkarnnp.html

UserId = int
来源：http://hz.pycfn.com/gtepdfwxua.html

[U29] Py：属性校验
来源：http://hz.tianlin.xyz/gtnttelihq.html

@property 与 @x.setter 配合
来源：http://hz.jlsjyb.cn/gtutfjvpqf.html

[U30] Py：数据类
来源：http://hz.chenjidiqi.icu/gtmeuapqps.html

@dataclass(slots=True)
来源：http://hz.fengsongda.top/gtpplmqplb.html

[U31] Py：单测
来源：http://hz.yj202588.top/gtrnrgzwqv.html

python -m pytest -q
来源：http://hz.sysykeji.top/gtjuilphft.html

[U32] Py：代码格式化
来源：http://hz.jinqigfzy.top/gtonlbesfa.html

ruff format . && ruff check --fix .
来源：http://hz.xingfuxueyuan.xyz/gtkreixxej.html

[U33] Py：打包发布
来源：http://hz.havefunace.top/gtxomdbuij.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jlsjyb.cn/gtrcfngpfw.html

[U34] Py：判断编码
来源：http://hz.xinyue.icu/gtjfjmmbyl.html

chardet.detect(raw)
来源：http://hz.chenlongwang.top/gtrgnwbtkn.html

[U35] Py：发送邮件
来源：http://hz.jlsjyb.cn/gtqjfsbfdx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.tian-w.cn/gtksqvjrzk.html

[U36] Py：定时任务
来源：http://hz.jiagoushi.top/gtdvhwkbsg.html

schedule.every(10).minutes.do(job)
来源：http://hz.chenlongwang.top/gtyxonujhr.html

[U37] Py：读写 Excel
来源：http://hz.cqqwz.cn/gtfxqpoeoh.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yangfankeji.com/gtdvxmpkoe.html

[U38] Py：获取脚本所在目录
来源：http://hz.daria6918.cn/gtqoxihybf.html

Path(__file__).resolve().parent
来源：http://hz.snrcjt.cn/gtsqvgungd.html

[U39] Py：判断是否在交互环境
来源：http://hz.xuanzx.com/gtjohuzwuw.html

sys.stdout.isatty()
来源：http://hz.sxryk.cn/gtmkmoujuc.html

[U40] Py：打印到标准错误
来源：http://hz.shuidangran.top/gtfwbnaeuh.html

print("err", file=sys.stderr)
来源：http://hz.zhiwuduotai.top/gtrdatdnsv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shangyingyoupin.top/gtdneeefwe.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.gogol.net.cn/gtemlqafqw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hfpthk.cn/gtuwqfufjw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hfpthk.cn/gtafsenrgo.html

[U43] PHP：声明命名空间
来源：http://hz.hysaishi.cn/gtqlxiaorn.html

namespace App\Http;
来源：http://hz.zycfv.cn/gtxvbfasyb.html

[U44] PHP：开启严格类型
来源：http://hz.nanxinkj.top/gtyksgqyro.html

declare(strict_types=1);
来源：http://hz.xingfuxueyuan.xyz/gtwvhaiism.html

[U45] PHP：类型声明与返回类型
来源：http://hz.52xcode.cn/gtlnnrlbkx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shuidangran.top/gtrehvyqpj.html

[U46] PHP：可空类型
来源：http://hz.jqgufenzy.top/gtgyvpogmq.html

?string $name = null
来源：http://hz.jyoumei.cn/gtofwopbrt.html

[U47] PHP：联合类型
来源：http://hz.hammf.cn/gtdeyskoqo.html

int|string $id
来源：http://hz.vqdsnc.cn/gtbwbqhdua.html

[U48] PHP：纯枚举
来源：http://hz.ywan-chungtsiang.top/gtieomdxva.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.feifeiyinyue.top/gtpaxadsxs.html


<!-- 参考信息 -->