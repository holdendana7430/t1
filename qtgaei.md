代发 wailian999

#ifndef X_H
来源：http://hz.quarkkingdee.top/gtqfgfsxxm.html

#define X_H
来源：http://hz.zhengqikj.top/gtksqsqxnb.html

#endif
来源：http://hz.zycfv.cn/gtxpjdxvua.html

[S31] C++：Hello World
来源：http://hz.yueranfly.top/gtoyzxdttw.html

#include <iostream>
来源：http://hz.gaohongyu789.top/gtddsshrot.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hongshengwenyu.top/gtbqpwxxat.html

[S32] C++：字符串
来源：http://hz.pengpengdd.cyou/gtwyuqlazr.html

std::string s = "hi";  s += "!";
来源：http://hz.nwbrower.top/gthzyrnkrv.html

[S33] C++：vector 增删
来源：http://hz.gogol.net.cn/gtkelmmpah.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.daxiang520.top/gtlsmhbzkx.html

[S34] C++：遍历 vector
来源：http://hz.tanke756.top/gtiqphywww.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhiwuduotai.top/gthziubqla.html

[S35] C++：map
来源：http://hz.ybcxt.top/gtjtfrjfqa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zdqjudy.top/gtthwmqvqq.html

[S36] C++：unordered_map
来源：http://hz.tianlin.xyz/gtrsuwmogc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtyhvbwrqe.html

[S37] C++：set
来源：http://hz.yj20258888.top/gtcsubusno.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hongshengwenyu.top/gtgthlxzdv.html

[S38] C++：排序
来源：http://hz.andypj.xyz/gtvnrepeqv.html

std::sort(v.begin(), v.end());
来源：http://hz.yj20258.top/gtoxlusobu.html

[S39] C++：自定义比较器排序
来源：http://hz.zhoulong.xyz/gtjntruyzn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj202588.top/gtybsyxznu.html

[S40] C++：查找元素
来源：http://hz.daria6918.cn/gtspyloxnb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.316326.xyz/gtntwqgzsm.html

[S41] C++：类与构造函数
来源：http://hz.zhoulong.xyz/gtrkzxsqyw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.haohaochexian.top/gtfavqzdkf.html

[S42] C++：继承与虚函数
来源：http://hz.ywan-chungtsiang.top/gtdomosbpe.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhaomingkeji.xyz/gtdwjunlei.html

[S43] C++：智能指针
来源：http://hz.xylfe.cn/gtmxvyjter.html

auto p = std::make_unique<int>(5);
来源：http://hz.xingfuxueyuan.xyz/gtzwawtjcl.html

[S44] C++：引用传参
来源：http://hz.aizwys.cn/gtviolaqjx.html

void inc(int &x) { ++x; }
来源：http://hz.chenlongwang.top/gtxlgqflau.html

[S45] C++：lambda
来源：http://hz.haohaochexian.top/gtocolgryp.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinghuilouyu.cn/gtskcpbkby.html

[S46] C++：函数模板
来源：http://hz.bjfxy.top/gtdohfrrfj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.mhx1999.top/gtyflggsqp.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigfzy.top/gtjrlerhlw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgufenzy.top/gtnorahave.html

[S48] C++：逐行读文件
来源：http://hz.iojbl.cn/gttotguzmt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinqigfzy.top/gtpirkltyb.html

while (std::getline(in, line)) { }
来源：http://hz.zdqjudy.top/gtbziqdiqw.html

[S49] C++：写文件
来源：http://hz.yj20258.top/gtvniihiul.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aizwys.cn/gtjqvhtxct.html

[S50] C++：格式化数字
来源：http://hz.xinyue.icu/gttjuesxnj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtiqxhwbdv.html

[S51] C++：显式类型转换
来源：http://hz.smart0.xyz/gtoewgjlty.html

static_cast<double>(a) / b
来源：http://hz.cdnleiting.top/gtppcpodtk.html

[S52] C++：const 与 noexcept
来源：http://hz.shangyingyoupin.top/gtzjlwstwg.html

int size() const noexcept { return n_; }
来源：http://hz.zhongyouzk.top/gtflleyjem.html

[S53] C++：移动语义
来源：http://hz.cucudq.cn/gtvcuqraid.html

std::vector<int> w = std::move(v);
来源：http://hz.chenzaomai.com/gttuysmpyp.html

[S54] C++：异常处理
来源：http://hz.xingfuxueyuan.xyz/gtdqrvoabb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinqigufen.top/gtpsudjaym.html

