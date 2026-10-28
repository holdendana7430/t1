代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.daria6918.cn/gtinlyrqhb.html

[S21] C：字符类别判断
来源：http://hz.hnqzz.top/gttomwsmty.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.svipenyu.cn/gtbgroggji.html

[S22] C：字符串转数字
来源：http://hz.yvedp.cn/gtbaiepljr.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hnqzz.top/gtvwuryyhk.html

[S23] C：随机数
来源：http://hz.hywenlv.cn/gtjpgsfarr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jianghu66.top/gtnrwqryun.html

[S24] C：获取本地时间
来源：http://hz.xuetiantiany.cn/gtqrhlgbsu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yanxiufei.cn/gtkcomiiuf.html

[S25] C：内存拷贝
来源：http://hz.yvedp.cn/gtkaozfpvg.html

memcpy(dst, src, n);
来源：http://hz.ppjwa.cn/gtcgbamrgr.html

[S26] C：内存清零
来源：http://hz.ivvv.top/gtggtsrxvv.html

memset(a, 0, sizeof a);
来源：http://hz.jqgfzy.top/gtqpsparlp.html

[S27] C：定义常量
来源：http://hz.havefunace.top/gtxlhjjfux.html

const double PI = 3.14159;
来源：http://hz.daria6918.cn/gteycpyekx.html

[S28] C：静态变量
来源：http://hz.wangshuangyany.cn/gtgsrfcmoa.html

static int counter = 0;
来源：http://hz.zhiwuduotai.top/gthnoeyhux.html

[S29] C：变参函数
来源：http://hz.wangdashe.top/gtkotoywog.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tianlin.xyz/gtmmsyeoun.html

[S30] C：头文件保护
来源：http://hz.pycfn.com/gtxdtmbsbp.html

#ifndef X_H
来源：http://hz.nanxinkj.top/gtwmqgyxmy.html

#define X_H
来源：http://hz.ybcxt.top/gtmrcugirk.html

#endif
来源：http://hz.jyoumei.cn/gtpofbienj.html

[S31] C++：Hello World
来源：http://hz.dashuyun.cn/gtxlrhgezz.html

#include <iostream>
来源：http://hz.cheryme.top/gtjfadtjab.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigfzy.top/gtnujetrmz.html

[S32] C++：字符串
来源：http://hz.yueranfly.top/gtyhujtfxi.html

std::string s = "hi";  s += "!";
来源：http://hz.aizwys.cn/gtzkpyneps.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gtacfzffid.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangtech.top/gtyivkzuji.html

[S34] C++：遍历 vector
来源：http://hz.zhongyouzk.top/gtemxqcila.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj20258.top/gtzeqcppwe.html

[S35] C++：map
来源：http://hz.yongpay.top/gtfakckjkp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hysaishi.cn/gtizvbihzy.html

[S36] C++：unordered_map
来源：http://hz.jinqigufen.top/gtrsckfbik.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtcuprcagu.html

[S37] C++：set
来源：http://hz.dianchejie.cn/gtokjouvyu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.redwolf501.top/gtzagicubp.html

[S38] C++：排序
来源：http://hz.mhx1999.top/gtfxxiiryh.html

std::sort(v.begin(), v.end());
来源：http://hz.mhx1999.top/gtizccdegi.html

[S39] C++：自定义比较器排序
来源：http://hz.zhoulong.xyz/gtmaoyqzaz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.dianchejie.cn/gtfmobjitc.html

[S40] C++：查找元素
来源：http://hz.cdnleiting.top/gtchvyxehh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xuetiantiany.cn/gtklfeelol.html

[S41] C++：类与构造函数
来源：http://hz.jqgfzy.top/gtghowuubp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yanxiufei.cn/gticalsodm.html

[S42] C++：继承与虚函数
来源：http://hz.nwbrower.top/gtjtwnpash.html

class B : public Base { public: void f() override {} };
来源：http://hz.daxiang520.top/gtjhlanwzz.html

[S43] C++：智能指针
来源：http://hz.gaohongyu789.top/gtdbcnqpmz.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhengqikj.top/gtvcyqjker.html

[S44] C++：引用传参
来源：http://hz.ppjwa.cn/gtanzokkhb.html

void inc(int &x) { ++x; }
来源：http://hz.feifeiyinyue.top/gtwmobwiip.html

[S45] C++：lambda
来源：http://hz.aibaodan.cn/gtfpexeswm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhixingplan.top/gtumgrbhxs.html

