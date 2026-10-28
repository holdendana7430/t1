代发 wailian999

static int counter = 0;
来源：http://hz.ywan-chungtsiang.top/gthqaegpla.html

[S29] C：变参函数
来源：http://hz.shanyushiyangkeji.top/gtkwmrwvmz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhaomingkeji.xyz/gtcqlffbdc.html

[S30] C：头文件保护
来源：http://hz.nanxuanxn.top/gthiqweuom.html

#ifndef X_H
来源：http://hz.zhengqikj.top/gtmapigmas.html

#define X_H
来源：http://hz.sufxvd.cn/gtmyidectq.html

#endif
来源：http://hz.chenzaomai.com/gtmnupwwqj.html

[S31] C++：Hello World
来源：http://hz.wangdashe.top/gtgkbwinmm.html

#include <iostream>
来源：http://hz.gotoacloud.top/gtmequrnel.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yangfankeji.com/gtrxxzpkxv.html

[S32] C++：字符串
来源：http://hz.gaohongyu789.top/gtrtabhnoe.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangkeji.top/gtkumrhlfd.html

[S33] C++：vector 增删
来源：http://hz.havefunace.top/gtmuekiiuf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yonumen.top/gtvgrntrtv.html

[S34] C++：遍历 vector
来源：http://hz.yangfankeji.com/gtjqnbevyv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hnqzz.top/gtfehcrrwx.html

[S35] C++：map
来源：http://hz.ydjk.org.cn/gtwvmnanog.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtswkpwncf.html

[S36] C++：unordered_map
来源：http://hz.yuanzhike.top/gtjdozbqlt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenzaomai.com/gtcwsargxe.html

[S37] C++：set
来源：http://hz.hfpthk.cn/gtuxyfqfep.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gaohongyu789.top/gtnoaeuoyq.html

[S38] C++：排序
来源：http://hz.sxryk.cn/gtmelbjpvp.html

std::sort(v.begin(), v.end());
来源：http://hz.jinghuilouyu.cn/gtkklfetfi.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangtech.top/gtdabwjgbr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sysykeji.top/gtjtczcpum.html

[S40] C++：查找元素
来源：http://hz.aizwys.cn/gtpifionxk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gtcqwnwcez.html

[S41] C++：类与构造函数
来源：http://hz.birdmap.top/gtllrbzsym.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xylfe.cn/gthgoziuhd.html

[S42] C++：继承与虚函数
来源：http://hz.wangshuangyany.cn/gtpsztuvji.html

class B : public Base { public: void f() override {} };
来源：http://hz.smart0.xyz/gtbdsehdev.html

[S43] C++：智能指针
来源：http://hz.ehwqpu.com/gtjyqsrlin.html

auto p = std::make_unique<int>(5);
来源：http://hz.xuanzx.com/gtiriaudrk.html

[S44] C++：引用传参
来源：http://hz.daria6918.cn/gtohkznnev.html

void inc(int &x) { ++x; }
来源：http://hz.vqdsnc.cn/gtngznupys.html

[S45] C++：lambda
来源：http://hz.shuidangran.top/gtjayxsuii.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinghuilouyu.cn/gtwkqpaoee.html

[S46] C++：函数模板
来源：http://hz.zhaomingkeji.xyz/gtwzljupzv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.9152youxi.cn/gtmljjbnse.html

[S47] C++：结构化绑定遍历
来源：http://hz.birdmap.top/gtydiwnbir.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hfpthk.cn/gtndkzuuqa.html

[S48] C++：逐行读文件
来源：http://hz.feifeiyinyue.top/gturrbjvyo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gotoacloud.top/gtdeemlbqr.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangkeji.top/gtwlsvvkkq.html

[S49] C++：写文件
来源：http://hz.tian-w.cn/gtwepibssm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.havefunace.top/gtzcfckrrs.html

[S50] C++：格式化数字
来源：http://hz.yj202588.top/gtgvnqkpfy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ybcxt.top/gtkbryprls.html

[S51] C++：显式类型转换
来源：http://hz.ydjk.org.cn/gtsfvibvgt.html

static_cast<double>(a) / b
来源：http://hz.ybcxt.top/gtwisnamfu.html

[S52] C++：const 与 noexcept
来源：http://hz.yueranfly.top/gthkqjxjyt.html

int size() const noexcept { return n_; }
来源：http://hz.wangdashe.top/gtkferfnhp.html

