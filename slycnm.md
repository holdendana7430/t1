代发 wailian999

static int counter = 0;
来源：http://hz.xinyue.icu/gtzugwkcmf.html

[S29] C：变参函数
来源：http://hz.jyoumei.cn/gttaipaqkq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.vqdsnc.cn/gtyyjkgobm.html

[S30] C：头文件保护
来源：http://hz.jiagoushi.top/gtcfeimuol.html

#ifndef X_H
来源：http://hz.chenjidiqi.icu/gttoomsvdz.html

#define X_H
来源：http://hz.vqdsnc.cn/gtyxxsncmu.html

#endif
来源：http://hz.cdnleiting.top/gtmllvlogj.html

[S31] C++：Hello World
来源：http://hz.hysaishi.cn/gtemsvpwih.html

#include <iostream>
来源：http://hz.jinqigfzy.top/gtfyjfvken.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigfzy.top/gtvbjdwxxg.html

[S32] C++：字符串
来源：http://hz.shzxlz.cn/gtlnwchavo.html

std::string s = "hi";  s += "!";
来源：http://hz.iojbl.cn/gtfrlzllfv.html

[S33] C++：vector 增删
来源：http://hz.cqqwz.cn/gtngysekkq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yongpay.top/gtvgaxzllf.html

[S34] C++：遍历 vector
来源：http://hz.zdqjudy.top/gtvjfratxz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xingfuxueyuan.xyz/gtwgjnshyx.html

[S35] C++：map
来源：http://hz.daria6918.cn/gtvouynwli.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cqqwz.cn/gtjppywzbh.html

[S36] C++：unordered_map
来源：http://hz.gogol.net.cn/gtrecsvoub.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yueranfly.top/gtkaujvmrm.html

[S37] C++：set
来源：http://hz.mhx1999.top/gtpbakcliq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jqgfzy.top/gtsknlddlv.html

[S38] C++：排序
来源：http://hz.hfpthk.cn/gtelznitpa.html

std::sort(v.begin(), v.end());
来源：http://hz.sweek.top/gtpxuiutfd.html

[S39] C++：自定义比较器排序
来源：http://hz.redwolf501.top/gtvarntnjl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenzaomai.com/gtgcfqyxjx.html

[S40] C++：查找元素
来源：http://hz.zycfv.cn/gtejysndyb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.iojbl.cn/gtvsnbmxyc.html

[S41] C++：类与构造函数
来源：http://hz.yvedp.cn/gtofvjslbh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.vqdsnc.cn/gtjgvqmljx.html

[S42] C++：继承与虚函数
来源：http://hz.zhengqikj.top/gtrzanfhed.html

class B : public Base { public: void f() override {} };
来源：http://hz.mhx1999.top/gtgmubkpzv.html

[S43] C++：智能指针
来源：http://hz.hnqzz.top/gtnzmdbldg.html

auto p = std::make_unique<int>(5);
来源：http://hz.xuanzx.com/gtellndztf.html

[S44] C++：引用传参
来源：http://hz.smart0.xyz/gtgcmhrhpa.html

void inc(int &x) { ++x; }
来源：http://hz.fzhhl.top/gtsosmdsip.html

[S45] C++：lambda
来源：http://hz.cucudq.cn/gtnnhgleoa.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.0kj1m.cn/gtddebsnwf.html

[S46] C++：函数模板
来源：http://hz.yongpay.top/gthstlrvum.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cheryme.top/gteeiwroos.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhijiandao.cn/gtfbenjmgj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.quarkkingdee.top/gtmvsemhos.html

[S48] C++：逐行读文件
来源：http://hz.tanke756.top/gtmalhgwfw.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jiagoushi.top/gtalgngqln.html

while (std::getline(in, line)) { }
来源：http://hz.dashuyun.cn/gtvbfbujgc.html

[S49] C++：写文件
来源：http://hz.guowangkeji.top/gtxpzpqveb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jiagoushi.top/gttnuvfncg.html

[S50] C++：格式化数字
来源：http://hz.yanxiufei.cn/gtklowmzaw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.guowangkeji.top/gtdrftxjnv.html

[S51] C++：显式类型转换
来源：http://hz.cdnleiting.top/gttcdgcnho.html

static_cast<double>(a) / b
来源：http://hz.aibaodan.cn/gtmntibmfu.html

[S52] C++：const 与 noexcept
来源：http://hz.c1oappe.top/gtcqbhywov.html

