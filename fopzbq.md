代发 wailian999

#ifndef X_H
来源：http://hz.xziqi.cn/gtlbqzxwth.html

#define X_H
来源：http://hz.hywenlv.cn/gtdyxdccmp.html

#endif
来源：http://hz.zhongyouzk.top/gtbhfiuymt.html

[S31] C++：Hello World
来源：http://hz.jyoumei.cn/gtiuvfxttg.html

#include <iostream>
来源：http://hz.ywan-chungtsiang.top/gtfktwshlu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gotoacloud.top/gteohcdqlk.html

[S32] C++：字符串
来源：http://hz.svipenyu.cn/gtovykixjd.html

std::string s = "hi";  s += "!";
来源：http://hz.andypj.xyz/gtbsklyehc.html

[S33] C++：vector 增删
来源：http://hz.andypj.xyz/gtgarzqowo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgfzy.top/gtbhjopesy.html

[S34] C++：遍历 vector
来源：http://hz.daria6918.cn/gtuposfong.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hammf.cn/gtfftxivrz.html

[S35] C++：map
来源：http://hz.yj20258888.top/gthhzwtvxh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtztqaahct.html

[S36] C++：unordered_map
来源：http://hz.yj20258.top/gtvtvhtskj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxinkj.top/gtqwzdwgrj.html

[S37] C++：set
来源：http://hz.shzxlz.cn/gtyyqowdwz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zdqjudy.top/gtqlttzagf.html

[S38] C++：排序
来源：http://hz.wangdashe.top/gtnrkbxvfv.html

std::sort(v.begin(), v.end());
来源：http://hz.gzhubu.top/gtryeigyvq.html

[S39] C++：自定义比较器排序
来源：http://hz.cdnleiting.top/gtcenuslzv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shzxlz.cn/gtndhxircr.html

[S40] C++：查找元素
来源：http://hz.yuanzhike.top/gthnrncojk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ydjk.org.cn/gttckfuizd.html

[S41] C++：类与构造函数
来源：http://hz.gzhubu.top/gtxxvoqfxn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hfpthk.cn/gtwdivlabn.html

[S42] C++：继承与虚函数
来源：http://hz.fengsongda.top/gtcgiorthz.html

class B : public Base { public: void f() override {} };
来源：http://hz.hfpthk.cn/gtclfxmeqb.html

[S43] C++：智能指针
来源：http://hz.ybcxt.top/gttmssxmgc.html

auto p = std::make_unique<int>(5);
来源：http://hz.sysykeji.top/gtfrexewew.html

[S44] C++：引用传参
来源：http://hz.hammf.cn/gtkcynokhv.html

void inc(int &x) { ++x; }
来源：http://hz.snrcjt.cn/gttpiubafw.html

[S45] C++：lambda
来源：http://hz.sweek.top/gtbnvuxibo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sxryk.cn/gtfmwchrxd.html

[S46] C++：函数模板
来源：http://hz.jqgufenzy.top/gtjojtploq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinghuilouyu.cn/gtwfjlhbpw.html

[S47] C++：结构化绑定遍历
来源：http://hz.fengsongda.top/gthcqougqb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guannengcc.top/gtrktoixbq.html

[S48] C++：逐行读文件
来源：http://hz.sweek.top/gtzpjqyesj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.guannengcc.top/gtlhtsnjid.html

while (std::getline(in, line)) { }
来源：http://hz.pycfn.com/gtwqdbuvht.html

[S49] C++：写文件
来源：http://hz.jqgufenzy.top/gtwjlecbtx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.quarkkingdee.top/gtrueznqfa.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtefrzbnvi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.vqdsnc.cn/gtqqumnsvs.html

[S51] C++：显式类型转换
来源：http://hz.cucudq.cn/gtqhckdsxo.html

static_cast<double>(a) / b
来源：http://hz.ybcxt.top/gtvaugodnp.html

[S52] C++：const 与 noexcept
来源：http://hz.zhixingplan.top/gtrjqlzkyt.html

int size() const noexcept { return n_; }
来源：http://hz.ydzc1.top/gtmoyvxzrk.html

[S53] C++：移动语义
来源：http://hz.yuxming.cn/gtuoqdzvbx.html

std::vector<int> w = std::move(v);
来源：http://hz.wangshuangyany.cn/gtqfngpove.html

[S54] C++：异常处理
来源：http://hz.xuanzx.com/gtaxiufkvl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yangfankeji.com/gtaictejdi.html