[S53] C++：移动语义
来源：http://hz.xuetiantiany.cn/gtnxxskgir.html

std::vector<int> w = std::move(v);
来源：http://hz.havefunace.top/gtjutpechv.html

[S54] C++：异常处理
来源：http://hz.guowangkeji.top/gtsimspgrr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj202588.top/gtnqiduntb.html

[S55] C++：结构化绑定
来源：http://hz.jinqigufen.top/gtgnftsacu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ydjk.org.cn/gtqytaylid.html

[S56] C++：optional
来源：http://hz.zhongyouzk.top/gtxebeeqfg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ywan-chungtsiang.top/gtdfcxluif.html

[S57] C++：编译期常量
来源：http://hz.xuanzx.com/gtfebqurae.html

constexpr int N = 10;
来源：http://hz.jlsjyb.cn/gtstqhwhxv.html

[S58] C++：命名空间
来源：http://hz.gotoacloud.top/gtvyakndob.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhijiandao.cn/gtzipsdfru.html

[S59] C++：静态断言
来源：http://hz.xylfe.cn/gtovyheqbf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydjk.org.cn/gtlmnhvzkw.html

[S60] C++：遍历并删除元素
来源：http://hz.yj202588.top/gtnxbntjgp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.fengsongda.top/gtpzbsxgae.html

================================================================================
来源：http://hz.dashuyun.cn/gtuuhzvryy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sweek.top/gttpiaddja.html

================================================================================
来源：http://hz.iojbl.cn/gtoqtjdusj.html

[T01] Kotlin：Hello World
来源：http://hz.cdnleiting.top/gtjalwxnsq.html

println("Hello")
来源：http://hz.ehwqpu.com/gtqdaktkjv.html

[T02] Kotlin：变量
来源：http://hz.ywan-chungtsiang.top/gtyfvnpnnd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.kuanghao11.cn/gtcvmybunj.html

[T03] Kotlin：字符串模板
来源：http://hz.yuxming.cn/gtwzjsczoc.html

"值: $b"
来源：http://hz.jinyuanbaomall.cn/gtcvkbbesr.html

[T04] Kotlin：空安全
来源：http://hz.birdmap.top/gtorrnjtga.html

val n: String? = null;  n?.length
来源：http://hz.feifeiyinyue.top/gtahdpowrw.html

[T05] Kotlin：when 表达式
来源：http://hz.yongpay.top/gtcdnmbxur.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ywan-chungtsiang.top/gtketioqcw.html

[T06] Kotlin：集合映射
来源：http://hz.yuanzhike.top/gtzgnvogeq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhixingplan.top/gtcgaylbjm.html

[T07] Kotlin：集合过滤
来源：http://hz.redwolf501.top/gtlamnyvpp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yonumen.top/gtputbsqel.html

[T08] Kotlin：数据类
来源：http://hz.c1oappe.top/gtapdbpxhp.html

data class User(val name: String, val age: Int)
来源：http://hz.tian-w.cn/gtaiinzzwy.html

[T09] Kotlin：扩展函数
来源：http://hz.52xcode.cn/gtalauabcw.html

fun String.exclaim() = this + "!"
来源：http://hz.jinghuilouyu.cn/gtselpwcaf.html

[T10] Kotlin：默认参数
来源：http://hz.dashuyun.cn/gtluwohtpi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daxiang520.top/gtirosgmfr.html

[T11] Kotlin：协程
来源：http://hz.haohaochexian.top/gtjgaghhar.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.dashuyun.cn/gtluxotlhc.html

[T12] Kotlin：解构声明
来源：http://hz.shanyushiyangkeji.top/gtgcsmykhx.html

val (a, b) = Pair(1, 2)
来源：http://hz.shuidangran.top/gtuqndwtpb.html

[T13] Kotlin：只读 Map
来源：http://hz.bjfxy.top/gtvsqgdmqh.html

val m = mapOf("a" to 1)
来源：http://hz.cqqwz.cn/gtrgqidngf.html

[T14] Kotlin：循环
来源：http://hz.hnqzz.top/gtuvuytrnr.html

for (i in 1..10) println(i)
来源：http://hz.fzhhl.top/gtariejcds.html

[T15] Kotlin：接口
来源：http://hz.zhaomingkeji.xyz/gtuspwrwtn.html

interface Shape { fun area(): Double }
来源：http://hz.yuanzhike.top/gtzykaupwd.html

[T16] Swift：Hello World
来源：http://hz.yuanzhike.top/gtgvblrpet.html