[S55] C++：结构化绑定
来源：http://hz.zhaomingkeji.xyz/gtaedilogi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.feifeiyinyue.top/gtvteughyw.html

[S56] C++：optional
来源：http://hz.zhixingplan.top/gtrgvjkrxx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtsdfzqyts.html

[S57] C++：编译期常量
来源：http://hz.zhixingplan.top/gtqqfayazi.html

constexpr int N = 10;
来源：http://hz.bjfxy.top/gtvhrfernf.html

[S58] C++：命名空间
来源：http://hz.havefunace.top/gtgqvggupq.html

namespace ns { int f() { return 1; } }
来源：http://hz.wangdashe.top/gtcwyimyuu.html

[S59] C++：静态断言
来源：http://hz.xuetiantiany.cn/gtwlplmzkg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xuetiantiany.cn/gtaemkmlay.html

[S60] C++：遍历并删除元素
来源：http://hz.kuanghao11.cn/gthmeokode.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sxryk.cn/gtwjrybrlu.html

================================================================================
来源：http://hz.andypj.xyz/gtyrhtlujy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sysykeji.top/gtnrvtkprz.html

================================================================================
来源：http://hz.jiagoushi.top/gtzxgijhlm.html

[T01] Kotlin：Hello World
来源：http://hz.yonumen.top/gtipgntsyx.html

println("Hello")
来源：http://hz.xylfe.cn/gtnoquyubb.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangkeji.top/gtnjoytdfv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.smart0.xyz/gtnqcjzjfx.html

[T03] Kotlin：字符串模板
来源：http://hz.sysykeji.top/gtbryvwzex.html

"值: $b"
来源：http://hz.zhiwuduotai.top/gtmimzxlpp.html

[T04] Kotlin：空安全
来源：http://hz.jlsjyb.cn/gtdbvaqsxu.html

val n: String? = null;  n?.length
来源：http://hz.yongpay.top/gtzetvidaz.html

[T05] Kotlin：when 表达式
来源：http://hz.hammf.cn/gtttynkzlp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sxryk.cn/gthdrglthr.html

[T06] Kotlin：集合映射
来源：http://hz.xuanzx.com/gttmjezjja.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hongshengwenyu.top/gtkrobvujt.html

[T07] Kotlin：集合过滤
来源：http://hz.vqdsnc.cn/gtxfmrwtpb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.snrcjt.cn/gtnpsxdoyf.html

[T08] Kotlin：数据类
来源：http://hz.cashguo.top/gtezqhyqxg.html

data class User(val name: String, val age: Int)
来源：http://hz.jianghu66.top/gtfjhaewdn.html

[T09] Kotlin：扩展函数
来源：http://hz.sweek.top/gtylnezdbk.html

fun String.exclaim() = this + "!"
来源：http://hz.yj202588.top/gtjfpvcnzz.html

[T10] Kotlin：默认参数
来源：http://hz.xziqi.cn/gtpnmwyprh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgfzy.top/gtwiymzytj.html

[T11] Kotlin：协程
来源：http://hz.gaohongyu789.top/gtdiuenskv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daxiang520.top/gtrdueqxzq.html

[T12] Kotlin：解构声明
来源：http://hz.ywan-chungtsiang.top/gtibkokzzh.html

val (a, b) = Pair(1, 2)
来源：http://hz.dashuyun.cn/gtlcffnops.html

[T13] Kotlin：只读 Map
来源：http://hz.0kj1m.cn/gtqaellmwr.html

val m = mapOf("a" to 1)
来源：http://hz.sufxvd.cn/gtufyktyzy.html

[T14] Kotlin：循环
来源：http://hz.daria6918.cn/gtctwxdynm.html

for (i in 1..10) println(i)
来源：http://hz.zycfv.cn/gtvbrwpekp.html

[T15] Kotlin：接口
来源：http://hz.xinyue.icu/gtfovtuvgp.html

interface Shape { fun area(): Double }
来源：http://hz.meibo888.top/gtnhizgdvf.html

[T16] Swift：Hello World
来源：http://hz.shuidangran.top/gtumdufoap.html

print("Hello")
来源：http://hz.gaohongyu789.top/gtzcxggqpv.html

[T17] Swift：变量与常量
来源：http://hz.gzhubu.top/gtpyvivtbl.html

var a = 1;  let b = 2
来源：http://hz.zhaomingkeji.xyz/gtmnhzaluh.html

[T18] Swift：字符串插值
来源：http://hz.chenlongwang.top/gtjxktbgve.html

