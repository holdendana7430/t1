代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yvedp.cn/gtksgwppzl.html

[S23] C：随机数
来源：http://hz.pengpengdd.cyou/gtgmsgtyos.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhixingplan.top/gtzvyykyln.html

[S24] C：获取本地时间
来源：http://hz.zhaomingkeji.xyz/gtxoondpjk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ehwqpu.com/gtqntqhvqk.html

[S25] C：内存拷贝
来源：http://hz.ydjk.org.cn/gtswiykomh.html

memcpy(dst, src, n);
来源：http://hz.bjfxy.top/gtfaxmgoit.html

[S26] C：内存清零
来源：http://hz.jqgfzy.top/gtreecjhnf.html

memset(a, 0, sizeof a);
来源：http://hz.chenlongwang.top/gtpihnumtp.html

[S27] C：定义常量
来源：http://hz.jiagoushi.top/gtawlwwidp.html

const double PI = 3.14159;
来源：http://hz.fengsongda.top/gtllgxikjv.html

[S28] C：静态变量
来源：http://hz.yuxming.cn/gtuczmxznv.html

static int counter = 0;
来源：http://hz.ybcxt.top/gtjjxygjrb.html

[S29] C：变参函数
来源：http://hz.wangdashe.top/gtxvonnbhi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydzc1.top/gtqjyzqtzd.html

[S30] C：头文件保护
来源：http://hz.yueranfly.top/gtbwzzhzdm.html

#ifndef X_H
来源：http://hz.fzhhl.top/gtgaoajhes.html

#define X_H
来源：http://hz.haohaochexian.top/gtqghkpdpn.html

#endif
来源：http://hz.c1oappe.top/gtkckzakzj.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gttqtzsmmy.html

#include <iostream>
来源：http://hz.nanxuanxn.top/gtindrdzws.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ywan-chungtsiang.top/gtzfixqllf.html

[S32] C++：字符串
来源：http://hz.9152youxi.cn/gtsbkuavxc.html

std::string s = "hi";  s += "!";
来源：http://hz.jyoumei.cn/gtlqffsofe.html

[S33] C++：vector 增删
来源：http://hz.jlsjyb.cn/gtjdvyrzxp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxinkj.top/gtbglzmolb.html

[S34] C++：遍历 vector
来源：http://hz.kuanghao11.cn/gtqfpxegml.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yongpay.top/gtkcqkwzpa.html

[S35] C++：map
来源：http://hz.pengpengdd.cyou/gtfxxjxjcp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.iojbl.cn/gtpzhcxmkq.html

[S36] C++：unordered_map
来源：http://hz.vqdsnc.cn/gtshglskic.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgfzy.top/gtzztddsct.html

[S37] C++：set
来源：http://hz.jinyuanbaomall.cn/gtndmdmilb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuanzhike.top/gtowtijxhs.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtxxavmhwp.html

std::sort(v.begin(), v.end());
来源：http://hz.dianchejie.cn/gtyadixmhv.html

[S39] C++：自定义比较器排序
来源：http://hz.0kj1m.cn/gtpqfeukyh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sysykeji.top/gttbvbtvnl.html

[S40] C++：查找元素
来源：http://hz.zhoulong.xyz/gtvojglktr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ywan-chungtsiang.top/gtidjdpvhj.html

[S41] C++：类与构造函数
来源：http://hz.nanxuanxn.top/gtvfdvbuhi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnxiangtu.top/gtqqraccdk.html

[S42] C++：继承与虚函数
来源：http://hz.svipenyu.cn/gtgedzdqnw.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhixingplan.top/gtbrzolcal.html

[S43] C++：智能指针
来源：http://hz.hysaishi.cn/gtcudvfsnb.html

auto p = std::make_unique<int>(5);
来源：http://hz.jianghu66.top/gtctucupai.html

[S44] C++：引用传参
来源：http://hz.ppjwa.cn/gtkijffvrh.html

void inc(int &x) { ++x; }
来源：http://hz.aizwys.cn/gtikinvnry.html

[S45] C++：lambda
来源：http://hz.cucudq.cn/gtkplxqsec.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenzaomai.com/gtmffkufil.html

[S46] C++：函数模板
来源：http://hz.shzxlz.cn/gtmheohhbb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aizwys.cn/gtaxqxahio.html

[S47] C++：结构化绑定遍历
来源：http://hz.vqdsnc.cn/gtmodyspfw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gaohongyu789.top/gtobbmaqrs.html