[S46] C++：函数模板
来源：http://hz.yuanzhike.top/gtrnflhwfp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.9152youxi.cn/gtaajmpfrf.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigfzy.top/gtqcyieeib.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ywan-chungtsiang.top/gtrlefruch.html

[S48] C++：逐行读文件
来源：http://hz.mhx1999.top/gtdkpvbiqm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.52xcode.cn/gtowbpkmah.html

while (std::getline(in, line)) { }
来源：http://hz.fzhhl.top/gtyqwafdtx.html

[S49] C++：写文件
来源：http://hz.guowangkeji.top/gthwpyepdl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xylfe.cn/gtomvdpwjg.html

[S50] C++：格式化数字
来源：http://hz.sxryk.cn/gttdfvzeut.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shzxlz.cn/gtrtcxliju.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtddtqxlcb.html

static_cast<double>(a) / b
来源：http://hz.shzxlz.cn/gtcmgevgge.html

[S52] C++：const 与 noexcept
来源：http://hz.zhoulong.xyz/gtfyhuzrto.html

int size() const noexcept { return n_; }
来源：http://hz.hongshengwenyu.top/gteihylyrs.html

[S53] C++：移动语义
来源：http://hz.fengsongda.top/gtfgotrjmd.html

std::vector<int> w = std::move(v);
来源：http://hz.ppjwa.cn/gttswgggpj.html

[S54] C++：异常处理
来源：http://hz.yuanzhike.top/gtmuuusokg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nwbrower.top/gtpucmjfql.html

[S55] C++：结构化绑定
来源：http://hz.haohaochexian.top/gtytclowbp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangdashe.top/gtraizkbnq.html

[S56] C++：optional
来源：http://hz.smart0.xyz/gtbvtwuags.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.c1oappe.top/gtcppppglr.html

[S57] C++：编译期常量
来源：http://hz.zhaomingkeji.xyz/gtxohndumv.html

constexpr int N = 10;
来源：http://hz.zhaomingkeji.xyz/gtoxwejswi.html

[S58] C++：命名空间
来源：http://hz.shanyushiyangtech.top/gtdnvlzxze.html

namespace ns { int f() { return 1; } }
来源：http://hz.gotoacloud.top/gtoubyyhwe.html

[S59] C++：静态断言
来源：http://hz.shangyingyoupin.top/gtwebqokiw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigufen.top/gteysiratk.html

[S60] C++：遍历并删除元素
来源：http://hz.zycfv.cn/gtivyzzaud.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jqgfzy.top/gtilyaozcm.html

================================================================================
来源：http://hz.nwbrower.top/gtbmhmzjzg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shangyingyoupin.top/gtuvdxxxkt.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthhpauhgt.html

[T01] Kotlin：Hello World
来源：http://hz.cheryme.top/gtetlripat.html

println("Hello")
来源：http://hz.cqqwz.cn/gtrnuugqis.html

[T02] Kotlin：变量
来源：http://hz.jianghu66.top/gtrhcaybnc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.316326.xyz/gtqsfslbhh.html

[T03] Kotlin：字符串模板
来源：http://hz.wangdashe.top/gtgnpxvemr.html

"值: $b"
来源：http://hz.tianlin.xyz/gtscrselib.html

[T04] Kotlin：空安全
来源：http://hz.pycfn.com/gtzeghuqbi.html

val n: String? = null;  n?.length
来源：http://hz.0kj1m.cn/gtiotsbxdq.html

[T05] Kotlin：when 表达式
来源：http://hz.hnqzz.top/gtnqkjygog.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.smart0.xyz/gtanfqhbxp.html

[T06] Kotlin：集合映射
来源：http://hz.vqdsnc.cn/gtnmvryywi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ehwqpu.com/gtklxxofhz.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gtfcbjhwhk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhoulong.xyz/gtuaubqphv.html

[T08] Kotlin：数据类
来源：http://hz.dianchejie.cn/gttdbgpidz.html

data class User(val name: String, val age: Int)
来源：http://hz.zhongyouzk.top/gtzraimmvi.html

[T09] Kotlin：扩展函数
来源：http://hz.hongshengwenyu.top/gtmkcvjdnh.html

fun String.exclaim() = this + "!"
来源：http://hz.0kj1m.cn/gtpwqbhbeg.html