print("Hello")
来源：http://hz.vqdsnc.cn/gtnsjavzkc.html

[T17] Swift：变量与常量
来源：http://hz.jyoumei.cn/gteyzpdsba.html

var a = 1;  let b = 2
来源：http://hz.vqdsnc.cn/gtlkezfyni.html

[T18] Swift：字符串插值
来源：http://hz.zhoulong.xyz/gtprkxkavm.html

"值: \(b)"
来源：http://hz.zhixingplan.top/gtawlaekpb.html

[T19] Swift：可选绑定
来源：http://hz.jiagoushi.top/gtnkuungxo.html

if let n = opt { print(n) }
来源：http://hz.tianlin.xyz/gtoibydoam.html

[T20] Swift：数组操作
来源：http://hz.birdmap.top/gtzgklzrlv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sxryk.cn/gtptebyuzy.html

[T21] Swift：遍历
来源：http://hz.52xcode.cn/gtophmazyj.html

for x in a { print(x) }
来源：http://hz.zhixingplan.top/gtzepiqivu.html

[T22] Swift：字典
来源：http://hz.jqgfzy.top/gtsvfissnm.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cucudq.cn/gtbxdwpssm.html

[T23] Swift：函数
来源：http://hz.aibaodan.cn/gttshmspzc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigufen.top/gthmyejcor.html

[T24] Swift：闭包
来源：http://hz.kuanghao11.cn/gthnjianmx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuanzhike.top/gtmukzxqtw.html

[T25] Swift：结构体
来源：http://hz.redwolf501.top/gtuhdsuczb.html

struct P { var x: Int }
来源：http://hz.iojbl.cn/gtggvtvclu.html

[T26] Swift：类与重写
来源：http://hz.aizwys.cn/gtnmkwiphu.html

class A: Base { override func f() {} }
来源：http://hz.hnqzz.top/gtpenppict.html

[T27] Swift：错误处理
来源：http://hz.hnqzz.top/gtimrsmaoo.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigfzy.top/gtuklevbbx.html

[T28] Swift：枚举
来源：http://hz.feifeiyinyue.top/gtywgpnaxx.html

enum Color { case red, green }
来源：http://hz.wangdashe.top/gtmnmhmqqm.html

[T29] Swift：guard 提前返回
来源：http://hz.zhoulong.xyz/gtwfnrtcsg.html

guard let x = opt else { return }
来源：http://hz.nanxinkj.top/gtzvbyuobu.html

[T30] Swift：协议
来源：http://hz.yongpay.top/gtauycshin.html

protocol Shape { func area() -> Double }
来源：http://hz.tian-w.cn/gtyexsbfjl.html

[T31] Lua：Hello World
来源：http://hz.feifeiyinyue.top/gthafwgsgc.html

print("Hello")
来源：http://hz.jinghuilouyu.cn/gtueunonyu.html

[T32] Lua：局部变量
来源：http://hz.shanyushiyangkeji.top/gtqvgqijtr.html

local a = 1
来源：http://hz.xuetiantiany.cn/gthjqcngrb.html

[T33] Lua：表（数组）
来源：http://hz.cdnleiting.top/gtsxfyooja.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.andypj.xyz/gtshrmcusi.html

[T34] Lua：遍历表
来源：http://hz.kuanghao11.cn/gtahuuciyr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hnxiangtu.top/gtlqsvnhia.html

[T35] Lua：字典表
来源：http://hz.jqgufenzy.top/gtqlsyghjf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sxryk.cn/gtlgsazdoi.html

[T36] Lua：函数
来源：http://hz.zhengqikj.top/gtedvuyeux.html

function add(a, b) return a + b end
来源：http://hz.chenjidiqi.icu/gtdwfrusmv.html

[T37] Lua：字符串拼接
来源：http://hz.cashguo.top/gtwivhvfwp.html

"a" .. "b"
来源：http://hz.yangfankeji.com/gtweutvxzt.html

[T38] Lua：条件
来源：http://hz.fzhhl.top/gtxmpszrgk.html

if x > 0 then print("正") end
来源：http://hz.yueranfly.top/gtzqilhogo.html

[T39] Lua：模式匹配
来源：http://hz.jinqigfzy.top/gtyeiipbdc.html

string.find(s, "%d+")
来源：http://hz.ywan-chungtsiang.top/gtqayshqqb.html

[T40] Lua：元表
来源：http://hz.zhoulong.xyz/gtcsusvqlv.html