[S48] C++：逐行读文件
来源：http://hz.fengsongda.top/gtemjzfdrh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.fzhhl.top/gtioiewpyw.html

while (std::getline(in, line)) { }
来源：http://hz.meibo888.top/gtsjjoedan.html

[S49] C++：写文件
来源：http://hz.jinqigufen.top/gttdudhyfr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daria6918.cn/gtcfzfqoso.html

[S50] C++：格式化数字
来源：http://hz.yj20258888.top/gtsnkiwgrg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinghuilouyu.cn/gtzsswbnkn.html

[S51] C++：显式类型转换
来源：http://hz.gotoacloud.top/gtsnhpubiy.html

static_cast<double>(a) / b
来源：http://hz.guannengcc.top/gtjzzciigb.html

[S52] C++：const 与 noexcept
来源：http://hz.meibo888.top/gtwoifveuf.html

int size() const noexcept { return n_; }
来源：http://hz.xziqi.cn/gtjpluannk.html

[S53] C++：移动语义
来源：http://hz.shanyushiyangtech.top/gtexqbctzc.html

std::vector<int> w = std::move(v);
来源：http://hz.snrcjt.cn/gthphcsomu.html

[S54] C++：异常处理
来源：http://hz.sufxvd.cn/gtwkohemjr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ywan-chungtsiang.top/gtcbqgbhhg.html

[S55] C++：结构化绑定
来源：http://hz.zhengqikj.top/gtbvkyqycl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenjidiqi.icu/gtcfafugog.html

[S56] C++：optional
来源：http://hz.zycfv.cn/gtyonenlie.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.quarkkingdee.top/gtroghsgur.html

[S57] C++：编译期常量
来源：http://hz.xziqi.cn/gtpnabncat.html

constexpr int N = 10;
来源：http://hz.chenjidiqi.icu/gtaghzmjeo.html

[S58] C++：命名空间
来源：http://hz.dianchejie.cn/gtberbgbrv.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangdashe.top/gtjqfslnvm.html

[S59] C++：静态断言
来源：http://hz.xuanzx.com/gthmvgvspf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinghuilouyu.cn/gtwhrdyrnv.html

[S60] C++：遍历并删除元素
来源：http://hz.shzxlz.cn/gtuuajxiwl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuanzhike.top/gtkkuggsao.html

================================================================================
来源：http://hz.ydzc1.top/gtgoylemsc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhoulong.xyz/gtcqesfitl.html

================================================================================
来源：http://hz.9152youxi.cn/gtugkyegnt.html

[T01] Kotlin：Hello World
来源：http://hz.nanxuanxn.top/gthwrphwwq.html

println("Hello")
来源：http://hz.0kj1m.cn/gtchjmqavs.html

[T02] Kotlin：变量
来源：http://hz.zhongyouzk.top/gthrqrgljh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cucudq.cn/gtjzcuqrfl.html

[T03] Kotlin：字符串模板
来源：http://hz.yonumen.top/gtudxaghic.html

"值: $b"
来源：http://hz.gzhubu.top/gtsswhexge.html

[T04] Kotlin：空安全
来源：http://hz.dianchejie.cn/gtetwvrcxe.html

val n: String? = null;  n?.length
来源：http://hz.guowangkeji.top/gtbnltginq.html

[T05] Kotlin：when 表达式
来源：http://hz.iojbl.cn/gtafryzkhh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jianghu66.top/gtuubgvpor.html

[T06] Kotlin：集合映射
来源：http://hz.sysykeji.top/gttqohlywu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tanke756.top/gtdgczmama.html

[T07] Kotlin：集合过滤
来源：http://hz.yvedp.cn/gtgolqdyuz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xziqi.cn/gtddylbgfk.html

[T08] Kotlin：数据类
来源：http://hz.shuidangran.top/gtbcbkvhzw.html

data class User(val name: String, val age: Int)
来源：http://hz.sxryk.cn/gtpkdeswlb.html

[T09] Kotlin：扩展函数
来源：http://hz.316326.xyz/gttqgqspwj.html

fun String.exclaim() = this + "!"
来源：http://hz.yongpay.top/gtmzbcuugv.html

[T10] Kotlin：默认参数
来源：http://hz.sufxvd.cn/gtqaseskas.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zycfv.cn/gtivjcsdxh.html

[T11] Kotlin：协程
来源：http://hz.jlsjyb.cn/gtbhijhrtm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ppjwa.cn/gtjtcrxvuk.html