[T10] Kotlin：默认参数
来源：http://hz.cdnleiting.top/gtrccjrjlb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.meibo888.top/gtyhbmhzlu.html

[T11] Kotlin：协程
来源：http://hz.snrcjt.cn/gtuiurdugo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhongyouzk.top/gtubjtybtv.html

[T12] Kotlin：解构声明
来源：http://hz.gaohongyu789.top/gtvxjdbwib.html

val (a, b) = Pair(1, 2)
来源：http://hz.xziqi.cn/gtmeshauwc.html

[T13] Kotlin：只读 Map
来源：http://hz.shanyushiyangkeji.top/gtzxrwvbue.html

val m = mapOf("a" to 1)
来源：http://hz.shangyingyoupin.top/gtqutnfxhp.html

[T14] Kotlin：循环
来源：http://hz.bjfxy.top/gtlqshzoxf.html

for (i in 1..10) println(i)
来源：http://hz.hnqzz.top/gtchtzsobx.html

[T15] Kotlin：接口
来源：http://hz.xinyue.icu/gtrxhghwdq.html

interface Shape { fun area(): Double }
来源：http://hz.316326.xyz/gtbakoxbmr.html

[T16] Swift：Hello World
来源：http://hz.hfpthk.cn/gttjkinjfp.html

print("Hello")
来源：http://hz.ybcxt.top/gttbczsoey.html

[T17] Swift：变量与常量
来源：http://hz.zhiwuduotai.top/gtyzjtntom.html

var a = 1;  let b = 2
来源：http://hz.yuxming.cn/gtxvmgdony.html

[T18] Swift：字符串插值
来源：http://hz.tianlin.xyz/gtrurodcvv.html

"值: \(b)"
来源：http://hz.haohaochexian.top/gtorjpxbsa.html

[T19] Swift：可选绑定
来源：http://hz.zhiwuduotai.top/gtqcpjdamm.html

if let n = opt { print(n) }
来源：http://hz.ppjwa.cn/gtehvrnmbf.html

[T20] Swift：数组操作
来源：http://hz.kuanghao11.cn/gtusmbdvgm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.nanxinkj.top/gtpziostwt.html

[T21] Swift：遍历
来源：http://hz.sysykeji.top/gthhwwcmqk.html

for x in a { print(x) }
来源：http://hz.jinqigfzy.top/gteflrsati.html

[T22] Swift：字典
来源：http://hz.hnxiangtu.top/gtruqrslhi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shzxlz.cn/gtojzzmozn.html

[T23] Swift：函数
来源：http://hz.yuxming.cn/gtvozmqcqu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jiagoushi.top/gtkeaibwas.html

[T24] Swift：闭包
来源：http://hz.nanxinkj.top/gtzvkkudyw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xziqi.cn/gtryhsvbjf.html

[T25] Swift：结构体
来源：http://hz.cdnleiting.top/gttewpnwmz.html

struct P { var x: Int }
来源：http://hz.yj20258.top/gtmllhbkyn.html

[T26] Swift：类与重写
来源：http://hz.nanxinkj.top/gthyfbdzlo.html

class A: Base { override func f() {} }
来源：http://hz.hammf.cn/gtcvrvgvmu.html

[T27] Swift：错误处理
来源：http://hz.zhijiandao.cn/gtzgvbyrus.html

do { try f() } catch { print(error) }
来源：http://hz.jiagoushi.top/gtavvtlwyy.html

[T28] Swift：枚举
来源：http://hz.ivvv.top/gtmcnpxief.html

enum Color { case red, green }
来源：http://hz.quarkkingdee.top/gtqdmkhpzg.html

[T29] Swift：guard 提前返回
来源：http://hz.jyoumei.cn/gtebrqpnfy.html

guard let x = opt else { return }
来源：http://hz.wangdashe.top/gtjopvplas.html

[T30] Swift：协议
来源：http://hz.wangdashe.top/gttzxxcshc.html

protocol Shape { func area() -> Double }
来源：http://hz.hfpthk.cn/gtjwwrxyqs.html

[T31] Lua：Hello World
来源：http://hz.andypj.xyz/gtmvnwxhtv.html

print("Hello")
来源：http://hz.zhixingplan.top/gtmjcsqvup.html

[T32] Lua：局部变量
来源：http://hz.ppjwa.cn/gtzijejypw.html

local a = 1
来源：http://hz.cqqwz.cn/gtyqtqxdmc.html

