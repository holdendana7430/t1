代发 wailian999

memset(a, 0, sizeof a);
来源：http://hz.snrcjt.cn/gttqqttjeu.html

[S27] C：定义常量
来源：http://hz.jinqigfzy.top/gtgfyfnttm.html

const double PI = 3.14159;
来源：http://hz.hywenlv.cn/gtcgmydlot.html

[S28] C：静态变量
来源：http://hz.gotoacloud.top/gttivteqfl.html

static int counter = 0;
来源：http://hz.yueranfly.top/gtzcrfuofv.html

[S29] C：变参函数
来源：http://hz.fengsongda.top/gtmrunelac.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj202588.top/gtljjeqtzt.html

[S30] C：头文件保护
来源：http://hz.yj20258.top/gtygzhnppj.html

#ifndef X_H
来源：http://hz.birdmap.top/gtowbajqiq.html

#define X_H
来源：http://hz.aizwys.cn/gtfzdfboiy.html

#endif
来源：http://hz.shanyushiyangkeji.top/gtvtgpsvkn.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtsyobhbbt.html

#include <iostream>
来源：http://hz.hnqzz.top/gtseexbtil.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.feifeiyinyue.top/gtsersjndg.html

[S32] C++：字符串
来源：http://hz.zhaomingkeji.xyz/gtcxmtzimn.html

std::string s = "hi";  s += "!";
来源：http://hz.wangdashe.top/gtgiydlqkg.html

[S33] C++：vector 增删
来源：http://hz.ydjk.org.cn/gtcslxcflv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxinkj.top/gtbscudjia.html

[S34] C++：遍历 vector
来源：http://hz.shangyingyoupin.top/gtzxckhhan.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangdashe.top/gtcdrcnkio.html

[S35] C++：map
来源：http://hz.jlsjyb.cn/gtdnkhcowg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtvzruzunc.html

[S36] C++：unordered_map
来源：http://hz.ivvv.top/gtyacmfzza.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tanke756.top/gtadmziony.html

[S37] C++：set
来源：http://hz.0kj1m.cn/gtevgymdhg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xziqi.cn/gtllymnxev.html

[S38] C++：排序
来源：http://hz.ehwqpu.com/gtkufaxule.html

std::sort(v.begin(), v.end());
来源：http://hz.yuanzhike.top/gteslrhzlp.html

[S39] C++：自定义比较器排序
来源：http://hz.aibaodan.cn/gtdnkylgfg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.svipenyu.cn/gttkzblfff.html

[S40] C++：查找元素
来源：http://hz.shzxlz.cn/gtjtibligx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.snrcjt.cn/gtbukjppua.html

[S41] C++：类与构造函数
来源：http://hz.ydzc1.top/gtrmnhnedf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinqigfzy.top/gtksyuulen.html

[S42] C++：继承与虚函数
来源：http://hz.0kj1m.cn/gtspzeigqo.html

class B : public Base { public: void f() override {} };
来源：http://hz.ehwqpu.com/gthvixiuag.html

[S43] C++：智能指针
来源：http://hz.ivvv.top/gtcgrswspx.html

auto p = std::make_unique<int>(5);
来源：http://hz.ehwqpu.com/gtbolpomqy.html

[S44] C++：引用传参
来源：http://hz.316326.xyz/gthzutkyrb.html

void inc(int &x) { ++x; }
来源：http://hz.xziqi.cn/gtllhqrvux.html

[S45] C++：lambda
来源：http://hz.0kj1m.cn/gtcblxiplx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xinyue.icu/gtqbuxheqv.html

[S46] C++：函数模板
来源：http://hz.gogol.net.cn/gtjwexloyj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sweek.top/gtgihanzrf.html

[S47] C++：结构化绑定遍历
来源：http://hz.shuidangran.top/gtaukwlcte.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.haohaochexian.top/gtlqlesfrj.html

[S48] C++：逐行读文件
来源：http://hz.tianlin.xyz/gtmlqmqjdj.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.iojbl.cn/gtykhnwtes.html

while (std::getline(in, line)) { }
来源：http://hz.zhongyouzk.top/gtxwqmvbyi.html

[S49] C++：写文件
来源：http://hz.zhiwuduotai.top/gtcmxnyfmk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sxryk.cn/gtekxujkqj.html

[S50] C++：格式化数字
来源：http://hz.shuidangran.top/gtnpoplynt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.feifeiyinyue.top/gtiikscuee.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtqrjvrplk.html