int size() const noexcept { return n_; }
来源：http://hz.haohaochexian.top/gtcvpbhmsj.html

[S53] C++：移动语义
来源：http://hz.redwolf501.top/gtwjtvwvld.html

std::vector<int> w = std::move(v);
来源：http://hz.hammf.cn/gteeerdmin.html

[S54] C++：异常处理
来源：http://hz.cashguo.top/gtqwdkpbzy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.9152youxi.cn/gthqpjnwuy.html

[S55] C++：结构化绑定
来源：http://hz.hnxiangtu.top/gtzyjormhi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cdnleiting.top/gtzgkfteoh.html

[S56] C++：optional
来源：http://hz.jqgufenzy.top/gtfoazzqbr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jiagoushi.top/gtgejjdvth.html

[S57] C++：编译期常量
来源：http://hz.tianlin.xyz/gtwvniwnmv.html

constexpr int N = 10;
来源：http://hz.gotoacloud.top/gtlsocowaf.html

[S58] C++：命名空间
来源：http://hz.meibo888.top/gttcgpfycu.html

namespace ns { int f() { return 1; } }
来源：http://hz.gogol.net.cn/gtecbhwrju.html

[S59] C++：静态断言
来源：http://hz.ywan-chungtsiang.top/gtknkcnwkf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tian-w.cn/gthimjieep.html

[S60] C++：遍历并删除元素
来源：http://hz.yonumen.top/gthhskzxed.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.daria6918.cn/gtyzcvanqt.html

================================================================================
来源：http://hz.kuanghao11.cn/gtpxpokvar.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigufen.top/gtsjfqrdsp.html

================================================================================
来源：http://hz.zdqjudy.top/gthflqirft.html

[T01] Kotlin：Hello World
来源：http://hz.nwbrower.top/gtbwcmhsxw.html

println("Hello")
来源：http://hz.cheryme.top/gtrnhagzht.html

[T02] Kotlin：变量
来源：http://hz.chenjidiqi.icu/gtzifukhda.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cucudq.cn/gtwrregnkg.html

[T03] Kotlin：字符串模板
来源：http://hz.xuetiantiany.cn/gtthgpdxsb.html

"值: $b"
来源：http://hz.jyoumei.cn/gtribsfeaj.html

[T04] Kotlin：空安全
来源：http://hz.ywan-chungtsiang.top/gtvdrjmqqp.html

val n: String? = null;  n?.length
来源：http://hz.hongshengwenyu.top/gttfzowasc.html

[T05] Kotlin：when 表达式
来源：http://hz.zhiwuduotai.top/gtirpwfgpg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cdnleiting.top/gtldvxxrmj.html

[T06] Kotlin：集合映射
来源：http://hz.redwolf501.top/gtqxemmnuv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxuanxn.top/gtkeetijfz.html

[T07] Kotlin：集合过滤
来源：http://hz.cashguo.top/gtkulztbpx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gzhubu.top/gtqlxuivic.html

[T08] Kotlin：数据类
来源：http://hz.hysaishi.cn/gtxscjoekf.html

data class User(val name: String, val age: Int)
来源：http://hz.hnxiangtu.top/gtscbgkyrh.html

[T09] Kotlin：扩展函数
来源：http://hz.zhiwuduotai.top/gtrwdqlwgs.html

fun String.exclaim() = this + "!"
来源：http://hz.hammf.cn/gtxndewjie.html

[T10] Kotlin：默认参数
来源：http://hz.snrcjt.cn/gttweqmety.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jyoumei.cn/gtzduyczss.html

[T11] Kotlin：协程
来源：http://hz.cqqwz.cn/gtzftcensh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.snrcjt.cn/gtjzelvilz.html

[T12] Kotlin：解构声明
来源：http://hz.c1oappe.top/gtyfsvmmtw.html

val (a, b) = Pair(1, 2)
来源：http://hz.hnxiangtu.top/gtyvvwwagi.html

[T13] Kotlin：只读 Map
来源：http://hz.yanxiufei.cn/gtshyeklyq.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtjehqmbxi.html

[T14] Kotlin：循环
来源：http://hz.hnxiangtu.top/gtoeawuitq.html

for (i in 1..10) println(i)
来源：http://hz.wangshuangyany.cn/gtsygwbvgw.html

[T15] Kotlin：接口
来源：http://hz.cheryme.top/gtykrrbplg.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258888.top/gtnpnpodez.html