[T33] Lua：表（数组）
来源：http://hz.ydzc1.top/gtawjmhlvl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.svipenyu.cn/gtwuevvndh.html

[T34] Lua：遍历表
来源：http://hz.shanyushiyangkeji.top/gtywqdxaud.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cashguo.top/gtrwaofqgm.html

[T35] Lua：字典表
来源：http://hz.xinyue.icu/gtecktatax.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yueranfly.top/gtoubwarjh.html

[T36] Lua：函数
来源：http://hz.ppjwa.cn/gtvifnowhq.html

function add(a, b) return a + b end
来源：http://hz.xuetiantiany.cn/gtntjxnggu.html

[T37] Lua：字符串拼接
来源：http://hz.gotoacloud.top/gtpdqschdd.html

"a" .. "b"
来源：http://hz.yueranfly.top/gtafdzwbhi.html

[T38] Lua：条件
来源：http://hz.svipenyu.cn/gtfjhbyulr.html

if x > 0 then print("正") end
来源：http://hz.jqgufenzy.top/gtlxpqkmtk.html

[T39] Lua：模式匹配
来源：http://hz.shanyushiyangkeji.top/gttngzayhn.html

string.find(s, "%d+")
来源：http://hz.feifeiyinyue.top/gtjnwowfcr.html

[T40] Lua：元表
来源：http://hz.yonumen.top/gtzwwkvgtx.html

setmetatable({}, { __index = base })
来源：http://hz.zhongyouzk.top/gtjralhycl.html

[T41] Perl：Hello World
来源：http://hz.sxryk.cn/gtdptnjrxf.html

print "Hello\n";
来源：http://hz.jqgufenzy.top/gtvjgbevjr.html

[T42] Perl：变量类型
来源：http://hz.sweek.top/gtavvwnbyv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xziqi.cn/gtgkmvybyx.html

[T43] Perl：字符串插值
来源：http://hz.zhiwuduotai.top/gtsydbikon.html

"值: $a"
来源：http://hz.hysaishi.cn/gtjgvjwoqo.html

[T44] Perl：条件
来源：http://hz.zdqjudy.top/gtcpvqbnqq.html

if ($a > 0) { print "正"; }
来源：http://hz.yj202588.top/gtsorolmda.html

[T45] Perl：数组遍历
来源：http://hz.jqgufenzy.top/gtfvicsbrx.html

for my $x (@arr) { print $x; }
来源：http://hz.yongpay.top/gtxlmswbix.html

[T46] Perl：哈希操作
来源：http://hz.hnxiangtu.top/gtidaniyyx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yanxiufei.cn/gtkxcdhkwb.html

[T47] Perl：正则捕获
来源：http://hz.gogol.net.cn/gtcbmbflvw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hywenlv.cn/gttirujmro.html

[T48] Perl：正则替换
来源：http://hz.yj20258.top/gtgvmybfkf.html

$s =~ s/old/new/g;
来源：http://hz.jianghu66.top/gtxcvollhy.html

[T49] Perl：函数
来源：http://hz.0kj1m.cn/gtfnqijyhw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tanke756.top/gtsimktoqa.html

[T50] Perl：逐行读文件
来源：http://hz.smart0.xyz/gttfftiozq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydjk.org.cn/gtfcengdqi.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yongpay.top/gtkkbmlftv.html

[T51] Scala：Hello World
来源：http://hz.pengpengdd.cyou/gtkcwqcyju.html

println("Hello")
来源：http://hz.yanxiufei.cn/gtyrjjaabq.html

[T52] Scala：变量
来源：http://hz.pycfn.com/gtvguntgow.html

val a = 1;  var b = 2
来源：http://hz.zdqjudy.top/gtemktjcgh.html

[T53] Scala：字符串插值
来源：http://hz.xinyue.icu/gtpnunqrmc.html

s"值: $b"
来源：http://hz.ywan-chungtsiang.top/gtkydbiquj.html

[T54] Scala：集合映射
来源：http://hz.jiagoushi.top/gtfneugfor.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.tianlin.xyz/gtucvvqbbj.html

[T55] Scala：集合过滤
来源：http://hz.yj20258.top/gtknnybwwt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hnxiangtu.top/gtzcjwrjiz.html

[T56] Scala：样例类
来源：http://hz.dashuyun.cn/gtzwmmxyzj.html

case class User(name: String, age: Int)
来源：http://hz.yj20258888.top/gtzcsjjiif.html