static_cast<double>(a) / b
来源：http://hz.ehwqpu.com/gtvjvxklxs.html

[S52] C++：const 与 noexcept
来源：http://hz.hammf.cn/gthsznngzc.html

int size() const noexcept { return n_; }
来源：http://hz.tian-w.cn/gtwpwpzmpm.html

[S53] C++：移动语义
来源：http://hz.birdmap.top/gtkmemyuxv.html

std::vector<int> w = std::move(v);
来源：http://hz.feifeiyinyue.top/gtfnrfrwnc.html

[S54] C++：异常处理
来源：http://hz.dianchejie.cn/gtgtcrxcjr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hysaishi.cn/gtnaiowruc.html

[S55] C++：结构化绑定
来源：http://hz.aizwys.cn/gtkqqleyyj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.havefunace.top/gttcubjupm.html

[S56] C++：optional
来源：http://hz.xylfe.cn/gtfjubtpms.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jyoumei.cn/gtgtpfyuht.html

[S57] C++：编译期常量
来源：http://hz.zdqjudy.top/gtuocvfmdr.html

constexpr int N = 10;
来源：http://hz.ybcxt.top/gtkeynpdkf.html

[S58] C++：命名空间
来源：http://hz.xinyue.icu/gtjrvpnqzo.html

namespace ns { int f() { return 1; } }
来源：http://hz.nwbrower.top/gtfktvmuyu.html

[S59] C++：静态断言
来源：http://hz.zdqjudy.top/gtjiwcdmwe.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.birdmap.top/gtomeamehb.html

[S60] C++：遍历并删除元素
来源：http://hz.zycfv.cn/gtmhkjavie.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tian-w.cn/gthzrwkpwz.html

================================================================================
来源：http://hz.ybcxt.top/gtujkuctby.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenzaomai.com/gtdkkawfww.html

================================================================================
来源：http://hz.xuanzx.com/gtokneyzoa.html

[T01] Kotlin：Hello World
来源：http://hz.hongshengwenyu.top/gtpgramcys.html

println("Hello")
来源：http://hz.yonumen.top/gtllzfgcgg.html

[T02] Kotlin：变量
来源：http://hz.snrcjt.cn/gtduvlmreu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aibaodan.cn/gtclsxzlgj.html

[T03] Kotlin：字符串模板
来源：http://hz.jqgufenzy.top/gtflawiply.html

"值: $b"
来源：http://hz.ywan-chungtsiang.top/gtngigistt.html

[T04] Kotlin：空安全
来源：http://hz.yanxiufei.cn/gtqaytuftk.html

val n: String? = null;  n?.length
来源：http://hz.ybcxt.top/gtwgdhtzdv.html

[T05] Kotlin：when 表达式
来源：http://hz.cashguo.top/gtdjuzokof.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gogol.net.cn/gtdghshsth.html

[T06] Kotlin：集合映射
来源：http://hz.meibo888.top/gtqnfquefm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cqqwz.cn/gtvbkpeylv.html

[T07] Kotlin：集合过滤
来源：http://hz.guowangkeji.top/gtxfqzzedf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xziqi.cn/gtmemyilcf.html

[T08] Kotlin：数据类
来源：http://hz.wangdashe.top/gtosqrkxws.html

data class User(val name: String, val age: Int)
来源：http://hz.cheryme.top/gtghpjaozz.html

[T09] Kotlin：扩展函数
来源：http://hz.yuanzhike.top/gtddogbayl.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgufenzy.top/gtvfbdsshz.html

[T10] Kotlin：默认参数
来源：http://hz.9152youxi.cn/gtytlkvyuh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinyuanbaomall.cn/gtapckotte.html

[T11] Kotlin：协程
来源：http://hz.chenzaomai.com/gtjqvwnvqt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinghuilouyu.cn/gtgkwvusmd.html

[T12] Kotlin：解构声明
来源：http://hz.hongshengwenyu.top/gttxefpdsc.html

val (a, b) = Pair(1, 2)
来源：http://hz.jyoumei.cn/gttaovqmjy.html

[T13] Kotlin：只读 Map
来源：http://hz.birdmap.top/gttlevohyr.html

val m = mapOf("a" to 1)
来源：http://hz.yueranfly.top/gtbufiyeel.html

[T14] Kotlin：循环
来源：http://hz.fzhhl.top/gtkkmrczil.html

for (i in 1..10) println(i)
来源：http://hz.zhiwuduotai.top/gtgftfkzvg.html