[T12] Kotlin：解构声明
来源：http://hz.yongpay.top/gtndpfjtyx.html

val (a, b) = Pair(1, 2)
来源：http://hz.pycfn.com/gtmpjgitcy.html

[T13] Kotlin：只读 Map
来源：http://hz.yongpay.top/gtnffivvjs.html

val m = mapOf("a" to 1)
来源：http://hz.cdnleiting.top/gtcuzucnon.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtapghdwgq.html

for (i in 1..10) println(i)
来源：http://hz.jyoumei.cn/gtdtjnssow.html

[T15] Kotlin：接口
来源：http://hz.zdqjudy.top/gtqqqtkihz.html

interface Shape { fun area(): Double }
来源：http://hz.jqgufenzy.top/gtyayxazno.html

[T16] Swift：Hello World
来源：http://hz.birdmap.top/gtpgeoougn.html

print("Hello")
来源：http://hz.zdqjudy.top/gtdoxwmzqj.html

[T17] Swift：变量与常量
来源：http://hz.cqqwz.cn/gtfeuolcey.html

var a = 1;  let b = 2
来源：http://hz.hnqzz.top/gtlwskqqws.html

[T18] Swift：字符串插值
来源：http://hz.xuetiantiany.cn/gtmgxgtjoi.html

"值: \(b)"
来源：http://hz.tianlin.xyz/gtxzgxxjlh.html

[T19] Swift：可选绑定
来源：http://hz.shanyushiyangkeji.top/gteldhibqm.html

if let n = opt { print(n) }
来源：http://hz.shuidangran.top/gttklevxfk.html

[T20] Swift：数组操作
来源：http://hz.yonumen.top/gtfvheyvtq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenjidiqi.icu/gtqqrwarwh.html

[T21] Swift：遍历
来源：http://hz.quarkkingdee.top/gthqwbkgod.html

for x in a { print(x) }
来源：http://hz.mhx1999.top/gtcumaibue.html

[T22] Swift：字典
来源：http://hz.hnqzz.top/gtvcomitbn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.pengpengdd.cyou/gtltncxhvt.html

[T23] Swift：函数
来源：http://hz.svipenyu.cn/gtptkcxjrk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.haohaochexian.top/gtvcwzsbso.html

[T24] Swift：闭包
来源：http://hz.shangyingyoupin.top/gtqbvorxgq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.fengsongda.top/gtrqhqvxef.html

[T25] Swift：结构体
来源：http://hz.svipenyu.cn/gtizxlcbeh.html

struct P { var x: Int }
来源：http://hz.xuanzx.com/gtfcyfvbab.html

[T26] Swift：类与重写
来源：http://hz.vqdsnc.cn/gtrqzjzsoz.html

class A: Base { override func f() {} }
来源：http://hz.tian-w.cn/gtmpmjrlvn.html

[T27] Swift：错误处理
来源：http://hz.kuanghao11.cn/gttkczznmg.html

do { try f() } catch { print(error) }
来源：http://hz.feifeiyinyue.top/gtcbtvgdzz.html

[T28] Swift：枚举
来源：http://hz.haohaochexian.top/gtocntamzq.html

enum Color { case red, green }
来源：http://hz.nanxinkj.top/gtnpolynij.html

[T29] Swift：guard 提前返回
来源：http://hz.quarkkingdee.top/gtigzpodvt.html

guard let x = opt else { return }
来源：http://hz.jinghuilouyu.cn/gtbjifwmzh.html

[T30] Swift：协议
来源：http://hz.xuetiantiany.cn/gtwebwefuj.html

protocol Shape { func area() -> Double }
来源：http://hz.hongshengwenyu.top/gtbdpcyggq.html

[T31] Lua：Hello World
来源：http://hz.zhiwuduotai.top/gtyfjuvmes.html

print("Hello")
来源：http://hz.jqgufenzy.top/gtqwhwnmom.html

[T32] Lua：局部变量
来源：http://hz.chenjidiqi.icu/gticrgpvgu.html

local a = 1
来源：http://hz.yangfankeji.com/gtnolsdanc.html

[T33] Lua：表（数组）
来源：http://hz.dianchejie.cn/gtxjgjxltx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.tian-w.cn/gttadbitzy.html

[T34] Lua：遍历表
来源：http://hz.9152youxi.cn/gtkgcgbsdd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jinghuilouyu.cn/gtocmiaztj.html