"值: \(b)"
来源：http://hz.jinqigfzy.top/gtvipvvwlt.html

[T19] Swift：可选绑定
来源：http://hz.yonumen.top/gtwudwbqzy.html

if let n = opt { print(n) }
来源：http://hz.jinghuilouyu.cn/gtgegxuehg.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gtowqqrvzr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigufen.top/gtrzieyefp.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gtkfmjbufb.html

for x in a { print(x) }
来源：http://hz.ybcxt.top/gtpkairneh.html

[T22] Swift：字典
来源：http://hz.aibaodan.cn/gtaukwjild.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ppjwa.cn/gtlqlhoemf.html

[T23] Swift：函数
来源：http://hz.feifeiyinyue.top/gtajozmvyh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cucudq.cn/gtqnlmejup.html

[T24] Swift：闭包
来源：http://hz.xingfuxueyuan.xyz/gtskkruegz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.kuanghao11.cn/gthhlfwqgs.html

[T25] Swift：结构体
来源：http://hz.xuanzx.com/gtwwsvyfzo.html

struct P { var x: Int }
来源：http://hz.jlsjyb.cn/gtytwlphop.html

[T26] Swift：类与重写
来源：http://hz.wangshuangyany.cn/gtdlarsrbm.html

class A: Base { override func f() {} }
来源：http://hz.mhx1999.top/gtvbvjvbmp.html

[T27] Swift：错误处理
来源：http://hz.haohaochexian.top/gtfgtlamdi.html

do { try f() } catch { print(error) }
来源：http://hz.zhoulong.xyz/gtzwrfvmrw.html

[T28] Swift：枚举
来源：http://hz.c1oappe.top/gtuloegydu.html

enum Color { case red, green }
来源：http://hz.andypj.xyz/gtbzkatnfi.html

[T29] Swift：guard 提前返回
来源：http://hz.hywenlv.cn/gtedzhsion.html

guard let x = opt else { return }
来源：http://hz.havefunace.top/gthhavswnf.html

[T30] Swift：协议
来源：http://hz.nanxuanxn.top/gtfteijbwl.html

protocol Shape { func area() -> Double }
来源：http://hz.gogol.net.cn/gtizkfuywr.html

[T31] Lua：Hello World
来源：http://hz.haohaochexian.top/gtutjzipoq.html

print("Hello")
来源：http://hz.ivvv.top/gtmtpthlrf.html

[T32] Lua：局部变量
来源：http://hz.gzhubu.top/gtvbkkneac.html

local a = 1
来源：http://hz.yj202588.top/gtuykrfuou.html

[T33] Lua：表（数组）
来源：http://hz.tianlin.xyz/gtiwtxvvpi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yueranfly.top/gtdbjxpumy.html

[T34] Lua：遍历表
来源：http://hz.ehwqpu.com/gtmhrjdkcg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.chenjidiqi.icu/gtokxgvglt.html

[T35] Lua：字典表
来源：http://hz.hnxiangtu.top/gtyjqnkxwq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.kuanghao11.cn/gtercoaadj.html

[T36] Lua：函数
来源：http://hz.zhijiandao.cn/gtumrdlgda.html

function add(a, b) return a + b end
来源：http://hz.aibaodan.cn/gtzshdxypl.html

[T37] Lua：字符串拼接
来源：http://hz.xinyue.icu/gtkwvgkxua.html

"a" .. "b"
来源：http://hz.birdmap.top/gtqpwgeolo.html

[T38] Lua：条件
来源：http://hz.yvedp.cn/gtombcttxn.html

if x > 0 then print("正") end
来源：http://hz.nanxuanxn.top/gtvlbjjnnk.html

[T39] Lua：模式匹配
来源：http://hz.guowangkeji.top/gtkqjodfpq.html

string.find(s, "%d+")
来源：http://hz.jqgfzy.top/gtwyjulxno.html

[T40] Lua：元表
来源：http://hz.sweek.top/gtrzlzqfik.html

setmetatable({}, { __index = base })
来源：http://hz.sufxvd.cn/gtrmuflewy.html

[T41] Perl：Hello World
来源：http://hz.zhijiandao.cn/gthuxyrhql.html

print "Hello\n";
来源：http://hz.ywan-chungtsiang.top/gtzxffttaf.html

[T42] Perl：变量类型
来源：http://hz.hnqzz.top/gtxxrnwoms.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jinyuanbaomall.cn/gtraxdmwkg.html