[T15] Kotlin：接口
来源：http://hz.cucudq.cn/gtaijgflbz.html

interface Shape { fun area(): Double }
来源：http://hz.feifeiyinyue.top/gtdrynthcn.html

[T16] Swift：Hello World
来源：http://hz.tian-w.cn/gtajfbuwuq.html

print("Hello")
来源：http://hz.gotoacloud.top/gtgrtsymlh.html

[T17] Swift：变量与常量
来源：http://hz.zhoulong.xyz/gtgygrpjhk.html

var a = 1;  let b = 2
来源：http://hz.0kj1m.cn/gtiqlmjrxo.html

[T18] Swift：字符串插值
来源：http://hz.jyoumei.cn/gtlizlrknf.html

"值: \(b)"
来源：http://hz.vqdsnc.cn/gtddlmtkhu.html

[T19] Swift：可选绑定
来源：http://hz.andypj.xyz/gtvltftsii.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gthpvpflbn.html

[T20] Swift：数组操作
来源：http://hz.jiagoushi.top/gthoaklmof.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yuanzhike.top/gtyahyhayp.html

[T21] Swift：遍历
来源：http://hz.haohaochexian.top/gtqbtdoqol.html

for x in a { print(x) }
来源：http://hz.havefunace.top/gthbsamaqa.html

[T22] Swift：字典
来源：http://hz.zhijiandao.cn/gtgoeorhbw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenzaomai.com/gtnfmvkvpi.html

[T23] Swift：函数
来源：http://hz.sxryk.cn/gtdyahratx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jqgfzy.top/gtmiulgfxy.html

[T24] Swift：闭包
来源：http://hz.cucudq.cn/gtnjxfggdy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zdqjudy.top/gtulilmhag.html

[T25] Swift：结构体
来源：http://hz.chenjidiqi.icu/gtgspreukx.html

struct P { var x: Int }
来源：http://hz.quarkkingdee.top/gtvgbmbsrt.html

[T26] Swift：类与重写
来源：http://hz.birdmap.top/gtgicmdtgw.html

class A: Base { override func f() {} }
来源：http://hz.yanxiufei.cn/gtufsznrni.html

[T27] Swift：错误处理
来源：http://hz.jinghuilouyu.cn/gteuaymojv.html

do { try f() } catch { print(error) }
来源：http://hz.cheryme.top/gtkkmripyl.html

[T28] Swift：枚举
来源：http://hz.chenjidiqi.icu/gtkeihdaqk.html

enum Color { case red, green }
来源：http://hz.andypj.xyz/gtpmsuukrb.html

[T29] Swift：guard 提前返回
来源：http://hz.sysykeji.top/gtextrrein.html

guard let x = opt else { return }
来源：http://hz.jianghu66.top/gtnasjqotx.html

[T30] Swift：协议
来源：http://hz.cheryme.top/gtfgwomqxr.html

protocol Shape { func area() -> Double }
来源：http://hz.shanyushiyangtech.top/gtmfuhchww.html

[T31] Lua：Hello World
来源：http://hz.c1oappe.top/gttnwnqhwy.html

print("Hello")
来源：http://hz.dianchejie.cn/gtutewbbhg.html

[T32] Lua：局部变量
来源：http://hz.zhoulong.xyz/gtwzyagpum.html

local a = 1
来源：http://hz.birdmap.top/gtimqrkkfe.html

[T33] Lua：表（数组）
来源：http://hz.hfpthk.cn/gtkajcupuy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.snrcjt.cn/gtzorlloit.html

[T34] Lua：遍历表
来源：http://hz.xziqi.cn/gtdyemzvcp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.meibo888.top/gtiwbkcemq.html

[T35] Lua：字典表
来源：http://hz.zhengqikj.top/gtjtdanafy.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yangfankeji.com/gtbmkqgrsl.html

[T36] Lua：函数
来源：http://hz.gaohongyu789.top/gtxsmjfxwk.html

function add(a, b) return a + b end
来源：http://hz.gzhubu.top/gtthtmkfni.html

[T37] Lua：字符串拼接
来源：http://hz.wangdashe.top/gtdkafcbox.html

"a" .. "b"
来源：http://hz.gaohongyu789.top/gtwsrsapzv.html

[T38] Lua：条件
来源：http://hz.hongshengwenyu.top/gtqtftvmoh.html

if x > 0 then print("正") end
来源：http://hz.yuanzhike.top/gthcjrlxyn.html