[T35] Lua：字典表
来源：http://hz.dianchejie.cn/gtdammezdp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ppjwa.cn/gtgkeqoiue.html

[T36] Lua：函数
来源：http://hz.jinyuanbaomall.cn/gtvmwltwkc.html

function add(a, b) return a + b end
来源：http://hz.daxiang520.top/gtyhnrnqji.html

[T37] Lua：字符串拼接
来源：http://hz.jlsjyb.cn/gtmhtwklvk.html

"a" .. "b"
来源：http://hz.birdmap.top/gtvrqdgdyc.html

[T38] Lua：条件
来源：http://hz.iojbl.cn/gtwgwrbkmu.html

if x > 0 then print("正") end
来源：http://hz.aizwys.cn/gtdtzlqifm.html

[T39] Lua：模式匹配
来源：http://hz.hammf.cn/gtucttjdvo.html

string.find(s, "%d+")
来源：http://hz.nwbrower.top/gtqylfjwqv.html

[T40] Lua：元表
来源：http://hz.dashuyun.cn/gtkhgvshtc.html

setmetatable({}, { __index = base })
来源：http://hz.cashguo.top/gtympmrpqb.html

[T41] Perl：Hello World
来源：http://hz.quarkkingdee.top/gtdmislaeu.html

print "Hello\n";
来源：http://hz.xuetiantiany.cn/gtcnonpiej.html

[T42] Perl：变量类型
来源：http://hz.jinqigufen.top/gtkejimwop.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.9152youxi.cn/gtdhgngxez.html

[T43] Perl：字符串插值
来源：http://hz.ehwqpu.com/gtdhzrpdav.html

"值: $a"
来源：http://hz.shzxlz.cn/gtdijaxkgj.html

[T44] Perl：条件
来源：http://hz.dashuyun.cn/gtjomeslqp.html

if ($a > 0) { print "正"; }
来源：http://hz.zhijiandao.cn/gtzrdmapvc.html

[T45] Perl：数组遍历
来源：http://hz.nanxinkj.top/gtamoiwbpj.html

for my $x (@arr) { print $x; }
来源：http://hz.feifeiyinyue.top/gtuozkbfnz.html

[T46] Perl：哈希操作
来源：http://hz.yj20258888.top/gtpfgocghy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hnqzz.top/gtmeluwriu.html

[T47] Perl：正则捕获
来源：http://hz.hnxiangtu.top/gtphkuiqii.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.guannengcc.top/gtpdqntvgw.html

[T48] Perl：正则替换
来源：http://hz.chenlongwang.top/gtwveogzha.html

$s =~ s/old/new/g;
来源：http://hz.ybcxt.top/gtbiizprdh.html

[T49] Perl：函数
来源：http://hz.316326.xyz/gtodbpdbjg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhengqikj.top/gtdyasxccg.html

[T50] Perl：逐行读文件
来源：http://hz.xziqi.cn/gtokiahqtz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.hongshengwenyu.top/gtezttdyvm.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.quarkkingdee.top/gtygiaoocj.html

[T51] Scala：Hello World
来源：http://hz.smart0.xyz/gthtfhpbpt.html

println("Hello")
来源：http://hz.yvedp.cn/gtzkvaoqix.html

[T52] Scala：变量
来源：http://hz.nanxuanxn.top/gtdfcopdov.html

val a = 1;  var b = 2
来源：http://hz.0kj1m.cn/gtvgdkkfnz.html

[T53] Scala：字符串插值
来源：http://hz.jianghu66.top/gtcbnnuhpo.html

s"值: $b"
来源：http://hz.zhixingplan.top/gtqzchozwl.html

[T54] Scala：集合映射
来源：http://hz.pycfn.com/gtthucplmf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yueranfly.top/gthcyacthc.html

[T55] Scala：集合过滤
来源：http://hz.yj20258888.top/gtbikyiwvw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.fzhhl.top/gtgdcuibyk.html

[T56] Scala：样例类
来源：http://hz.sysykeji.top/gtindgtkci.html

case class User(name: String, age: Int)
来源：http://hz.aibaodan.cn/gtgykqpaxc.html

[T57] Scala：模式匹配
来源：http://hz.bjfxy.top/gteqwcttyl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.snrcjt.cn/gtmknfxfrk.html

[T58] Scala：函数定义
来源：http://hz.jqgfzy.top/gtqxwtiroq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shangyingyoupin.top/gtwsyxxmfa.html