[S55] C++：结构化绑定
来源：http://hz.meibo888.top/gteisfoasd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.guowangkeji.top/gttojllsbe.html

[S56] C++：optional
来源：http://hz.zhoulong.xyz/gteiukssbx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.havefunace.top/gtpdhpogfi.html

[S57] C++：编译期常量
来源：http://hz.yuanzhike.top/gtlbvyqwqg.html

constexpr int N = 10;
来源：http://hz.fzhhl.top/gtxmxfpugv.html

[S58] C++：命名空间
来源：http://hz.pengpengdd.cyou/gtdbamqjld.html

namespace ns { int f() { return 1; } }
来源：http://hz.hysaishi.cn/gtjfgfqsdc.html

[S59] C++：静态断言
来源：http://hz.vqdsnc.cn/gtgzjuzeis.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gotoacloud.top/gtpetxdgup.html

[S60] C++：遍历并删除元素
来源：http://hz.ydzc1.top/gtgaktpmny.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gotoacloud.top/gtizevbeeu.html

================================================================================
来源：http://hz.chenzaomai.com/gtkkhguqll.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258.top/gtwjfzjxog.html

================================================================================
来源：http://hz.wangdashe.top/gtolvqmprf.html

[T01] Kotlin：Hello World
来源：http://hz.daria6918.cn/gtoafybhok.html

println("Hello")
来源：http://hz.daxiang520.top/gtmobwtcca.html

[T02] Kotlin：变量
来源：http://hz.cqqwz.cn/gtwtglisqr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenzaomai.com/gthfjlamqg.html

[T03] Kotlin：字符串模板
来源：http://hz.shzxlz.cn/gthgohayej.html

"值: $b"
来源：http://hz.jinqigufen.top/gthkroweyp.html

[T04] Kotlin：空安全
来源：http://hz.ivvv.top/gttznnlhux.html

val n: String? = null;  n?.length
来源：http://hz.jinqigufen.top/gtbqmykbge.html

[T05] Kotlin：when 表达式
来源：http://hz.yj202588.top/gtzfeoalpw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.snrcjt.cn/gthpwetlnq.html

[T06] Kotlin：集合映射
来源：http://hz.yj20258.top/gtudkcrjnf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tian-w.cn/gtilnpuwus.html

[T07] Kotlin：集合过滤
来源：http://hz.shanyushiyangtech.top/gtfaxrsmya.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.smart0.xyz/gtxcrvqkdi.html

[T08] Kotlin：数据类
来源：http://hz.zdqjudy.top/gtasrpoiru.html

data class User(val name: String, val age: Int)
来源：http://hz.cucudq.cn/gtjntpapaq.html

[T09] Kotlin：扩展函数
来源：http://hz.yj20258888.top/gtvbjopzgg.html

fun String.exclaim() = this + "!"
来源：http://hz.daria6918.cn/gtqdyugmwt.html

[T10] Kotlin：默认参数
来源：http://hz.yueranfly.top/gtblvhiqrr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yongpay.top/gtmpjhnvfn.html

[T11] Kotlin：协程
来源：http://hz.svipenyu.cn/gtgakvwlrl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gaohongyu789.top/gtdfhrlkqx.html

[T12] Kotlin：解构声明
来源：http://hz.meibo888.top/gtqwjvrrdu.html

val (a, b) = Pair(1, 2)
来源：http://hz.jlsjyb.cn/gtokxtbbfg.html

[T13] Kotlin：只读 Map
来源：http://hz.52xcode.cn/gtgnmerujs.html

val m = mapOf("a" to 1)
来源：http://hz.xziqi.cn/gttlgodpqa.html

[T14] Kotlin：循环
来源：http://hz.dashuyun.cn/gtigiisssd.html

for (i in 1..10) println(i)
来源：http://hz.redwolf501.top/gtirklpwsp.html

[T15] Kotlin：接口
来源：http://hz.sufxvd.cn/gtlgkimarj.html

interface Shape { fun area(): Double }
来源：http://hz.zhoulong.xyz/gtucbgpjbl.html

[T16] Swift：Hello World
来源：http://hz.tian-w.cn/gtclbvzkvx.html

print("Hello")
来源：http://hz.jinqigufen.top/gtdsehtvtv.html

[T17] Swift：变量与常量
来源：http://hz.shangyingyoupin.top/gtpfmjdktf.html

var a = 1;  let b = 2
来源：http://hz.sxryk.cn/gtclboeijo.html

[T18] Swift：字符串插值
来源：http://hz.xinyue.icu/gtztygghto.html