[T16] Swift：Hello World
来源：http://hz.wangshuangyany.cn/gthhifaksj.html

print("Hello")
来源：http://hz.ppjwa.cn/gttwgjcrmx.html

[T17] Swift：变量与常量
来源：http://hz.chenjidiqi.icu/gtpctpsngo.html

var a = 1;  let b = 2
来源：http://hz.shzxlz.cn/gtsniquemf.html

[T18] Swift：字符串插值
来源：http://hz.jinqigufen.top/gtfsyitero.html

"值: \(b)"
来源：http://hz.daria6918.cn/gtoyzldbqj.html

[T19] Swift：可选绑定
来源：http://hz.xinyue.icu/gtbqyzxjtm.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gtuafdvzwa.html

[T20] Swift：数组操作
来源：http://hz.ydzc1.top/gtgvnttuwk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shzxlz.cn/gthxerwtmd.html

[T21] Swift：遍历
来源：http://hz.ehwqpu.com/gtyiuwgiwo.html

for x in a { print(x) }
来源：http://hz.zhiwuduotai.top/gtlucnrexj.html

[T22] Swift：字典
来源：http://hz.wangdashe.top/gtelmwymoo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yongpay.top/gthgvribro.html

[T23] Swift：函数
来源：http://hz.quarkkingdee.top/gtbwaapdza.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.vqdsnc.cn/gtwcmaplgp.html

[T24] Swift：闭包
来源：http://hz.zycfv.cn/gtoitndzwa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sweek.top/gtniowvtyh.html

[T25] Swift：结构体
来源：http://hz.pengpengdd.cyou/gtuvvokysx.html

struct P { var x: Int }
来源：http://hz.fzhhl.top/gtvxdiccvc.html

[T26] Swift：类与重写
来源：http://hz.kuanghao11.cn/gtizpqdxti.html

class A: Base { override func f() {} }
来源：http://hz.jinghuilouyu.cn/gtyzdgtcqe.html

[T27] Swift：错误处理
来源：http://hz.zhiwuduotai.top/gtvilmdqbc.html

do { try f() } catch { print(error) }
来源：http://hz.cheryme.top/gtcnwlzvqp.html

[T28] Swift：枚举
来源：http://hz.smart0.xyz/gtqpfntsvl.html

enum Color { case red, green }
来源：http://hz.hysaishi.cn/gtqyoskqwh.html

[T29] Swift：guard 提前返回
来源：http://hz.tanke756.top/gtahqiudxp.html

guard let x = opt else { return }
来源：http://hz.mhx1999.top/gtsfipdmfc.html

[T30] Swift：协议
来源：http://hz.zhongyouzk.top/gtiwwnzxof.html

protocol Shape { func area() -> Double }
来源：http://hz.jinghuilouyu.cn/gtflcslvug.html

[T31] Lua：Hello World
来源：http://hz.sufxvd.cn/gthymcqhod.html

print("Hello")
来源：http://hz.chenjidiqi.icu/gtuoteffjk.html

[T32] Lua：局部变量
来源：http://hz.tanke756.top/gtozdxcigw.html

local a = 1
来源：http://hz.zhixingplan.top/gtoajcslcb.html

[T33] Lua：表（数组）
来源：http://hz.wangdashe.top/gtdgqdpxcz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cheryme.top/gttlyhtdpv.html

[T34] Lua：遍历表
来源：http://hz.xuetiantiany.cn/gtiyhmitip.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.sufxvd.cn/gtbgbxypyg.html

[T35] Lua：字典表
来源：http://hz.cqqwz.cn/gtdpiqfcbj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.meibo888.top/gtanwqhhxm.html

[T36] Lua：函数
来源：http://hz.hongshengwenyu.top/gtcxfruhfe.html

function add(a, b) return a + b end
来源：http://hz.andypj.xyz/gtgamodjul.html

[T37] Lua：字符串拼接
来源：http://hz.gaohongyu789.top/gtwkxdxcxe.html

"a" .. "b"
来源：http://hz.daxiang520.top/gtfomavjzk.html

[T38] Lua：条件
来源：http://hz.0kj1m.cn/gtcyofuetp.html

if x > 0 then print("正") end
来源：http://hz.sweek.top/gtiwqmzbud.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gtfuuhpath.html

string.find(s, "%d+")
来源：http://hz.sufxvd.cn/gtyvchkcav.html

[T40] Lua：元表
来源：http://hz.yanxiufei.cn/gthahsnrkk.html