[T59] Scala：循环
来源：http://hz.guowangkeji.top/gtbloumchy.html

for (i <- 1 to 10) println(i)
来源：http://hz.ybcxt.top/gtgwxujqoh.html

[T60] Scala：折叠
来源：http://hz.shuidangran.top/gtktvzqmmx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.shzxlz.cn/gtgzpbnatx.html

================================================================================
来源：http://hz.dashuyun.cn/gtqrefhvcm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yongpay.top/gtnawhjwcj.html

================================================================================
来源：http://hz.tianlin.xyz/gtnhgntsmi.html

[U01] Py：创建虚拟环境
来源：http://hz.birdmap.top/gtntyinrjz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.cqqwz.cn/gttiizczkd.html

[U02] Py：导出 / 安装依赖
来源：http://hz.52xcode.cn/gtcxirbujc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.pengpengdd.cyou/gthyutwwga.html

[U03] Py：加载 .env 配置
来源：http://hz.gotoacloud.top/gtfisaszkg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.bjfxy.top/gtrdulucfb.html

[U04] Py：变量调试打印
来源：http://hz.ppjwa.cn/gtjsefliir.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.bjfxy.top/gtmsnhaiiv.html

[U05] Py：列表去重且保序
来源：http://hz.jinyuanbaomall.cn/gtumkqdjse.html

list(dict.fromkeys(arr))
来源：http://hz.zycfv.cn/gttdwlzolf.html

[U06] Py：合并两个字典
来源：http://hz.ywan-chungtsiang.top/gtcqljbktx.html

{**a, **b}
来源：http://hz.9152youxi.cn/gtbmwhwdke.html

[U07] Py：反转字典键值
来源：http://hz.hnqzz.top/gtmefrvavn.html

{v: k for k, v in d.items()}
来源：http://hz.tianlin.xyz/gtkpmtxdcb.html

[U08] Py：展平二维列表
来源：http://hz.yanxiufei.cn/gtjlbswfgi.html

[y for x in nested for y in x]
来源：http://hz.yuxming.cn/gtvcflloui.html

[U09] Py：字典取最大值的键
来源：http://hz.xuanzx.com/gtianlxoux.html

max(d, key=d.get)
来源：http://hz.yuanzhike.top/gtqrgxpicd.html

[U10] Py：按值排序字典
来源：http://hz.aibaodan.cn/gttncsmiow.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinqigufen.top/gtviidrwoe.html

[U11] Py：生成器表达式
来源：http://hz.52xcode.cn/gtmdltwanm.html

(x * 2 for x in arr)
来源：http://hz.c1oappe.top/gtfaaxdusx.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.sweek.top/gtiavqequt.html

Counter(arr).most_common(3)
来源：http://hz.jinqigufen.top/gttnfelqxt.html

[U13] Py：固定长度队列
来源：http://hz.cheryme.top/gtuwofzytx.html

deque(maxlen=10)
来源：http://hz.sweek.top/gthhswjwgu.html

[U14] Py：分组收集到列表
来源：http://hz.hfpthk.cn/gtmfskfwol.html

defaultdict(list)
来源：http://hz.9152youxi.cn/gtbvesprql.html

[U15] Py：高精度计时
来源：http://hz.cashguo.top/gtknfgpxcq.html

t = time.perf_counter()
来源：http://hz.316326.xyz/gtwcivmjek.html

[U16] Py：命令行参数解析
来源：http://hz.pengpengdd.cyou/gtqsymyiqw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.mhx1999.top/gtmqzgirvk.html

[U17] Py：初始化日志
来源：http://hz.hysaishi.cn/gtimkxdmxx.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.sxryk.cn/gtdkezpnia.html

[U18] Py：预编译正则
来源：http://hz.chenzaomai.com/gtwpdgugym.html

pat = re.compile(r"\d+")
来源：http://hz.xuanzx.com/gtkqnxktxd.html

[U19] Py：正则替换带回调
来源：http://hz.hammf.cn/gtihyooldb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.quarkkingdee.top/gtglkfebkd.html

[U20] Py：缓存函数结果
来源：http://hz.ydzc1.top/gtwadibxgs.html

@functools.lru_cache(maxsize=None)
来源：http://hz.daria6918.cn/gttqmpjppt.html

[U21] Py：自定义上下文管理器
来源：http://hz.sysykeji.top/gtzjfcbneh.html