[T39] Lua：模式匹配
来源：http://hz.ehwqpu.com/gttfugyqtc.html

string.find(s, "%d+")
来源：http://hz.svipenyu.cn/gtpdkxmxos.html

[T40] Lua：元表
来源：http://hz.xinyue.icu/gtggsmitkg.html

setmetatable({}, { __index = base })
来源：http://hz.pengpengdd.cyou/gtlqlszcar.html

[T41] Perl：Hello World
来源：http://hz.shuidangran.top/gtdbisboiv.html

print "Hello\n";
来源：http://hz.jqgufenzy.top/gtldiunllm.html

[T42] Perl：变量类型
来源：http://hz.chenjidiqi.icu/gtgkqzpdfy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gotoacloud.top/gtjfywpjdh.html

[T43] Perl：字符串插值
来源：http://hz.fengsongda.top/gtdbjkkmcs.html

"值: $a"
来源：http://hz.cqqwz.cn/gtxcamzgwb.html

[T44] Perl：条件
来源：http://hz.wangdashe.top/gtmyytumdm.html

if ($a > 0) { print "正"; }
来源：http://hz.kuanghao11.cn/gtsulmklrk.html

[T45] Perl：数组遍历
来源：http://hz.vqdsnc.cn/gtutwpaqzk.html

for my $x (@arr) { print $x; }
来源：http://hz.yongpay.top/gtyiyvdgwf.html

[T46] Perl：哈希操作
来源：http://hz.yanxiufei.cn/gtufejqjhw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhoulong.xyz/gtgxrbrqel.html

[T47] Perl：正则捕获
来源：http://hz.yj202588.top/gtdtoihddl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.snrcjt.cn/gtalktggdg.html

[T48] Perl：正则替换
来源：http://hz.havefunace.top/gttcpsnjob.html

$s =~ s/old/new/g;
来源：http://hz.tian-w.cn/gtstogchye.html

[T49] Perl：函数
来源：http://hz.ywan-chungtsiang.top/gtahgyaimr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhijiandao.cn/gthhtobcjt.html

[T50] Perl：逐行读文件
来源：http://hz.yonumen.top/gtqurglbcs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ydjk.org.cn/gtjsccnkvs.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.bjfxy.top/gtwhgwtkbi.html

[T51] Scala：Hello World
来源：http://hz.jqgufenzy.top/gteymncpjf.html

println("Hello")
来源：http://hz.nwbrower.top/gtrcbaxoku.html

[T52] Scala：变量
来源：http://hz.yongpay.top/gtjaxenvtq.html

val a = 1;  var b = 2
来源：http://hz.fengsongda.top/gtxxikpwvc.html

[T53] Scala：字符串插值
来源：http://hz.nwbrower.top/gtvmnrubgi.html

s"值: $b"
来源：http://hz.shzxlz.cn/gtelsgiztb.html

[T54] Scala：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtmxqsavpv.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.meibo888.top/gtcxapubop.html

[T55] Scala：集合过滤
来源：http://hz.xylfe.cn/gtrzwcdayo.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj202588.top/gtugsoxydf.html

[T56] Scala：样例类
来源：http://hz.tianlin.xyz/gtxoffwduo.html

case class User(name: String, age: Int)
来源：http://hz.havefunace.top/gtrtqjednp.html

[T57] Scala：模式匹配
来源：http://hz.nwbrower.top/gtltpoptkz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.fengsongda.top/gtocakcohz.html

[T58] Scala：函数定义
来源：http://hz.ydjk.org.cn/gtrdavppjv.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.hnqzz.top/gtrfchofof.html

[T59] Scala：循环
来源：http://hz.vqdsnc.cn/gtyjdeuvkc.html

for (i <- 1 to 10) println(i)
来源：http://hz.ybcxt.top/gtzxehtmrt.html

[T60] Scala：折叠
来源：http://hz.tanke756.top/gtdlrmyptf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jlsjyb.cn/gtsiofqfcx.html

================================================================================
来源：http://hz.birdmap.top/gtlcydvicj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.shuidangran.top/gtszjruytt.html

================================================================================
来源：http://hz.zycfv.cn/gtiwqspfgt.html

[U01] Py：创建虚拟环境
来源：http://hz.jinghuilouyu.cn/gtauvxrwqu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.meibo888.top/gtbawecffc.html

[U02] Py：导出 / 安装依赖
来源：http://hz.yongpay.top/gtdqwtdrpa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cheryme.top/gtzkrumtsf.html