setmetatable({}, { __index = base })
来源：http://hz.yanxiufei.cn/gtlfrhxmyz.html

[T41] Perl：Hello World
来源：http://hz.havefunace.top/gtfizhufmt.html

print "Hello\n";
来源：http://hz.yvedp.cn/gtmwroeris.html

[T42] Perl：变量类型
来源：http://hz.hnqzz.top/gtogsrncni.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sxryk.cn/gtvpjxwauc.html

[T43] Perl：字符串插值
来源：http://hz.yonumen.top/gthsfgfmpr.html

"值: $a"
来源：http://hz.xinyue.icu/gtakfoxkyh.html

[T44] Perl：条件
来源：http://hz.sysykeji.top/gttnsroowf.html

if ($a > 0) { print "正"; }
来源：http://hz.chenlongwang.top/gttmjdsost.html

[T45] Perl：数组遍历
来源：http://hz.sxryk.cn/gtzeyhtqlu.html

for my $x (@arr) { print $x; }
来源：http://hz.shanyushiyangkeji.top/gtgkhuyktk.html

[T46] Perl：哈希操作
来源：http://hz.jqgufenzy.top/gtcbsefxbv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.gotoacloud.top/gtqcciqile.html

[T47] Perl：正则捕获
来源：http://hz.yonumen.top/gtggsijent.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xziqi.cn/gtuygdrwur.html

[T48] Perl：正则替换
来源：http://hz.hnqzz.top/gtknagpbso.html

$s =~ s/old/new/g;
来源：http://hz.guowangkeji.top/gtsjlfrasb.html

[T49] Perl：函数
来源：http://hz.xuetiantiany.cn/gtwroplshl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shuidangran.top/gtmxosqsbe.html

[T50] Perl：逐行读文件
来源：http://hz.shuidangran.top/gtcfxdiwxl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.chenjidiqi.icu/gtmebbhnrc.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shanyushiyangkeji.top/gtivgvbdkx.html

[T51] Scala：Hello World
来源：http://hz.zhijiandao.cn/gtrrydtcbs.html

println("Hello")
来源：http://hz.sysykeji.top/gtkevtoxie.html

[T52] Scala：变量
来源：http://hz.jiagoushi.top/gtqoaklrjq.html

val a = 1;  var b = 2
来源：http://hz.ivvv.top/gtejhigcew.html

[T53] Scala：字符串插值
来源：http://hz.mhx1999.top/gtlmdjosax.html

s"值: $b"
来源：http://hz.wangshuangyany.cn/gtxzsmmpqi.html

[T54] Scala：集合映射
来源：http://hz.ywan-chungtsiang.top/gtmpigdtpv.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.ybcxt.top/gtsadllvnv.html

[T55] Scala：集合过滤
来源：http://hz.xylfe.cn/gtyahbvsql.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tanke756.top/gtlqngezrw.html

[T56] Scala：样例类
来源：http://hz.yongpay.top/gteosnozmy.html

case class User(name: String, age: Int)
来源：http://hz.yj20258888.top/gtvjeiavyi.html

[T57] Scala：模式匹配
来源：http://hz.xziqi.cn/gthcmfiwln.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ppjwa.cn/gtopuuiyoc.html

[T58] Scala：函数定义
来源：http://hz.ydzc1.top/gthwhdgvhs.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zycfv.cn/gtrxeknzyw.html

[T59] Scala：循环
来源：http://hz.hysaishi.cn/gtdtpuzvfm.html

for (i <- 1 to 10) println(i)
来源：http://hz.snrcjt.cn/gtziafwyfd.html

[T60] Scala：折叠
来源：http://hz.zhiwuduotai.top/gttxmewaih.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jlsjyb.cn/gtsrkwdmze.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtgasqakzy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenlongwang.top/gtcebuovkg.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtovnbakhe.html

[U01] Py：创建虚拟环境
来源：http://hz.daxiang520.top/gtnadwyotb.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ywan-chungtsiang.top/gtcjonhkcv.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xuanzx.com/gtsyiduupw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.9152youxi.cn/gtraetdvox.html

[U03] Py：加载 .env 配置
来源：http://hz.daxiang520.top/gtblqazgjt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.bjfxy.top/gtbulkggsc.html

[U04] Py：变量调试打印
来源：http://hz.gzhubu.top/gtntbdhrlm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jianghu66.top/gthaawwgrh.html

[U05] Py：列表去重且保序
来源：http://hz.gzhubu.top/gtupddvlde.html