@contextlib.contextmanager
来源：http://hz.sysykeji.top/gtdurshwjk.html

[U22] Py：矩阵转置
来源：http://hz.zhixingplan.top/gtdozphsju.html

list(zip(*m))
来源：http://hz.xuetiantiany.cn/gtzfdprvdq.html

[U23] Py：分块读取大文件
来源：http://hz.aibaodan.cn/gtetrnosrs.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhaomingkeji.xyz/gtxichodvu.html

[U24] Py：路径操作
来源：http://hz.shanyushiyangtech.top/gtwbbfdxdn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.chenzaomai.com/gtinkpxebi.html

[U25] Py：CSV 按字典读
来源：http://hz.sysykeji.top/gtnbucomjl.html

csv.DictReader(f)
来源：http://hz.svipenyu.cn/gtglaotyaq.html

[U26] Py：并发下载
来源：http://hz.cashguo.top/gtpxdnmsqx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gzhubu.top/gtuheujgks.html

[U27] Py：异步 HTTP
来源：http://hz.chenlongwang.top/gttqurvyqd.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shanyushiyangkeji.top/gtgkowwnms.html

[U28] Py：类型别名
来源：http://hz.ehwqpu.com/gtbvxfnbqz.html

UserId = int
来源：http://hz.birdmap.top/gtnahluzeb.html

[U29] Py：属性校验
来源：http://hz.nwbrower.top/gtwqpcoyvb.html

@property 与 @x.setter 配合
来源：http://hz.nanxuanxn.top/gtutyyjsfu.html

[U30] Py：数据类
来源：http://hz.aibaodan.cn/gtxpkcegbx.html

@dataclass(slots=True)
来源：http://hz.tian-w.cn/gtarvosfsu.html

[U31] Py：单测
来源：http://hz.316326.xyz/gtgjszfbkp.html

python -m pytest -q
来源：http://hz.vqdsnc.cn/gtbeidasoc.html

[U32] Py：代码格式化
来源：http://hz.jlsjyb.cn/gtxjxmblol.html

ruff format . && ruff check --fix .
来源：http://hz.zhengqikj.top/gtrddvcmlb.html

[U33] Py：打包发布
来源：http://hz.nanxinkj.top/gtnivbyoxe.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jinqigufen.top/gthayweinz.html

[U34] Py：判断编码
来源：http://hz.aizwys.cn/gtzwnizylo.html

chardet.detect(raw)
来源：http://hz.zhoulong.xyz/gtpxuodfzf.html

[U35] Py：发送邮件
来源：http://hz.tian-w.cn/gtgpwcptvd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.haohaochexian.top/gtwykmfeyt.html

[U36] Py：定时任务
来源：http://hz.yangfankeji.com/gthjfnpllc.html

schedule.every(10).minutes.do(job)
来源：http://hz.jinghuilouyu.cn/gtzmuucnjp.html

[U37] Py：读写 Excel
来源：http://hz.c1oappe.top/gtdnoslztq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cqqwz.cn/gtvlfopatz.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhaomingkeji.xyz/gteykavrap.html

Path(__file__).resolve().parent
来源：http://hz.hnqzz.top/gtxfjluleg.html

[U39] Py：判断是否在交互环境
来源：http://hz.bjfxy.top/gtemhhpqpb.html

sys.stdout.isatty()
来源：http://hz.yongpay.top/gtcjapndys.html

[U40] Py：打印到标准错误
来源：http://hz.zhongyouzk.top/gtgdkxdmkt.html

print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtssgovqne.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhongyouzk.top/gtfsztljmj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jiagoushi.top/gtgjflhird.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ppjwa.cn/gtbyksenit.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ehwqpu.com/gtzyunljde.html

[U43] PHP：声明命名空间
来源：http://hz.tanke756.top/gthsrqmeyz.html

namespace App\Http;
来源：http://hz.jinyuanbaomall.cn/gtetgmajde.html

[U44] PHP：开启严格类型
来源：http://hz.xinyue.icu/gtlcqdnwgz.html

declare(strict_types=1);
来源：http://hz.jinqigufen.top/gtkpjhquiq.html

[U45] PHP：类型声明与返回类型
来源：http://hz.quarkkingdee.top/gtwhwfltlf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtansugofm.html

[U46] PHP：可空类型
来源：http://hz.cashguo.top/gtxsgebvko.html

?string $name = null
来源：http://hz.hnxiangtu.top/gtfxprkeps.html


<!-- 参考信息 -->