"值: \(b)"
来源：http://hz.smart0.xyz/gtyuoeddmd.html

[T19] Swift：可选绑定
来源：http://hz.sxryk.cn/gtqijnbcbr.html

if let n = opt { print(n) }
来源：http://hz.zhiwuduotai.top/gtjcukrwbs.html

[T20] Swift：数组操作
来源：http://hz.zdqjudy.top/gtfmrmxvrs.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.xinyue.icu/gtwrlwfhmz.html

[T21] Swift：遍历
来源：http://hz.zhiwuduotai.top/gtyworenvp.html

for x in a { print(x) }
来源：http://hz.chenlongwang.top/gtywtxwxtv.html

[T22] Swift：字典
来源：http://hz.ehwqpu.com/gtdkxnlpwo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnxiangtu.top/gtxlfbpmum.html

[T23] Swift：函数
来源：http://hz.jinyuanbaomall.cn/gtacaqlibi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nanxuanxn.top/gtbagzxycy.html

[T24] Swift：闭包
来源：http://hz.jinghuilouyu.cn/gtypabzmsv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shangyingyoupin.top/gtyaqlmyea.html

[T25] Swift：结构体
来源：http://hz.ivvv.top/gtoasgdvix.html

struct P { var x: Int }
来源：http://hz.cqqwz.cn/gtincdcqef.html

[T26] Swift：类与重写
来源：http://hz.chenzaomai.com/gtbnlyrnls.html

class A: Base { override func f() {} }
来源：http://hz.gaohongyu789.top/gtcxegoope.html

[T27] Swift：错误处理
来源：http://hz.yueranfly.top/gtvjjlowkk.html

do { try f() } catch { print(error) }
来源：http://hz.bjfxy.top/gtjocjuzdh.html

[T28] Swift：枚举
来源：http://hz.zhaomingkeji.xyz/gtvhwhmcew.html

enum Color { case red, green }
来源：http://hz.hammf.cn/gtercdtiom.html

[T29] Swift：guard 提前返回
来源：http://hz.gotoacloud.top/gticehrdkc.html

guard let x = opt else { return }
来源：http://hz.gzhubu.top/gtmkqumhpz.html

[T30] Swift：协议
来源：http://hz.iojbl.cn/gtskpjmtwi.html

protocol Shape { func area() -> Double }
来源：http://hz.gaohongyu789.top/gtfvfkzxii.html

[T31] Lua：Hello World
来源：http://hz.hammf.cn/gtnxyyvlwx.html

print("Hello")
来源：http://hz.zhongyouzk.top/gtrsmbsouj.html

[T32] Lua：局部变量
来源：http://hz.zhijiandao.cn/gtdhctqvyf.html

local a = 1
来源：http://hz.kuanghao11.cn/gtqagyxybs.html

[T33] Lua：表（数组）
来源：http://hz.jiagoushi.top/gtbqcpastd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ydjk.org.cn/gtjssvfqzy.html

[T34] Lua：遍历表
来源：http://hz.ydzc1.top/gtgsvdjozr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhaomingkeji.xyz/gtyemjiizt.html

[T35] Lua：字典表
来源：http://hz.pengpengdd.cyou/gtqhstnadh.html

local d = { a = 1 };  d.b = 2
来源：http://hz.fzhhl.top/gtdmngzuaf.html

[T36] Lua：函数
来源：http://hz.tanke756.top/gtxtbkqwcx.html

function add(a, b) return a + b end
来源：http://hz.shanyushiyangtech.top/gteluzizmm.html

[T37] Lua：字符串拼接
来源：http://hz.feifeiyinyue.top/gtbczsmpaf.html

"a" .. "b"
来源：http://hz.chenlongwang.top/gtykeagsby.html

[T38] Lua：条件
来源：http://hz.dashuyun.cn/gtukfitonk.html

if x > 0 then print("正") end
来源：http://hz.zdqjudy.top/gtedsspyiq.html

[T39] Lua：模式匹配
来源：http://hz.sufxvd.cn/gtygvdpctr.html

string.find(s, "%d+")
来源：http://hz.shzxlz.cn/gtdwdsoqcx.html

[T40] Lua：元表
来源：http://hz.shangyingyoupin.top/gtirydfzjv.html

setmetatable({}, { __index = base })
来源：http://hz.nanxinkj.top/gtrootncuc.html

[T41] Perl：Hello World
来源：http://hz.yj202588.top/gtryxxzzpu.html