[U03] Py：加载 .env 配置
来源：http://hz.ywan-chungtsiang.top/gtitmxbeow.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.dashuyun.cn/gtqwzpdovm.html

[U04] Py：变量调试打印
来源：http://hz.0kj1m.cn/gtggwqiooj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gotoacloud.top/gtpnmdawoj.html

[U05] Py：列表去重且保序
来源：http://hz.ivvv.top/gtqznhkaqj.html

list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtorbfxunb.html

[U06] Py：合并两个字典
来源：http://hz.hysaishi.cn/gtekhcbjpl.html

{**a, **b}
来源：http://hz.9152youxi.cn/gtletqffhw.html

[U07] Py：反转字典键值
来源：http://hz.yvedp.cn/gtcdfkyjpv.html

{v: k for k, v in d.items()}
来源：http://hz.zhiwuduotai.top/gtjldqdecx.html

[U08] Py：展平二维列表
来源：http://hz.yanxiufei.cn/gttyxvmzgr.html

[y for x in nested for y in x]
来源：http://hz.svipenyu.cn/gtnpukepjd.html

[U09] Py：字典取最大值的键
来源：http://hz.yvedp.cn/gtyvxwntki.html

max(d, key=d.get)
来源：http://hz.yuxming.cn/gtjpthijrx.html

[U10] Py：按值排序字典
来源：http://hz.havefunace.top/gtyjquqmke.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.sxryk.cn/gtdnhnwzsw.html

[U11] Py：生成器表达式
来源：http://hz.xuetiantiany.cn/gtcncsukma.html

(x * 2 for x in arr)
来源：http://hz.hnqzz.top/gtnjpyioev.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ybcxt.top/gtynzqfmqo.html

Counter(arr).most_common(3)
来源：http://hz.zhoulong.xyz/gtotronlcw.html

[U13] Py：固定长度队列
来源：http://hz.svipenyu.cn/gtbxzkqatp.html

deque(maxlen=10)
来源：http://hz.xylfe.cn/gtuoxigbln.html

[U14] Py：分组收集到列表
来源：http://hz.jqgfzy.top/gtjujvopmd.html

defaultdict(list)
来源：http://hz.wangshuangyany.cn/gttewbyxvt.html

[U15] Py：高精度计时
来源：http://hz.zhaomingkeji.xyz/gtpyvbwmac.html

t = time.perf_counter()
来源：http://hz.pycfn.com/gtqzezrmoi.html

[U16] Py：命令行参数解析
来源：http://hz.9152youxi.cn/gtebvwpmuz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yj20258.top/gtanjmdtjy.html

[U17] Py：初始化日志
来源：http://hz.zhaomingkeji.xyz/gtsejyvpjq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fengsongda.top/gtwevxlmgn.html

[U18] Py：预编译正则
来源：http://hz.fzhhl.top/gttckskdwx.html

pat = re.compile(r"\d+")
来源：http://hz.jiagoushi.top/gtzbgndvwl.html

[U19] Py：正则替换带回调
来源：http://hz.hfpthk.cn/gtfiwvwsuc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zdqjudy.top/gtlkobvlax.html

[U20] Py：缓存函数结果
来源：http://hz.cucudq.cn/gtigaauort.html

@functools.lru_cache(maxsize=None)
来源：http://hz.0kj1m.cn/gtwpidfzuu.html

[U21] Py：自定义上下文管理器
来源：http://hz.zhaomingkeji.xyz/gtytdtbyyu.html

@contextlib.contextmanager
来源：http://hz.xingfuxueyuan.xyz/gtpqnsnjan.html

[U22] Py：矩阵转置
来源：http://hz.jinghuilouyu.cn/gtbqgrqdpv.html

list(zip(*m))
来源：http://hz.ydzc1.top/gtwakjxisn.html

[U23] Py：分块读取大文件
来源：http://hz.zhoulong.xyz/gtpyxcmjfr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.iojbl.cn/gtmvgsnvzr.html

[U24] Py：路径操作
来源：http://hz.birdmap.top/gtueyldhom.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hnqzz.top/gtrsrksigx.html

[U25] Py：CSV 按字典读
来源：http://hz.dashuyun.cn/gtinwkksoo.html

csv.DictReader(f)
来源：http://hz.zhaomingkeji.xyz/gtnwksbtqu.html