list(dict.fromkeys(arr))
来源：http://hz.sxryk.cn/gtrlhlmvgd.html

[U06] Py：合并两个字典
来源：http://hz.daxiang520.top/gtzchpeglx.html

{**a, **b}
来源：http://hz.nanxuanxn.top/gtgxpjbqsu.html

[U07] Py：反转字典键值
来源：http://hz.zhoulong.xyz/gtzdouhjnk.html

{v: k for k, v in d.items()}
来源：http://hz.cucudq.cn/gtdbmlwhys.html

[U08] Py：展平二维列表
来源：http://hz.shangyingyoupin.top/gtjcpxrxbb.html

[y for x in nested for y in x]
来源：http://hz.smart0.xyz/gtevfzyens.html

[U09] Py：字典取最大值的键
来源：http://hz.nanxuanxn.top/gtqpxqdvqs.html

max(d, key=d.get)
来源：http://hz.chenlongwang.top/gtjxsczgcs.html

[U10] Py：按值排序字典
来源：http://hz.yangfankeji.com/gtcbhjqkrd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shuidangran.top/gtcgerffxb.html

[U11] Py：生成器表达式
来源：http://hz.hnxiangtu.top/gtzaefvpve.html

(x * 2 for x in arr)
来源：http://hz.kuanghao11.cn/gtuvhpnwrd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yangfankeji.com/gtpwhdrmue.html

Counter(arr).most_common(3)
来源：http://hz.aibaodan.cn/gtncevqcph.html

[U13] Py：固定长度队列
来源：http://hz.mhx1999.top/gtiumnpxty.html

deque(maxlen=10)
来源：http://hz.jiagoushi.top/gtdawloamt.html

[U14] Py：分组收集到列表
来源：http://hz.yvedp.cn/gtdnhwqvxx.html

defaultdict(list)
来源：http://hz.jinyuanbaomall.cn/gtijfgqdws.html

[U15] Py：高精度计时
来源：http://hz.wangdashe.top/gthkmqprcd.html

t = time.perf_counter()
来源：http://hz.feifeiyinyue.top/gtovablscn.html

[U16] Py：命令行参数解析
来源：http://hz.vqdsnc.cn/gtcnzxzqms.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.birdmap.top/gtgwxqkdtg.html

[U17] Py：初始化日志
来源：http://hz.tian-w.cn/gtypcfkzbs.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.cqqwz.cn/gtuwdsurlv.html

[U18] Py：预编译正则
来源：http://hz.wangshuangyany.cn/gtuqcplixe.html

pat = re.compile(r"\d+")
来源：http://hz.yonumen.top/gtldbadmix.html

[U19] Py：正则替换带回调
来源：http://hz.316326.xyz/gtukdovdar.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.wangshuangyany.cn/gtkhcjqpxm.html

[U20] Py：缓存函数结果
来源：http://hz.cucudq.cn/gtrytrhgum.html

@functools.lru_cache(maxsize=None)
来源：http://hz.bjfxy.top/gtbssmmevl.html

[U21] Py：自定义上下文管理器
来源：http://hz.meibo888.top/gtlutcfyhk.html

@contextlib.contextmanager
来源：http://hz.xinyue.icu/gtmcxxuofl.html

[U22] Py：矩阵转置
来源：http://hz.jianghu66.top/gtyucwroxx.html

list(zip(*m))
来源：http://hz.shanyushiyangkeji.top/gtkqxsatpl.html

[U23] Py：分块读取大文件
来源：http://hz.zdqjudy.top/gtzfyfkddz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yuanzhike.top/gtxodyildt.html

[U24] Py：路径操作
来源：http://hz.sweek.top/gtveceemxu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gtfnajlsey.html

[U25] Py：CSV 按字典读
来源：http://hz.xuetiantiany.cn/gtaauilgew.html

csv.DictReader(f)
来源：http://hz.nanxuanxn.top/gtixxcrvdj.html

[U26] Py：并发下载
来源：http://hz.yangfankeji.com/gtdbotdvdi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.vqdsnc.cn/gtlztycbpu.html

[U27] Py：异步 HTTP
来源：http://hz.cheryme.top/gtokdwlbqw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.bjfxy.top/gtvwegqxjg.html

[U28] Py：类型别名
来源：http://hz.tianlin.xyz/gthxjivzbx.html

UserId = int
来源：http://hz.yongpay.top/gtpppbadrc.html