setmetatable({}, { __index = base })
来源：http://hz.hnxiangtu.top/gtnfytfnpz.html

[T41] Perl：Hello World
来源：http://hz.tianlin.xyz/gtxxyzmwzw.html

print "Hello\n";
来源：http://hz.chenjidiqi.icu/gtwvlaipcx.html

[T42] Perl：变量类型
来源：http://hz.cqqwz.cn/gtygjzhuki.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shzxlz.cn/gtlmcqdnvz.html

[T43] Perl：字符串插值
来源：http://hz.ydzc1.top/gtiiradvpr.html

"值: $a"
来源：http://hz.zdqjudy.top/gtqcpdkqxj.html

[T44] Perl：条件
来源：http://hz.pycfn.com/gtiqdvomfp.html

if ($a > 0) { print "正"; }
来源：http://hz.shuidangran.top/gtatobqhak.html

[T45] Perl：数组遍历
来源：http://hz.shanyushiyangtech.top/gtcgsgjgqf.html

for my $x (@arr) { print $x; }
来源：http://hz.pycfn.com/gtupowqqnv.html

[T46] Perl：哈希操作
来源：http://hz.hongshengwenyu.top/gtzezyzrfr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhiwuduotai.top/gtfernntnm.html

[T47] Perl：正则捕获
来源：http://hz.tian-w.cn/gtahagtvgl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shangyingyoupin.top/gtsxfhoklu.html

[T48] Perl：正则替换
来源：http://hz.ivvv.top/gtllscdhow.html

$s =~ s/old/new/g;
来源：http://hz.chenlongwang.top/gtcxjhpjwx.html

[T49] Perl：函数
来源：http://hz.tianlin.xyz/gtrsldupsh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yanxiufei.cn/gtfkjzhtsw.html

[T50] Perl：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtfubntzvl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sweek.top/gtizaybrak.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jlsjyb.cn/gtgjdtgixv.html

[T51] Scala：Hello World
来源：http://hz.aizwys.cn/gtxenucmrj.html

println("Hello")
来源：http://hz.svipenyu.cn/gtukruczve.html

[T52] Scala：变量
来源：http://hz.jyoumei.cn/gtnfnzvweg.html

val a = 1;  var b = 2
来源：http://hz.haohaochexian.top/gtzmsbzxoc.html

[T53] Scala：字符串插值
来源：http://hz.pengpengdd.cyou/gtzltsubeh.html

s"值: $b"
来源：http://hz.chenlongwang.top/gtmfttdxih.html

[T54] Scala：集合映射
来源：http://hz.snrcjt.cn/gtqqpsclbu.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhijiandao.cn/gtyuovzagy.html

[T55] Scala：集合过滤
来源：http://hz.daria6918.cn/gtoontvjtx.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj202588.top/gtbrfdnclw.html

[T56] Scala：样例类
来源：http://hz.0kj1m.cn/gtvpvbsdyl.html

case class User(name: String, age: Int)
来源：http://hz.jqgfzy.top/gtfrouapei.html

[T57] Scala：模式匹配
来源：http://hz.xuanzx.com/gtpiyfsaim.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hongshengwenyu.top/gtsfmhigqo.html

[T58] Scala：函数定义
来源：http://hz.cucudq.cn/gturndluxs.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.gaohongyu789.top/gtfzhehnzo.html

[T59] Scala：循环
来源：http://hz.9152youxi.cn/gtzegmshgw.html

for (i <- 1 to 10) println(i)
来源：http://hz.aizwys.cn/gtujoschfq.html

[T60] Scala：折叠
来源：http://hz.fzhhl.top/gtzvuyzrra.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.zycfv.cn/gtrnbstwzq.html

================================================================================
来源：http://hz.guannengcc.top/gtxobvvmvy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.c1oappe.top/gtcffimweb.html

================================================================================
来源：http://hz.xuanzx.com/gtfpqnufza.html

[U01] Py：创建虚拟环境
来源：http://hz.mhx1999.top/gtqphdjzvv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shzxlz.cn/gtiswfdxum.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhaomingkeji.xyz/gterwwnxfi.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xylfe.cn/gtojhvihbx.html

[U03] Py：加载 .env 配置
来源：http://hz.smart0.xyz/gtonnnokbz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shanyushiyangtech.top/gtqvpycapn.html

[U04] Py：变量调试打印
来源：http://hz.cdnleiting.top/gtaczeoqyp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.dianchejie.cn/gtwkrjywqx.html