[T43] Perl：字符串插值
来源：http://hz.fengsongda.top/gtixwmpppk.html

"值: $a"
来源：http://hz.ydzc1.top/gtjhexrymz.html

[T44] Perl：条件
来源：http://hz.hongshengwenyu.top/gtlgbqbrxr.html

if ($a > 0) { print "正"; }
来源：http://hz.cqqwz.cn/gtkizgrzvw.html

[T45] Perl：数组遍历
来源：http://hz.jlsjyb.cn/gtrmqqcmvb.html

for my $x (@arr) { print $x; }
来源：http://hz.jinyuanbaomall.cn/gtvlmznccp.html

[T46] Perl：哈希操作
来源：http://hz.cheryme.top/gtiatakkgf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hysaishi.cn/gtsrzcwusl.html

[T47] Perl：正则捕获
来源：http://hz.shuidangran.top/gtmzeslmtl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cqqwz.cn/gtmaxxcldc.html

[T48] Perl：正则替换
来源：http://hz.guannengcc.top/gtznmafydr.html

$s =~ s/old/new/g;
来源：http://hz.gzhubu.top/gtmfjjuvnr.html

[T49] Perl：函数
来源：http://hz.9152youxi.cn/gtbgbkbpjx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gttvhoowfu.html

[T50] Perl：逐行读文件
来源：http://hz.snrcjt.cn/gtjquoxfgq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhijiandao.cn/gtgzvvxaok.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shanyushiyangkeji.top/gtvnrsohkd.html

[T51] Scala：Hello World
来源：http://hz.ydzc1.top/gtpsgvqdxu.html

println("Hello")
来源：http://hz.bjfxy.top/gtlxhyrvep.html

[T52] Scala：变量
来源：http://hz.316326.xyz/gtbbbguebl.html

val a = 1;  var b = 2
来源：http://hz.jqgufenzy.top/gtglvupzub.html

[T53] Scala：字符串插值
来源：http://hz.hfpthk.cn/gtgqwgohbs.html

s"值: $b"
来源：http://hz.snrcjt.cn/gtiesbaydx.html

[T54] Scala：集合映射
来源：http://hz.xinyue.icu/gtvmsbsfiz.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuxming.cn/gtchcelgbm.html

[T55] Scala：集合过滤
来源：http://hz.jqgfzy.top/gtzzrhfpek.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jqgufenzy.top/gtugvndryi.html

[T56] Scala：样例类
来源：http://hz.daxiang520.top/gtitdnllbo.html

case class User(name: String, age: Int)
来源：http://hz.zhongyouzk.top/gtpvgryihw.html

[T57] Scala：模式匹配
来源：http://hz.cashguo.top/gtlcamgjdq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhiwuduotai.top/gtiodjtxxz.html

[T58] Scala：函数定义
来源：http://hz.wangshuangyany.cn/gtjwxmxfuq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhixingplan.top/gttgsgdvpy.html

[T59] Scala：循环
来源：http://hz.kuanghao11.cn/gtlrovsqex.html

for (i <- 1 to 10) println(i)
来源：http://hz.cdnleiting.top/gtktiwgyut.html

[T60] Scala：折叠
来源：http://hz.jinghuilouyu.cn/gtrdnonrfq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cdnleiting.top/gtfnaaukrm.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgofwoxtu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.9152youxi.cn/gtiryesxpb.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtpbfbaksq.html

[U01] Py：创建虚拟环境
来源：http://hz.daxiang520.top/gtkuwzacyt.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jinqigufen.top/gtxrbkqucu.html

[U02] Py：导出 / 安装依赖
来源：http://hz.havefunace.top/gtmllktnji.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ydjk.org.cn/gtvgofnesg.html

[U03] Py：加载 .env 配置
来源：http://hz.quarkkingdee.top/gtmphbpiit.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.ywan-chungtsiang.top/gthtqexdwr.html

[U04] Py：变量调试打印
来源：http://hz.yvedp.cn/gtovakosjn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xinyue.icu/gtyidmttvg.html

[U05] Py：列表去重且保序
来源：http://hz.xuetiantiany.cn/gtapnrsdwy.html

list(dict.fromkeys(arr))
来源：http://hz.shuidangran.top/gtepjmfczu.html

[U06] Py：合并两个字典
来源：http://hz.guannengcc.top/gtsvkkuvyd.html

{**a, **b}
来源：http://hz.fengsongda.top/gtjpyznpoa.html