[T57] Scala：模式匹配
来源：http://hz.zhengqikj.top/gtqlaiehls.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.daxiang520.top/gtegnihmvz.html

[T58] Scala：函数定义
来源：http://hz.pycfn.com/gtrvsqogga.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.guannengcc.top/gtkgcdlcbo.html

[T59] Scala：循环
来源：http://hz.meibo888.top/gtgknopeeg.html

for (i <- 1 to 10) println(i)
来源：http://hz.xylfe.cn/gtxqmcyvwj.html

[T60] Scala：折叠
来源：http://hz.guannengcc.top/gtsgemapvi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.daria6918.cn/gtlybxvxxy.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtkwgnobkf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhengqikj.top/gtvsgycxtp.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthspixcar.html

[U01] Py：创建虚拟环境
来源：http://hz.wangdashe.top/gtsohxmcqf.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.quarkkingdee.top/gtoabpzifi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.iojbl.cn/gtqfjwejgm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yuxming.cn/gthoortzcn.html

[U03] Py：加载 .env 配置
来源：http://hz.fengsongda.top/gtbvjeusmo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhengqikj.top/gtwxgnaoyx.html

[U04] Py：变量调试打印
来源：http://hz.yonumen.top/gtdipdzlwo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cucudq.cn/gtleuircrh.html

[U05] Py：列表去重且保序
来源：http://hz.jqgufenzy.top/gtdfdkemyi.html

list(dict.fromkeys(arr))
来源：http://hz.daxiang520.top/gtclezncxx.html

[U06] Py：合并两个字典
来源：http://hz.svipenyu.cn/gtujfymbuf.html

{**a, **b}
来源：http://hz.hnxiangtu.top/gthipjbryw.html

[U07] Py：反转字典键值
来源：http://hz.guowangkeji.top/gttsthjvwv.html

{v: k for k, v in d.items()}
来源：http://hz.ivvv.top/gtruanqdce.html

[U08] Py：展平二维列表
来源：http://hz.fzhhl.top/gtjxzwkbrn.html

[y for x in nested for y in x]
来源：http://hz.havefunace.top/gtrepzuvqq.html

[U09] Py：字典取最大值的键
来源：http://hz.yongpay.top/gtguiigsxw.html

max(d, key=d.get)
来源：http://hz.jinyuanbaomall.cn/gtrenaxjwp.html

[U10] Py：按值排序字典
来源：http://hz.cheryme.top/gtbuitebhl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yuanzhike.top/gtjaxcyipf.html

[U11] Py：生成器表达式
来源：http://hz.andypj.xyz/gtymplrwdu.html

(x * 2 for x in arr)
来源：http://hz.xziqi.cn/gtnfhokiij.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yj202588.top/gtoqramkve.html

Counter(arr).most_common(3)
来源：http://hz.yuxming.cn/gtogkfmabx.html

[U13] Py：固定长度队列
来源：http://hz.cheryme.top/gtpsomphdf.html

deque(maxlen=10)
来源：http://hz.cashguo.top/gtuuouayyc.html

[U14] Py：分组收集到列表
来源：http://hz.yongpay.top/gttvbgiyap.html

defaultdict(list)
来源：http://hz.jqgfzy.top/gtrpmvviye.html

[U15] Py：高精度计时
来源：http://hz.kuanghao11.cn/gtsazkpntb.html

t = time.perf_counter()
来源：http://hz.guowangkeji.top/gtwminpaxq.html

[U16] Py：命令行参数解析
来源：http://hz.jinyuanbaomall.cn/gtconilxwj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.svipenyu.cn/gtqgksajml.html

[U17] Py：初始化日志
来源：http://hz.316326.xyz/gthotucnue.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.wangdashe.top/gtdcpewkfr.html

[U18] Py：预编译正则
来源：http://hz.zhijiandao.cn/gtthvnrhed.html

pat = re.compile(r"\d+")
来源：http://hz.gzhubu.top/gtinvvtykg.html

[U19] Py：正则替换带回调
来源：http://hz.gotoacloud.top/gtdqfnbxpg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cheryme.top/gtifzalhdq.html

[U20] Py：缓存函数结果
来源：http://hz.svipenyu.cn/gtvbxmnexf.html

@functools.lru_cache(maxsize=None)
来源：http://hz.nanxuanxn.top/gtafvozeob.html