[U05] Py：列表去重且保序
来源：http://hz.cdnleiting.top/gthiesdgqy.html

list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtgdddbtvu.html

[U06] Py：合并两个字典
来源：http://hz.zhijiandao.cn/gttoqciamv.html

{**a, **b}
来源：http://hz.jyoumei.cn/gtqspqafpx.html

[U07] Py：反转字典键值
来源：http://hz.dianchejie.cn/gtsawoyhuv.html

{v: k for k, v in d.items()}
来源：http://hz.meibo888.top/gtzzulkxai.html

[U08] Py：展平二维列表
来源：http://hz.tian-w.cn/gtnhlhspai.html

[y for x in nested for y in x]
来源：http://hz.zhoulong.xyz/gtptfhicek.html

[U09] Py：字典取最大值的键
来源：http://hz.meibo888.top/gttmzrgklv.html

max(d, key=d.get)
来源：http://hz.jqgfzy.top/gtkhpvlopk.html

[U10] Py：按值排序字典
来源：http://hz.mhx1999.top/gttcqxitry.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.chenjidiqi.icu/gtfdwyasjw.html

[U11] Py：生成器表达式
来源：http://hz.jlsjyb.cn/gtdjysficp.html

(x * 2 for x in arr)
来源：http://hz.sxryk.cn/gtwntirmrd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhijiandao.cn/gttsrdiwbw.html

Counter(arr).most_common(3)
来源：http://hz.svipenyu.cn/gthkmtaqsm.html

[U13] Py：固定长度队列
来源：http://hz.316326.xyz/gtrcgkqvtt.html

deque(maxlen=10)
来源：http://hz.ydjk.org.cn/gtkaabcvgy.html

[U14] Py：分组收集到列表
来源：http://hz.xinyue.icu/gtepnjefop.html

defaultdict(list)
来源：http://hz.yj20258.top/gtxpcipovl.html

[U15] Py：高精度计时
来源：http://hz.vqdsnc.cn/gtglgwfumd.html

t = time.perf_counter()
来源：http://hz.shzxlz.cn/gtohrgwlqu.html

[U16] Py：命令行参数解析
来源：http://hz.cdnleiting.top/gtfgovffgf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hammf.cn/gtsogosmwq.html

[U17] Py：初始化日志
来源：http://hz.haohaochexian.top/gtdwbtjloc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yj20258888.top/gtlhaxiztg.html

[U18] Py：预编译正则
来源：http://hz.meibo888.top/gtoletyptz.html

pat = re.compile(r"\d+")
来源：http://hz.daxiang520.top/gtdmhkurmw.html

[U19] Py：正则替换带回调
来源：http://hz.tanke756.top/gtlrgrdthn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.sufxvd.cn/gtduyyrtyf.html

[U20] Py：缓存函数结果
来源：http://hz.redwolf501.top/gtzqzsywux.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhaomingkeji.xyz/gtjyyjrjii.html

[U21] Py：自定义上下文管理器
来源：http://hz.cheryme.top/gtqjihpsvd.html

@contextlib.contextmanager
来源：http://hz.shzxlz.cn/gtzriazrwc.html

[U22] Py：矩阵转置
来源：http://hz.zhongyouzk.top/gtvhzenmtm.html

list(zip(*m))
来源：http://hz.haohaochexian.top/gtyjdnpjco.html

[U23] Py：分块读取大文件
来源：http://hz.xinyue.icu/gtogflvbxs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yanxiufei.cn/gtrswezvlu.html

[U24] Py：路径操作
来源：http://hz.xylfe.cn/gtayspjacl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.ehwqpu.com/gtajuyfvpj.html

[U25] Py：CSV 按字典读
来源：http://hz.yuxming.cn/gtfugcqsdx.html

csv.DictReader(f)
来源：http://hz.cashguo.top/gtpunjwspl.html

[U26] Py：并发下载
来源：http://hz.xingfuxueyuan.xyz/gtoxpohmvf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jqgufenzy.top/gtxfeuabvp.html

[U27] Py：异步 HTTP
来源：http://hz.mhx1999.top/gtkhsffaju.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.feifeiyinyue.top/gtftupabeg.html

[U28] Py：类型别名
来源：http://hz.ppjwa.cn/gtdglqqznu.html

UserId = int
来源：http://hz.ydjk.org.cn/gtynotgyvd.html