print "Hello\n";
来源：http://hz.vqdsnc.cn/gtvabbfncr.html

[T42] Perl：变量类型
来源：http://hz.aibaodan.cn/gthglyreyi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zhoulong.xyz/gtfzuxseeu.html

[T43] Perl：字符串插值
来源：http://hz.haohaochexian.top/gtzoihwezi.html

"值: $a"
来源：http://hz.yuxming.cn/gtnqstogck.html

[T44] Perl：条件
来源：http://hz.zhoulong.xyz/gtkdtyyyjg.html

if ($a > 0) { print "正"; }
来源：http://hz.yueranfly.top/gtjpahbwoy.html

[T45] Perl：数组遍历
来源：http://hz.shuidangran.top/gtwirxfnqw.html

for my $x (@arr) { print $x; }
来源：http://hz.cucudq.cn/gtootaywma.html

[T46] Perl：哈希操作
来源：http://hz.cucudq.cn/gtgpexchzw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhaomingkeji.xyz/gtflsmsncv.html

[T47] Perl：正则捕获
来源：http://hz.quarkkingdee.top/gtcmnzofze.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.dashuyun.cn/gtjmiuixwl.html

[T48] Perl：正则替换
来源：http://hz.zhaomingkeji.xyz/gtvbzxhntl.html

$s =~ s/old/new/g;
来源：http://hz.zhoulong.xyz/gtmeccbscv.html

[T49] Perl：函数
来源：http://hz.jyoumei.cn/gtoyhjqcju.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.quarkkingdee.top/gtdtiihshn.html

[T50] Perl：逐行读文件
来源：http://hz.yuxming.cn/gtqympccaq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dashuyun.cn/gtbzokpxba.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.snrcjt.cn/gtgywrqrrt.html

[T51] Scala：Hello World
来源：http://hz.ywan-chungtsiang.top/gteqiyxlwm.html

println("Hello")
来源：http://hz.ybcxt.top/gtsqjvacve.html

[T52] Scala：变量
来源：http://hz.ydzc1.top/gtjylkuvuf.html

val a = 1;  var b = 2
来源：http://hz.sxryk.cn/gtumnzmhuk.html

[T53] Scala：字符串插值
来源：http://hz.dianchejie.cn/gtprclpazw.html

s"值: $b"
来源：http://hz.havefunace.top/gtawiikfyb.html

[T54] Scala：集合映射
来源：http://hz.quarkkingdee.top/gtlzcyrhud.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.cqqwz.cn/gtqtgpxgqt.html

[T55] Scala：集合过滤
来源：http://hz.havefunace.top/gtcvzwalpo.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dashuyun.cn/gtxvulolxt.html

[T56] Scala：样例类
来源：http://hz.ywan-chungtsiang.top/gtgayvdclp.html

case class User(name: String, age: Int)
来源：http://hz.yongpay.top/gtyoebfmnf.html

[T57] Scala：模式匹配
来源：http://hz.vqdsnc.cn/gthvlvkgqe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhijiandao.cn/gtazsdjkwf.html

[T58] Scala：函数定义
来源：http://hz.yongpay.top/gtufgirkgl.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.cqqwz.cn/gtwsqhfmlk.html

[T59] Scala：循环
来源：http://hz.gaohongyu789.top/gtkhoctrva.html

for (i <- 1 to 10) println(i)
来源：http://hz.xuetiantiany.cn/gtorzolakb.html

[T60] Scala：折叠
来源：http://hz.hysaishi.cn/gthywqxhcf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.fzhhl.top/gtwbvlpmul.html

================================================================================
来源：http://hz.bjfxy.top/gtbgnxcrjw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shangyingyoupin.top/gtnszkucqu.html

================================================================================
来源：http://hz.zhoulong.xyz/gtkahkfzpi.html

[U01] Py：创建虚拟环境
来源：http://hz.zhijiandao.cn/gtzuislhpv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.smart0.xyz/gtrotzhimb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.birdmap.top/gtntqoiyen.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenjidiqi.icu/gtyczxfxvq.html

[U03] Py：加载 .env 配置
来源：http://hz.smart0.xyz/gtvfgjppez.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jyoumei.cn/gtjpfupygj.html

[U04] Py：变量调试打印
来源：http://hz.yangfankeji.com/gthrpmnbea.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.jinqigfzy.top/gtprxizbbv.html

[U05] Py：列表去重且保序
来源：http://hz.nanxinkj.top/gtpdpbvcxw.html

list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtcfgkuwiq.html