[U21] Py：自定义上下文管理器
来源：http://hz.chenzaomai.com/gthkepzboi.html

@contextlib.contextmanager
来源：http://hz.hfpthk.cn/gtckalimuf.html

[U22] Py：矩阵转置
来源：http://hz.haohaochexian.top/gtqnxkadle.html

list(zip(*m))
来源：http://hz.zhiwuduotai.top/gtidmxsgbv.html

[U23] Py：分块读取大文件
来源：http://hz.c1oappe.top/gtgjvspwrq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.ehwqpu.com/gtohiuilxz.html

[U24] Py：路径操作
来源：http://hz.aizwys.cn/gtdluwwsxn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.nanxinkj.top/gtegpmwhes.html

[U25] Py：CSV 按字典读
来源：http://hz.jinqigfzy.top/gtlpawsrfg.html

csv.DictReader(f)
来源：http://hz.xingfuxueyuan.xyz/gtyitrxbnb.html

[U26] Py：并发下载
来源：http://hz.xuetiantiany.cn/gtchwjlcmx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yuxming.cn/gtzpacywfo.html

[U27] Py：异步 HTTP
来源：http://hz.jqgfzy.top/gtfefodwkd.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.wangshuangyany.cn/gtpmyroadj.html

[U28] Py：类型别名
来源：http://hz.smart0.xyz/gtqibgbxli.html

UserId = int
来源：http://hz.jinghuilouyu.cn/gtgjcavwdi.html

[U29] Py：属性校验
来源：http://hz.ybcxt.top/gtpztqogjc.html

@property 与 @x.setter 配合
来源：http://hz.zdqjudy.top/gtxcnwtypn.html

[U30] Py：数据类
来源：http://hz.bjfxy.top/gtxtkflwfg.html

@dataclass(slots=True)
来源：http://hz.guannengcc.top/gtedugjwpk.html

[U31] Py：单测
来源：http://hz.jqgfzy.top/gttjfeiyxa.html

python -m pytest -q
来源：http://hz.wangdashe.top/gtfvzgkueb.html

[U32] Py：代码格式化
来源：http://hz.yj20258.top/gtfwndxayn.html

ruff format . && ruff check --fix .
来源：http://hz.jinyuanbaomall.cn/gtzkzhzjhh.html

[U33] Py：打包发布
来源：http://hz.svipenyu.cn/gtnenjuldh.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hysaishi.cn/gtbqhjrnoo.html

[U34] Py：判断编码
来源：http://hz.52xcode.cn/gtdetpnmvm.html

chardet.detect(raw)
来源：http://hz.yj202588.top/gtnpjijreu.html

[U35] Py：发送邮件
来源：http://hz.gaohongyu789.top/gtgufnldxp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.birdmap.top/gtdyqrhcml.html

[U36] Py：定时任务
来源：http://hz.wangdashe.top/gtvizrzorq.html

schedule.every(10).minutes.do(job)
来源：http://hz.0kj1m.cn/gtaakrfbuz.html

[U37] Py：读写 Excel
来源：http://hz.xinyue.icu/gtfrccnmes.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shangyingyoupin.top/gtjsbvevbe.html

[U38] Py：获取脚本所在目录
来源：http://hz.sxryk.cn/gtprjdvvur.html

Path(__file__).resolve().parent
来源：http://hz.ydjk.org.cn/gttkbgrgnt.html

[U39] Py：判断是否在交互环境
来源：http://hz.nanxuanxn.top/gtkfirjwjb.html

sys.stdout.isatty()
来源：http://hz.shanyushiyangkeji.top/gtizygocup.html

[U40] Py：打印到标准错误
来源：http://hz.9152youxi.cn/gtxaksucfe.html

print("err", file=sys.stderr)
来源：http://hz.hnqzz.top/gtcjaggefg.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.guowangkeji.top/gtqzpljcas.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.316326.xyz/gtoxfudvwj.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.9152youxi.cn/gtgmlxnvoo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ydjk.org.cn/gteervxouf.html

[U43] PHP：声明命名空间
来源：http://hz.nanxuanxn.top/gtyiwvunib.html

namespace App\Http;
来源：http://hz.nwbrower.top/gtcdvfxqsy.html

[U44] PHP：开启严格类型
来源：http://hz.bjfxy.top/gtgafjkdjz.html

declare(strict_types=1);
来源：http://hz.gaohongyu789.top/gtqvgwulmc.html


<!-- 参考信息 -->