[U26] Py：并发下载
来源：http://hz.sxryk.cn/gtwmslwjbr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sysykeji.top/gtnomjoqwo.html

[U27] Py：异步 HTTP
来源：http://hz.zhixingplan.top/gtvkxtsvbk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhongyouzk.top/gtufhryghm.html

[U28] Py：类型别名
来源：http://hz.chenzaomai.com/gtrlwkiehp.html

UserId = int
来源：http://hz.jqgfzy.top/gtvrwlprpk.html

[U29] Py：属性校验
来源：http://hz.tian-w.cn/gtqtnfqmuf.html

@property 与 @x.setter 配合
来源：http://hz.gotoacloud.top/gtoauhpguu.html

[U30] Py：数据类
来源：http://hz.chenlongwang.top/gtuurtdnbh.html

@dataclass(slots=True)
来源：http://hz.c1oappe.top/gtzlyhhlth.html

[U31] Py：单测
来源：http://hz.zhaomingkeji.xyz/gtinpaxhmg.html

python -m pytest -q
来源：http://hz.tanke756.top/gtlbjbndno.html

[U32] Py：代码格式化
来源：http://hz.zhiwuduotai.top/gtrkhodgzy.html

ruff format . && ruff check --fix .
来源：http://hz.gogol.net.cn/gtapsovrdk.html

[U33] Py：打包发布
来源：http://hz.zhoulong.xyz/gtbfdbcqje.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.dianchejie.cn/gtyeunpggb.html

[U34] Py：判断编码
来源：http://hz.iojbl.cn/gtftfjrwra.html

chardet.detect(raw)
来源：http://hz.feifeiyinyue.top/gtlmuifqfq.html

[U35] Py：发送邮件
来源：http://hz.xuanzx.com/gtbmhbjttc.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jiagoushi.top/gtzrwygekn.html

[U36] Py：定时任务
来源：http://hz.52xcode.cn/gtbofytnxe.html

schedule.every(10).minutes.do(job)
来源：http://hz.xingfuxueyuan.xyz/gtztkntuny.html

[U37] Py：读写 Excel
来源：http://hz.mhx1999.top/gtrgqwjiho.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.hywenlv.cn/gtmnmmxzgo.html

[U38] Py：获取脚本所在目录
来源：http://hz.52xcode.cn/gtptkkfdih.html

Path(__file__).resolve().parent
来源：http://hz.0kj1m.cn/gthxbuhqbg.html

[U39] Py：判断是否在交互环境
来源：http://hz.feifeiyinyue.top/gtohwwgylo.html

sys.stdout.isatty()
来源：http://hz.sxryk.cn/gtluldiryl.html

[U40] Py：打印到标准错误
来源：http://hz.sufxvd.cn/gtzxcaooll.html

print("err", file=sys.stderr)
来源：http://hz.guannengcc.top/gtgglpfyyj.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.daria6918.cn/gtocnkbbmh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xuanzx.com/gtknujszef.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jinqigufen.top/gtiztcreyr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jqgfzy.top/gttdqshrep.html

[U43] PHP：声明命名空间
来源：http://hz.ivvv.top/gtqamfcrvi.html

namespace App\Http;
来源：http://hz.xuetiantiany.cn/gtcupdxuro.html

[U44] PHP：开启严格类型
来源：http://hz.hnxiangtu.top/gtdisnwelc.html

declare(strict_types=1);
来源：http://hz.fengsongda.top/gtelyjzqqi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.guowangkeji.top/gtdqrgrdmi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtyecohpou.html

[U46] PHP：可空类型
来源：http://hz.hysaishi.cn/gtawgriuxr.html

?string $name = null
来源：http://hz.sxryk.cn/gtpjadttqb.html

[U47] PHP：联合类型
来源：http://hz.feifeiyinyue.top/gtiilcxaut.html

int|string $id
来源：http://hz.jianghu66.top/gtiitiwtow.html

[U48] PHP：纯枚举
来源：http://hz.daxiang520.top/gtqwdptzsa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.aizwys.cn/gthwesbjgp.html

[U49] PHP：只读属性
来源：http://hz.zhoulong.xyz/gtecxhrfws.html

public readonly string $name
来源：http://hz.hnxiangtu.top/gtqglonbdd.html

[U50] PHP：构造器属性提升
来源：http://hz.hfpthk.cn/gtomlbhjbs.html

public function __construct(private int $id) {}
来源：http://hz.c1oappe.top/gtobzvhosd.html


<!-- 参考信息 -->