[U06] Py：合并两个字典
来源：http://hz.xuetiantiany.cn/gtufuwnxwp.html

{**a, **b}
来源：http://hz.yj202588.top/gtqskjzufi.html

[U07] Py：反转字典键值
来源：http://hz.316326.xyz/gtvuwzqusx.html

{v: k for k, v in d.items()}
来源：http://hz.cashguo.top/gtuzgtpvek.html

[U08] Py：展平二维列表
来源：http://hz.fengsongda.top/gtfxfqfsud.html

[y for x in nested for y in x]
来源：http://hz.cashguo.top/gtrxznxehf.html

[U09] Py：字典取最大值的键
来源：http://hz.yonumen.top/gtysootlys.html

max(d, key=d.get)
来源：http://hz.zhongyouzk.top/gtofgxkxrj.html

[U10] Py：按值排序字典
来源：http://hz.sxryk.cn/gteuzkorfg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ybcxt.top/gtixgvbkbk.html

[U11] Py：生成器表达式
来源：http://hz.jlsjyb.cn/gtwvixkwyr.html

(x * 2 for x in arr)
来源：http://hz.zycfv.cn/gtxhydrfxk.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.smart0.xyz/gtxapvhgua.html

Counter(arr).most_common(3)
来源：http://hz.tanke756.top/gtdjrqynkz.html

[U13] Py：固定长度队列
来源：http://hz.yonumen.top/gtcmkxxazi.html

deque(maxlen=10)
来源：http://hz.yvedp.cn/gtimbawcpm.html

[U14] Py：分组收集到列表
来源：http://hz.yangfankeji.com/gtamlqyttn.html

defaultdict(list)
来源：http://hz.ppjwa.cn/gtbxkohlba.html

[U15] Py：高精度计时
来源：http://hz.tanke756.top/gtrywsxbjl.html

t = time.perf_counter()
来源：http://hz.sweek.top/gtlbdynrgz.html

[U16] Py：命令行参数解析
来源：http://hz.xuanzx.com/gtkidijdpa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.aizwys.cn/gtbdtbhteo.html

[U17] Py：初始化日志
来源：http://hz.wangshuangyany.cn/gtpxstazcj.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.havefunace.top/gtsfnpwvjz.html

[U18] Py：预编译正则
来源：http://hz.jiagoushi.top/gtsdyfzhgt.html

pat = re.compile(r"\d+")
来源：http://hz.hfpthk.cn/gtzaqwwtiy.html

[U19] Py：正则替换带回调
来源：http://hz.chenlongwang.top/gtgeluttui.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.fzhhl.top/gtzkkvkbly.html

[U20] Py：缓存函数结果
来源：http://hz.pengpengdd.cyou/gtjwzjphpq.html

@functools.lru_cache(maxsize=None)
来源：http://hz.birdmap.top/gtcfjqpsxs.html

[U21] Py：自定义上下文管理器
来源：http://hz.sufxvd.cn/gtrgsovbuv.html

@contextlib.contextmanager
来源：http://hz.fengsongda.top/gtobsbyinr.html

[U22] Py：矩阵转置
来源：http://hz.ybcxt.top/gtlbntmyxs.html

list(zip(*m))
来源：http://hz.hfpthk.cn/gtuknolpio.html

[U23] Py：分块读取大文件
来源：http://hz.jlsjyb.cn/gtjghsssic.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.daxiang520.top/gthqwjpowx.html

[U24] Py：路径操作
来源：http://hz.aizwys.cn/gtlmqljlqs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jqgfzy.top/gtxlfdxcrw.html

[U25] Py：CSV 按字典读
来源：http://hz.jinqigfzy.top/gtefolxioq.html

csv.DictReader(f)
来源：http://hz.wangdashe.top/gttxtwohzx.html

[U26] Py：并发下载
来源：http://hz.ydjk.org.cn/gtrolqpoga.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jqgufenzy.top/gthbafbwag.html

[U27] Py：异步 HTTP
来源：http://hz.ivvv.top/gtzzelbzzk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.dashuyun.cn/gteximhhqk.html

[U28] Py：类型别名
来源：http://hz.tanke756.top/gtyxlgwels.html

UserId = int
来源：http://hz.iojbl.cn/gtsztnrrae.html

[U29] Py：属性校验
来源：http://hz.daria6918.cn/gtsnyhtgcy.html

@property 与 @x.setter 配合
来源：http://hz.wangdashe.top/gtrhyspcnv.html

[U30] Py：数据类
来源：http://hz.jqgfzy.top/gtlfzqliuu.html