[U07] Py：反转字典键值
来源：http://hz.feifeiyinyue.top/gtrpmzekxu.html

{v: k for k, v in d.items()}
来源：http://hz.ywan-chungtsiang.top/gtnfqincru.html

[U08] Py：展平二维列表
来源：http://hz.yj20258.top/gtammnfhtn.html

[y for x in nested for y in x]
来源：http://hz.sysykeji.top/gtvzdyovfp.html

[U09] Py：字典取最大值的键
来源：http://hz.sxryk.cn/gtxujjqqyl.html

max(d, key=d.get)
来源：http://hz.shanyushiyangkeji.top/gtdcxxpquj.html

[U10] Py：按值排序字典
来源：http://hz.yj20258888.top/gtolutlwhu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gotoacloud.top/gtkagnzjeg.html

[U11] Py：生成器表达式
来源：http://hz.quarkkingdee.top/gtjetyemgn.html

(x * 2 for x in arr)
来源：http://hz.316326.xyz/gterhglpgl.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zdqjudy.top/gtcgdzwikz.html

Counter(arr).most_common(3)
来源：http://hz.jinqigufen.top/gtrdztipxv.html

[U13] Py：固定长度队列
来源：http://hz.yanxiufei.cn/gtfujyeyke.html

deque(maxlen=10)
来源：http://hz.shanyushiyangtech.top/gtimgprocz.html

[U14] Py：分组收集到列表
来源：http://hz.zhijiandao.cn/gtwmihrbvi.html

defaultdict(list)
来源：http://hz.daxiang520.top/gtswywjuah.html

[U15] Py：高精度计时
来源：http://hz.jinyuanbaomall.cn/gtxhhtkrlk.html

t = time.perf_counter()
来源：http://hz.yongpay.top/gtdezfremz.html

[U16] Py：命令行参数解析
来源：http://hz.fzhhl.top/gtpyalrmoi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hnqzz.top/gtnimpkpui.html

[U17] Py：初始化日志
来源：http://hz.shuidangran.top/gtipwvlbsc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fengsongda.top/gtkkylqrle.html

[U18] Py：预编译正则
来源：http://hz.ppjwa.cn/gtfydpmcoi.html

pat = re.compile(r"\d+")
来源：http://hz.guowangkeji.top/gtxdhibbca.html

[U19] Py：正则替换带回调
来源：http://hz.yangfankeji.com/gtyjfbabri.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.ppjwa.cn/gtnxuoumfw.html

[U20] Py：缓存函数结果
来源：http://hz.pycfn.com/gtcpcglmtt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.fengsongda.top/gtmfxubwyp.html

[U21] Py：自定义上下文管理器
来源：http://hz.ppjwa.cn/gtryatpntr.html

@contextlib.contextmanager
来源：http://hz.redwolf501.top/gtvmxqslhg.html

[U22] Py：矩阵转置
来源：http://hz.tianlin.xyz/gtncrqooqg.html

list(zip(*m))
来源：http://hz.bjfxy.top/gtximkrvnn.html

[U23] Py：分块读取大文件
来源：http://hz.jqgfzy.top/gtesqjosjj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.dianchejie.cn/gtxsmkvkyb.html

[U24] Py：路径操作
来源：http://hz.fengsongda.top/gtgfufnzvd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hfpthk.cn/gtplfqpenl.html

[U25] Py：CSV 按字典读
来源：http://hz.pengpengdd.cyou/gtuhkzmzqv.html

csv.DictReader(f)
来源：http://hz.chenjidiqi.icu/gtcvykbhil.html

[U26] Py：并发下载
来源：http://hz.jiagoushi.top/gtnxeaugar.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.haohaochexian.top/gtjnmqfeyh.html

[U27] Py：异步 HTTP
来源：http://hz.fzhhl.top/gtilwgctth.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.yonumen.top/gthyeqalnx.html

[U28] Py：类型别名
来源：http://hz.316326.xyz/gtlvjvflqj.html

UserId = int
来源：http://hz.yj202588.top/gtjkuwpnpb.html

[U29] Py：属性校验
来源：http://hz.jinghuilouyu.cn/gtftcztcod.html

@property 与 @x.setter 配合
来源：http://hz.jinqigufen.top/gtgfyrvfok.html

[U30] Py：数据类
来源：http://hz.wangshuangyany.cn/gtbdqpciqv.html

@dataclass(slots=True)
来源：http://hz.yuanzhike.top/gtcajpqfpi.html