[U29] Py：属性校验
来源：http://hz.pengpengdd.cyou/gtdyqbwvdv.html

@property 与 @x.setter 配合
来源：http://hz.cucudq.cn/gtpdlelogs.html

[U30] Py：数据类
来源：http://hz.jyoumei.cn/gttbnungdk.html

@dataclass(slots=True)
来源：http://hz.shuidangran.top/gtgzeiltrt.html

[U31] Py：单测
来源：http://hz.gotoacloud.top/gtrhhtgyox.html

python -m pytest -q
来源：http://hz.xziqi.cn/gtezcmorxe.html

[U32] Py：代码格式化
来源：http://hz.jyoumei.cn/gtjqdjfkzo.html

ruff format . && ruff check --fix .
来源：http://hz.kuanghao11.cn/gthpkgsgyw.html

[U33] Py：打包发布
来源：http://hz.gaohongyu789.top/gtshlopyev.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.xingfuxueyuan.xyz/gtyhiuqyit.html

[U34] Py：判断编码
来源：http://hz.xinyue.icu/gtibpcuvcm.html

chardet.detect(raw)
来源：http://hz.yanxiufei.cn/gthisloouo.html

[U35] Py：发送邮件
来源：http://hz.yvedp.cn/gtmqyudkya.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jinyuanbaomall.cn/gteroafbgr.html

[U36] Py：定时任务
来源：http://hz.zhoulong.xyz/gtdclsoknq.html

schedule.every(10).minutes.do(job)
来源：http://hz.havefunace.top/gtdckwhyhd.html

[U37] Py：读写 Excel
来源：http://hz.tian-w.cn/gtcligwwdn.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.9152youxi.cn/gthvjhzupr.html

[U38] Py：获取脚本所在目录
来源：http://hz.svipenyu.cn/gtooliolwv.html

Path(__file__).resolve().parent
来源：http://hz.nwbrower.top/gtnoenpdkq.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhongyouzk.top/gtqjrqlijv.html

sys.stdout.isatty()
来源：http://hz.ydzc1.top/gtshvooyzc.html

[U40] Py：打印到标准错误
来源：http://hz.cdnleiting.top/gtemubyode.html

print("err", file=sys.stderr)
来源：http://hz.andypj.xyz/gtzhwbtzxv.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.hywenlv.cn/gtfornlfvu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shanyushiyangtech.top/gtgkmkdokh.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.vqdsnc.cn/gtfioyttip.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.mhx1999.top/gtkbolvuut.html

[U43] PHP：声明命名空间
来源：http://hz.iojbl.cn/gtsffjyaut.html

namespace App\Http;
来源：http://hz.yongpay.top/gtyshlcjsg.html

[U44] PHP：开启严格类型
来源：http://hz.haohaochexian.top/gtjsgnoref.html

declare(strict_types=1);
来源：http://hz.hongshengwenyu.top/gttfrsunbs.html

[U45] PHP：类型声明与返回类型
来源：http://hz.xuanzx.com/gthhcchqhc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fengsongda.top/gtuhcmfxag.html

[U46] PHP：可空类型
来源：http://hz.tianlin.xyz/gtpokbhcfu.html

?string $name = null
来源：http://hz.kuanghao11.cn/gtuovoijmj.html

[U47] PHP：联合类型
来源：http://hz.hywenlv.cn/gtbkdiabol.html

int|string $id
来源：http://hz.ppjwa.cn/gtecodcwkx.html

[U48] PHP：纯枚举
来源：http://hz.dianchejie.cn/gtxfielhkp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yangfankeji.com/gtwrvkvfeb.html

[U49] PHP：只读属性
来源：http://hz.gzhubu.top/gtcyjazdhk.html

public readonly string $name
来源：http://hz.yuxming.cn/gtcowysaxm.html

[U50] PHP：构造器属性提升
来源：http://hz.snrcjt.cn/gtwumekcwa.html

public function __construct(private int $id) {}
来源：http://hz.mhx1999.top/gtxkybrzec.html

[U51] PHP：数组解构
来源：http://hz.wangshuangyany.cn/gtdechicab.html

[$a, $b] = $arr;
来源：http://hz.jinqigfzy.top/gtcaxsalui.html

[U52] PHP：箭头函数
来源：http://hz.shanyushiyangkeji.top/gtudaqthrn.html

$double = fn($x) => $x * 2;
来源：http://hz.hfpthk.cn/gtptxhligf.html


<!-- 参考信息 -->