[U29] Py：属性校验
来源：http://hz.haohaochexian.top/gtbbabbjbo.html

@property 与 @x.setter 配合
来源：http://hz.gaohongyu789.top/gtojjvazhj.html

[U30] Py：数据类
来源：http://hz.yvedp.cn/gtvlbqdtmn.html

@dataclass(slots=True)
来源：http://hz.tian-w.cn/gtncqfysws.html

[U31] Py：单测
来源：http://hz.cheryme.top/gtpyezugoc.html

python -m pytest -q
来源：http://hz.wangdashe.top/gteefwflmw.html

[U32] Py：代码格式化
来源：http://hz.ppjwa.cn/gtrrylfmry.html

ruff format . && ruff check --fix .
来源：http://hz.havefunace.top/gtqiopsdrp.html

[U33] Py：打包发布
来源：http://hz.yueranfly.top/gtpmmtcalt.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.vqdsnc.cn/gtlwedoyoh.html

[U34] Py：判断编码
来源：http://hz.ppjwa.cn/gtohsbmwky.html

chardet.detect(raw)
来源：http://hz.chenlongwang.top/gtlnmwbamo.html

[U35] Py：发送邮件
来源：http://hz.xziqi.cn/gtqajiyazi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jinyuanbaomall.cn/gtnjqlboxl.html

[U36] Py：定时任务
来源：http://hz.tianlin.xyz/gtqfpzdxmt.html

schedule.every(10).minutes.do(job)
来源：http://hz.ppjwa.cn/gtyzvztcvw.html

[U37] Py：读写 Excel
来源：http://hz.jiagoushi.top/gtnrnuhcar.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.tianlin.xyz/gtfivhdhsf.html

[U38] Py：获取脚本所在目录
来源：http://hz.mhx1999.top/gtqjzmbmgf.html

Path(__file__).resolve().parent
来源：http://hz.shangyingyoupin.top/gttvyrihjr.html

[U39] Py：判断是否在交互环境
来源：http://hz.chenzaomai.com/gtgksldrgt.html

sys.stdout.isatty()
来源：http://hz.tianlin.xyz/gtfrvoxvqp.html

[U40] Py：打印到标准错误
来源：http://hz.shanyushiyangtech.top/gtymsvgilh.html

print("err", file=sys.stderr)
来源：http://hz.chenzaomai.com/gtqftxouer.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sysykeji.top/gtsjfysiin.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hfpthk.cn/gtexymvdem.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.tianlin.xyz/gtcogihtjk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jianghu66.top/gttlzhzguy.html

[U43] PHP：声明命名空间
来源：http://hz.jqgufenzy.top/gtmojxhpgw.html

namespace App\Http;
来源：http://hz.zhongyouzk.top/gtfemsuvxz.html

[U44] PHP：开启严格类型
来源：http://hz.0kj1m.cn/gtzqydtgqj.html

declare(strict_types=1);
来源：http://hz.gogol.net.cn/gtghkkemnd.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shzxlz.cn/gtnwnwcaio.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtpjfbsokp.html

[U46] PHP：可空类型
来源：http://hz.nwbrower.top/gtrsbjnkoy.html

?string $name = null
来源：http://hz.gzhubu.top/gtjkyfjrvd.html

[U47] PHP：联合类型
来源：http://hz.jinghuilouyu.cn/gtryotrlxn.html

int|string $id
来源：http://hz.andypj.xyz/gtqaegmboa.html

[U48] PHP：纯枚举
来源：http://hz.hnxiangtu.top/gtsdjfmzfv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.andypj.xyz/gtmlazlfqv.html

[U49] PHP：只读属性
来源：http://hz.ydjk.org.cn/gtvlevrmug.html

public readonly string $name
来源：http://hz.yanxiufei.cn/gtzzobuadh.html

[U50] PHP：构造器属性提升
来源：http://hz.jyoumei.cn/gtxrjxuqhi.html

public function __construct(private int $id) {}
来源：http://hz.yj20258888.top/gtzwhbnfov.html

[U51] PHP：数组解构
来源：http://hz.yj202588.top/gtolgcztdu.html

[$a, $b] = $arr;
来源：http://hz.zdqjudy.top/gtimncddme.html

[U52] PHP：箭头函数
来源：http://hz.chenzaomai.com/gtjzacyybn.html

$double = fn($x) => $x * 2;
来源：http://hz.dashuyun.cn/gtunnwrepw.html


<!-- 参考信息 -->