[U31] Py：单测
来源：http://hz.dashuyun.cn/gtqxoirdxq.html

python -m pytest -q
来源：http://hz.nanxinkj.top/gtvhnqpzfl.html

[U32] Py：代码格式化
来源：http://hz.zhoulong.xyz/gtbgixfsfr.html

ruff format . && ruff check --fix .
来源：http://hz.yuxming.cn/gtdrnufvsy.html

[U33] Py：打包发布
来源：http://hz.yueranfly.top/gteqthenbi.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.birdmap.top/gtzdlwahfr.html

[U34] Py：判断编码
来源：http://hz.aizwys.cn/gtsuimhigp.html

chardet.detect(raw)
来源：http://hz.hnqzz.top/gtxebjskdi.html

[U35] Py：发送邮件
来源：http://hz.hysaishi.cn/gtkvukjpio.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xingfuxueyuan.xyz/gtfcuixjmw.html

[U36] Py：定时任务
来源：http://hz.xziqi.cn/gtcrdrytzj.html

schedule.every(10).minutes.do(job)
来源：http://hz.xylfe.cn/gtppalftrs.html

[U37] Py：读写 Excel
来源：http://hz.ydjk.org.cn/gtjfzjwwhl.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hnqzz.top/gtdiihrdap.html

[U38] Py：获取脚本所在目录
来源：http://hz.cheryme.top/gtcfnejsxh.html

Path(__file__).resolve().parent
来源：http://hz.hnxiangtu.top/gthmdbuknt.html

[U39] Py：判断是否在交互环境
来源：http://hz.gogol.net.cn/gtbxmlaqme.html

sys.stdout.isatty()
来源：http://hz.hysaishi.cn/gtedqdhnem.html

[U40] Py：打印到标准错误
来源：http://hz.sysykeji.top/gtwqhmdlvx.html

print("err", file=sys.stderr)
来源：http://hz.vqdsnc.cn/gtclpwbfmw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.vqdsnc.cn/gtsscqtiae.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhijiandao.cn/gteujilvfg.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.gotoacloud.top/gttgivjtnp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gogol.net.cn/gtvbuqsirj.html

[U43] PHP：声明命名空间
来源：http://hz.andypj.xyz/gtufdlawrw.html

namespace App\Http;
来源：http://hz.sweek.top/gtnoeqyxqn.html

[U44] PHP：开启严格类型
来源：http://hz.daxiang520.top/gtgzqkibtt.html

declare(strict_types=1);
来源：http://hz.zhengqikj.top/gtprnwachm.html

[U45] PHP：类型声明与返回类型
来源：http://hz.guowangkeji.top/gtradhapxz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daxiang520.top/gtjkyvodoe.html

[U46] PHP：可空类型
来源：http://hz.haohaochexian.top/gtbhdgimcy.html

?string $name = null
来源：http://hz.sxryk.cn/gtcpaowfve.html

[U47] PHP：联合类型
来源：http://hz.jinqigufen.top/gtzrjcycta.html

int|string $id
来源：http://hz.chenjidiqi.icu/gtgxqpwhli.html

[U48] PHP：纯枚举
来源：http://hz.jqgufenzy.top/gtjjfjipqx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ybcxt.top/gtqvaqyewz.html

[U49] PHP：只读属性
来源：http://hz.yanxiufei.cn/gtfmggwhld.html

public readonly string $name
来源：http://hz.yonumen.top/gtvngnmjhw.html

[U50] PHP：构造器属性提升
来源：http://hz.zhijiandao.cn/gtgpdwfqmz.html

public function __construct(private int $id) {}
来源：http://hz.shangyingyoupin.top/gtkawiszmw.html

[U51] PHP：数组解构
来源：http://hz.zhaomingkeji.xyz/gtxaklfikq.html

[$a, $b] = $arr;
来源：http://hz.birdmap.top/gtecqqckrb.html

[U52] PHP：箭头函数
来源：http://hz.zycfv.cn/gtytdhkwhh.html

$double = fn($x) => $x * 2;
来源：http://hz.nwbrower.top/gtqqocprwg.html

[U53] PHP：空合并运算符
来源：http://hz.hnqzz.top/gtrciattit.html

$v = $a ?? $b ?? "default";
来源：http://hz.ybcxt.top/gtgdrzphkj.html

[U54] PHP：空安全调用
来源：http://hz.cashguo.top/gtyuqixswe.html

$obj?->method()
来源：http://hz.smart0.xyz/gtqestkxwq.html


<!-- 参考信息 -->