@dataclass(slots=True)
来源：http://hz.hnqzz.top/gtqdraotwm.html

[U31] Py：单测
来源：http://hz.dianchejie.cn/gthjzkpfgh.html

python -m pytest -q
来源：http://hz.pengpengdd.cyou/gtraploruv.html

[U32] Py：代码格式化
来源：http://hz.daria6918.cn/gtugwfihdu.html

ruff format . && ruff check --fix .
来源：http://hz.hongshengwenyu.top/gtvqybaikv.html

[U33] Py：打包发布
来源：http://hz.zycfv.cn/gtqxviusxx.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhixingplan.top/gtsyggkgji.html

[U34] Py：判断编码
来源：http://hz.hysaishi.cn/gtbgfdjvzl.html

chardet.detect(raw)
来源：http://hz.cashguo.top/gtwcmzotjd.html

[U35] Py：发送邮件
来源：http://hz.zhijiandao.cn/gtxsxiantz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xziqi.cn/gtauvcxqme.html

[U36] Py：定时任务
来源：http://hz.xziqi.cn/gttpidesnu.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhaomingkeji.xyz/gtsjbqkpjn.html

[U37] Py：读写 Excel
来源：http://hz.chenjidiqi.icu/gtkwjycagy.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.nanxuanxn.top/gtcgbieizt.html

[U38] Py：获取脚本所在目录
来源：http://hz.chenlongwang.top/gtxtntemaj.html

Path(__file__).resolve().parent
来源：http://hz.jqgufenzy.top/gtpsnlptqd.html

[U39] Py：判断是否在交互环境
来源：http://hz.jqgufenzy.top/gtukckmapl.html

sys.stdout.isatty()
来源：http://hz.jlsjyb.cn/gtipfwevlw.html

[U40] Py：打印到标准错误
来源：http://hz.aibaodan.cn/gtgcgnezkl.html

print("err", file=sys.stderr)
来源：http://hz.ehwqpu.com/gtiadpxotw.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ydjk.org.cn/gthznobuzx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yonumen.top/gtowkeubda.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xuanzx.com/gtolqpcojo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hammf.cn/gtbveetovs.html

[U43] PHP：声明命名空间
来源：http://hz.chenjidiqi.icu/gtpkpxmqpj.html

namespace App\Http;
来源：http://hz.jqgufenzy.top/gtbelioump.html

[U44] PHP：开启严格类型
来源：http://hz.xuetiantiany.cn/gtbufchovb.html

declare(strict_types=1);
来源：http://hz.hywenlv.cn/gtnkupxcfz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.daxiang520.top/gthnpcmets.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtnjsnfktd.html

[U46] PHP：可空类型
来源：http://hz.hammf.cn/gtxqpchtxq.html

?string $name = null
来源：http://hz.shuidangran.top/gthyadtibi.html

[U47] PHP：联合类型
来源：http://hz.xuanzx.com/gtwxzqvoof.html

int|string $id
来源：http://hz.yj20258.top/gtmpklmksr.html

[U48] PHP：纯枚举
来源：http://hz.yueranfly.top/gtcrfvjwbw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.shanyushiyangkeji.top/gtwjnzkbry.html

[U49] PHP：只读属性
来源：http://hz.yanxiufei.cn/gtpnwnikdf.html

public readonly string $name
来源：http://hz.jiagoushi.top/gtuxrnlssm.html

[U50] PHP：构造器属性提升
来源：http://hz.mhx1999.top/gtuqmhjegr.html

public function __construct(private int $id) {}
来源：http://hz.52xcode.cn/gtytmvjaqq.html

[U51] PHP：数组解构
来源：http://hz.yj20258888.top/gtbpevueda.html

[$a, $b] = $arr;
来源：http://hz.jqgfzy.top/gtdevpyzqj.html

[U52] PHP：箭头函数
来源：http://hz.gaohongyu789.top/gtfjtmwhhq.html

$double = fn($x) => $x * 2;
来源：http://hz.aizwys.cn/gtpyxxwgfu.html

[U53] PHP：空合并运算符
来源：http://hz.hfpthk.cn/gtxezggkrq.html

$v = $a ?? $b ?? "default";
来源：http://hz.kuanghao11.cn/gtkvsmljfl.html

[U54] PHP：空安全调用
来源：http://hz.xuetiantiany.cn/gtobdobkib.html

$obj?->method()
来源：http://hz.ydzc1.top/gtutyshuok.html


<!-- 参考信息 -->