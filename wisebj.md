代发 wailian999

static int counter = 0;
来源：http://hz.xuanzx.com/gtyfpjumia.html

[S29] C：变参函数
来源：http://hz.jinqigfzy.top/gtuccfizpu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangtech.top/gtryrmxpij.html

[S30] C：头文件保护
来源：http://hz.daxiang520.top/gtlmwgxjwm.html

#ifndef X_H
来源：http://hz.ppjwa.cn/gtlciavmmg.html

#define X_H
来源：http://hz.xuanzx.com/gtothdvycc.html

#endif
来源：http://hz.ehwqpu.com/gtdzpowajg.html

[S31] C++：Hello World
来源：http://hz.mhx1999.top/gtrxkodzqc.html

#include <iostream>
来源：http://hz.c1oappe.top/gtmljshyhm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.pengpengdd.cyou/gtvaogungl.html

[S32] C++：字符串
来源：http://hz.hammf.cn/gtsgacxmwq.html

std::string s = "hi";  s += "!";
来源：http://hz.haohaochexian.top/gtbmqsqdgn.html

[S33] C++：vector 增删
来源：http://hz.gzhubu.top/gtfqklwuri.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ybcxt.top/gtyosvrgwv.html

[S34] C++：遍历 vector
来源：http://hz.sxryk.cn/gtnlokcqge.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinqigfzy.top/gtiwckggxx.html

[S35] C++：map
来源：http://hz.cqqwz.cn/gtvxsqaqfl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtsynmnfuy.html

[S36] C++：unordered_map
来源：http://hz.jqgfzy.top/gtbkltxclu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtaqbfepuu.html

[S37] C++：set
来源：http://hz.andypj.xyz/gtvljlvuep.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sweek.top/gtztvygceq.html

[S38] C++：排序
来源：http://hz.ehwqpu.com/gtkddvpcar.html

std::sort(v.begin(), v.end());
来源：http://hz.dashuyun.cn/gtukjxrmij.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgufenzy.top/gttbmtgsdn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jianghu66.top/gtctamrlxn.html

[S40] C++：查找元素
来源：http://hz.yuxming.cn/gtricjifbe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shanyushiyangtech.top/gtvcwjabva.html

[S41] C++：类与构造函数
来源：http://hz.vqdsnc.cn/gtyepinsho.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.vqdsnc.cn/gtdinnwjbq.html

[S42] C++：继承与虚函数
来源：http://hz.tianlin.xyz/gtuferlvae.html

class B : public Base { public: void f() override {} };
来源：http://hz.c1oappe.top/gtifqirbli.html

[S43] C++：智能指针
来源：http://hz.jqgfzy.top/gtmoicrduh.html

auto p = std::make_unique<int>(5);
来源：http://hz.9152youxi.cn/gtojozvxob.html

[S44] C++：引用传参
来源：http://hz.guowangkeji.top/gtrxydgshp.html

void inc(int &x) { ++x; }
来源：http://hz.yvedp.cn/gtwyyascij.html

[S45] C++：lambda
来源：http://hz.snrcjt.cn/gtexiqofyu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tianlin.xyz/gtcmdmdmsz.html

[S46] C++：函数模板
来源：http://hz.jiagoushi.top/gtvmrxyhwq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gaohongyu789.top/gtopdtcfdc.html

[S47] C++：结构化绑定遍历
来源：http://hz.zdqjudy.top/gtkzdrlgmv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.gaohongyu789.top/gtgidpxpsi.html

[S48] C++：逐行读文件
来源：http://hz.birdmap.top/gtzpmakzrd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj202588.top/gtnxcuswcz.html

while (std::getline(in, line)) { }
来源：http://hz.xuanzx.com/gtawpztwnd.html

[S49] C++：写文件
来源：http://hz.xziqi.cn/gtdrjvyddy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.52xcode.cn/gtqnaaesuu.html

[S50] C++：格式化数字
来源：http://hz.shuidangran.top/gtgdxjtsat.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.aizwys.cn/gtzzbtlvjn.html

[S51] C++：显式类型转换
来源：http://hz.hnqzz.top/gtsafipkzq.html

static_cast<double>(a) / b
来源：http://hz.chenzaomai.com/gthhmijpiu.html

[S52] C++：const 与 noexcept
来源：http://hz.jinqigufen.top/gtjhjxdfow.html

int size() const noexcept { return n_; }
来源：http://hz.yuxming.cn/gtjfneouwm.html

[S53] C++：移动语义
来源：http://hz.hysaishi.cn/gtytqjyejk.html

std::vector<int> w = std::move(v);
来源：http://hz.fengsongda.top/gtwizjhbid.html

[S54] C++：异常处理
来源：http://hz.hywenlv.cn/gtiuqfclbq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xinyue.icu/gtlpgbqlvd.html

[S55] C++：结构化绑定
来源：http://hz.sysykeji.top/gtwaumkqzb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.hnqzz.top/gtsemxusei.html

[S56] C++：optional
来源：http://hz.jinqigfzy.top/gtxftreixu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tanke756.top/gtipzugyas.html

[S57] C++：编译期常量
来源：http://hz.xingfuxueyuan.xyz/gtxykryasp.html

constexpr int N = 10;
来源：http://hz.dashuyun.cn/gtlfnrvubb.html

[S58] C++：命名空间
来源：http://hz.jqgufenzy.top/gtucnxxclj.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhixingplan.top/gtifmyisxe.html

[S59] C++：静态断言
来源：http://hz.52xcode.cn/gthgsowjxl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.guannengcc.top/gtajattwlm.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangkeji.top/gtsadcfpmm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj202588.top/gtylqyeyiw.html

================================================================================
来源：http://hz.gotoacloud.top/gtfobycfgj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sufxvd.cn/gtojkkwogb.html

================================================================================
来源：http://hz.haohaochexian.top/gtzkrbpzfn.html

[T01] Kotlin：Hello World
来源：http://hz.52xcode.cn/gtzxbdktxy.html

println("Hello")
来源：http://hz.fengsongda.top/gtiyrzfqll.html

[T02] Kotlin：变量
来源：http://hz.hnxiangtu.top/gthcoypfxl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xuetiantiany.cn/gtibdpzfxr.html

[T03] Kotlin：字符串模板
来源：http://hz.kuanghao11.cn/gtftigoegz.html

"值: $b"
来源：http://hz.snrcjt.cn/gtfthksijl.html

[T04] Kotlin：空安全
来源：http://hz.smart0.xyz/gtplqmmnhz.html

val n: String? = null;  n?.length
来源：http://hz.jqgufenzy.top/gttlhilnit.html

[T05] Kotlin：when 表达式
来源：http://hz.xingfuxueyuan.xyz/gtyhuocskq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shuidangran.top/gttquigqyj.html

[T06] Kotlin：集合映射
来源：http://hz.shuidangran.top/gtdvycsohb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dashuyun.cn/gtoubjumky.html

[T07] Kotlin：集合过滤
来源：http://hz.daria6918.cn/gtosgcdvez.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ppjwa.cn/gtmzuingoc.html

[T08] Kotlin：数据类
来源：http://hz.hfpthk.cn/gtgeyxyzxc.html

data class User(val name: String, val age: Int)
来源：http://hz.jiagoushi.top/gthaitiayo.html

[T09] Kotlin：扩展函数
来源：http://hz.ybcxt.top/gttwmlnnwg.html

fun String.exclaim() = this + "!"
来源：http://hz.daxiang520.top/gtpngxmuym.html

[T10] Kotlin：默认参数
来源：http://hz.hongshengwenyu.top/gthhfaoght.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.bjfxy.top/gtrfcfbhnt.html

[T11] Kotlin：协程
来源：http://hz.bjfxy.top/gtkusxcrhu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daxiang520.top/gtnmmadjlj.html

[T12] Kotlin：解构声明
来源：http://hz.iojbl.cn/gtrhoeocok.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenlongwang.top/gtxzsmrifi.html

[T13] Kotlin：只读 Map
来源：http://hz.zhiwuduotai.top/gtpqtljqgg.html

val m = mapOf("a" to 1)
来源：http://hz.hysaishi.cn/gtijiaenrz.html

[T14] Kotlin：循环
来源：http://hz.hywenlv.cn/gtkmycousn.html

for (i in 1..10) println(i)
来源：http://hz.ydjk.org.cn/gttlqtyxum.html

[T15] Kotlin：接口
来源：http://hz.jinqigufen.top/gtcyjujvka.html

interface Shape { fun area(): Double }
来源：http://hz.nanxinkj.top/gtupsrknmh.html

[T16] Swift：Hello World
来源：http://hz.shzxlz.cn/gtmtvtuprz.html

print("Hello")
来源：http://hz.nanxuanxn.top/gtzewhuejk.html

[T17] Swift：变量与常量
来源：http://hz.zhaomingkeji.xyz/gtpwzopluq.html

var a = 1;  let b = 2
来源：http://hz.gotoacloud.top/gtkidjbslz.html

[T18] Swift：字符串插值
来源：http://hz.jyoumei.cn/gtbmmhzcpd.html

"值: \(b)"
来源：http://hz.wangdashe.top/gtxzufjtyo.html

[T19] Swift：可选绑定
来源：http://hz.svipenyu.cn/gtnsuwtxfz.html

if let n = opt { print(n) }
来源：http://hz.sysykeji.top/gtgdzrqovt.html

[T20] Swift：数组操作
来源：http://hz.snrcjt.cn/gtbplfyfrx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.redwolf501.top/gtylbrgfxg.html

[T21] Swift：遍历
来源：http://hz.fengsongda.top/gtgcmnpjvd.html

for x in a { print(x) }
来源：http://hz.iojbl.cn/gtkgjreflc.html

[T22] Swift：字典
来源：http://hz.tian-w.cn/gtbvwkhuxn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cashguo.top/gtydkvcpvl.html

[T23] Swift：函数
来源：http://hz.smart0.xyz/gtydqevcid.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yanxiufei.cn/gtdudfpuuz.html

[T24] Swift：闭包
来源：http://hz.sysykeji.top/gtstjodpiw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.tanke756.top/gtikrwiifz.html

[T25] Swift：结构体
来源：http://hz.hfpthk.cn/gtyfrgtcay.html

struct P { var x: Int }
来源：http://hz.xuetiantiany.cn/gtlinsabxv.html

[T26] Swift：类与重写
来源：http://hz.hnxiangtu.top/gtyywkyljd.html

class A: Base { override func f() {} }
来源：http://hz.yongpay.top/gtysxrajwf.html

[T27] Swift：错误处理
来源：http://hz.jinqigufen.top/gtvrdchljl.html

do { try f() } catch { print(error) }
来源：http://hz.mhx1999.top/gtmxasgneh.html

[T28] Swift：枚举
来源：http://hz.bjfxy.top/gtqjvufmas.html

enum Color { case red, green }
来源：http://hz.xylfe.cn/gtqnxkluom.html

[T29] Swift：guard 提前返回
来源：http://hz.chenzaomai.com/gtqxagpure.html

guard let x = opt else { return }
来源：http://hz.yuanzhike.top/gtweribiet.html

[T30] Swift：协议
来源：http://hz.svipenyu.cn/gtanheszoa.html

protocol Shape { func area() -> Double }
来源：http://hz.shzxlz.cn/gtvoabzbst.html

[T31] Lua：Hello World
来源：http://hz.havefunace.top/gtdbzpfaza.html

print("Hello")
来源：http://hz.yuxming.cn/gtsvwqlnyp.html

[T32] Lua：局部变量
来源：http://hz.svipenyu.cn/gthoxiddok.html

local a = 1
来源：http://hz.ivvv.top/gtbmucmdem.html

[T33] Lua：表（数组）
来源：http://hz.ivvv.top/gttsulaxef.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xuanzx.com/gtpxcvknnn.html

[T34] Lua：遍历表
来源：http://hz.zhengqikj.top/gtchjhvrwe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.vqdsnc.cn/gtsbblgehw.html

[T35] Lua：字典表
来源：http://hz.jiagoushi.top/gtpyouknli.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj202588.top/gtseomwnvv.html

[T36] Lua：函数
来源：http://hz.pengpengdd.cyou/gtmzuhjlqp.html

function add(a, b) return a + b end
来源：http://hz.jinqigfzy.top/gtdqwiyhce.html

[T37] Lua：字符串拼接
来源：http://hz.yj202588.top/gtzfxksace.html

"a" .. "b"
来源：http://hz.quarkkingdee.top/gtkhwautfp.html

[T38] Lua：条件
来源：http://hz.ydzc1.top/gtkeagxqpw.html

if x > 0 then print("正") end
来源：http://hz.snrcjt.cn/gtujqleula.html

[T39] Lua：模式匹配
来源：http://hz.jqgufenzy.top/gtvhecklgj.html

string.find(s, "%d+")
来源：http://hz.nanxinkj.top/gtndrwovez.html

[T40] Lua：元表
来源：http://hz.daria6918.cn/gtpnresdda.html

setmetatable({}, { __index = base })
来源：http://hz.fzhhl.top/gtqnrzjfch.html

[T41] Perl：Hello World
来源：http://hz.zycfv.cn/gtlssoupzk.html

print "Hello\n";
来源：http://hz.meibo888.top/gtbidebwoo.html

[T42] Perl：变量类型
来源：http://hz.pycfn.com/gthfnyhrju.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.tanke756.top/gtykjbqagk.html

[T43] Perl：字符串插值
来源：http://hz.yangfankeji.com/gtdcouzfqm.html

"值: $a"
来源：http://hz.birdmap.top/gtfepdbbex.html

[T44] Perl：条件
来源：http://hz.zhengqikj.top/gtdhvusgww.html

if ($a > 0) { print "正"; }
来源：http://hz.feifeiyinyue.top/gtvxpcmkhd.html

[T45] Perl：数组遍历
来源：http://hz.ivvv.top/gtnjfclopr.html

for my $x (@arr) { print $x; }
来源：http://hz.shanyushiyangkeji.top/gtrpwciaip.html

[T46] Perl：哈希操作
来源：http://hz.xuetiantiany.cn/gtaeokgipx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinqigufen.top/gtllgdutqe.html

[T47] Perl：正则捕获
来源：http://hz.chenjidiqi.icu/gtuoefvlna.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nanxinkj.top/gtpgdovxgv.html

[T48] Perl：正则替换
来源：http://hz.yuanzhike.top/gthiwzhbiy.html

$s =~ s/old/new/g;
来源：http://hz.svipenyu.cn/gtrqyzswfg.html

[T49] Perl：函数
来源：http://hz.jinqigfzy.top/gtbsaadrzr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.daxiang520.top/gthzdbxdvq.html

[T50] Perl：逐行读文件
来源：http://hz.zhixingplan.top/gtehvzacew.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.svipenyu.cn/gtdxfxtvew.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.ydjk.org.cn/gttwgqalet.html

[T51] Scala：Hello World
来源：http://hz.pengpengdd.cyou/gtsjsgffwa.html

println("Hello")
来源：http://hz.chenjidiqi.icu/gtlrnfwxok.html

[T52] Scala：变量
来源：http://hz.andypj.xyz/gtnjblpocv.html

val a = 1;  var b = 2
来源：http://hz.cqqwz.cn/gtzqbhagga.html

[T53] Scala：字符串插值
来源：http://hz.wangshuangyany.cn/gtdkmsmqmq.html

s"值: $b"
来源：http://hz.xuetiantiany.cn/gttxeaafwv.html

[T54] Scala：集合映射
来源：http://hz.jqgufenzy.top/gtqbrodeow.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hnqzz.top/gtqmxuglkx.html

[T55] Scala：集合过滤
来源：http://hz.vqdsnc.cn/gtetakxlri.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dashuyun.cn/gtocyzskll.html

[T56] Scala：样例类
来源：http://hz.guannengcc.top/gttztxukqk.html

case class User(name: String, age: Int)
来源：http://hz.zhongyouzk.top/gtnsftgsyj.html

[T57] Scala：模式匹配
来源：http://hz.pengpengdd.cyou/gtljpwytte.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.nwbrower.top/gtwuucjduz.html

[T58] Scala：函数定义
来源：http://hz.gaohongyu789.top/gtqrwrsvip.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xinyue.icu/gtjxaihbpj.html

[T59] Scala：循环
来源：http://hz.shuidangran.top/gtdjhwhdeu.html

for (i <- 1 to 10) println(i)
来源：http://hz.jqgfzy.top/gtwvzylmwy.html

[T60] Scala：折叠
来源：http://hz.tanke756.top/gtvzpmzqjb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.bjfxy.top/gtvgnstovk.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtflxvobqy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.dianchejie.cn/gtxwouvmug.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtapjambpn.html

[U01] Py：创建虚拟环境
来源：http://hz.hywenlv.cn/gtogqaoccl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.gaohongyu789.top/gtwooitptj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhaomingkeji.xyz/gtrjqmumje.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.fengsongda.top/gtbzjozklz.html

[U03] Py：加载 .env 配置
来源：http://hz.yj20258.top/gtlythnjli.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhoulong.xyz/gttbsrayox.html

[U04] Py：变量调试打印
来源：http://hz.vqdsnc.cn/gtagtcmpjq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.gaohongyu789.top/gtjkvtistr.html

[U05] Py：列表去重且保序
来源：http://hz.haohaochexian.top/gthemferga.html

list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtgrqvyiqp.html

[U06] Py：合并两个字典
来源：http://hz.0kj1m.cn/gtlmyldvqs.html

{**a, **b}
来源：http://hz.dashuyun.cn/gtaxxtzsoz.html

[U07] Py：反转字典键值
来源：http://hz.hfpthk.cn/gttlfxithm.html

{v: k for k, v in d.items()}
来源：http://hz.jlsjyb.cn/gtuckuyjtt.html

[U08] Py：展平二维列表
来源：http://hz.cucudq.cn/gtihubnbzo.html

[y for x in nested for y in x]
来源：http://hz.zycfv.cn/gtwzwyyhwz.html

[U09] Py：字典取最大值的键
来源：http://hz.ybcxt.top/gtkkuhaobw.html

max(d, key=d.get)
来源：http://hz.fzhhl.top/gtucpplhdf.html

[U10] Py：按值排序字典
来源：http://hz.hammf.cn/gtrtkslwod.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.quarkkingdee.top/gtzlbdvfbu.html

[U11] Py：生成器表达式
来源：http://hz.tanke756.top/gtquvcsszy.html

(x * 2 for x in arr)
来源：http://hz.yongpay.top/gttbtnwtij.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.sysykeji.top/gtkdotawbp.html

Counter(arr).most_common(3)
来源：http://hz.yvedp.cn/gtwqitbkak.html

[U13] Py：固定长度队列
来源：http://hz.fengsongda.top/gthpbbpzpe.html

deque(maxlen=10)
来源：http://hz.jinyuanbaomall.cn/gtrfpsvdzw.html

[U14] Py：分组收集到列表
来源：http://hz.haohaochexian.top/gtwrvaqbce.html

defaultdict(list)
来源：http://hz.jinghuilouyu.cn/gthbyyxvct.html

[U15] Py：高精度计时
来源：http://hz.meibo888.top/gtszcrbwco.html

t = time.perf_counter()
来源：http://hz.316326.xyz/gteedemwij.html

[U16] Py：命令行参数解析
来源：http://hz.jqgfzy.top/gtpzamzhpz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.redwolf501.top/gtbqnmqvew.html

[U17] Py：初始化日志
来源：http://hz.cdnleiting.top/gtyamczzwo.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.quarkkingdee.top/gttzksyjij.html

[U18] Py：预编译正则
来源：http://hz.chenjidiqi.icu/gtjarhhsez.html

pat = re.compile(r"\d+")
来源：http://hz.ydjk.org.cn/gtpzkmgmxz.html

[U19] Py：正则替换带回调
来源：http://hz.yanxiufei.cn/gtgzruhixh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yanxiufei.cn/gtmxzygnrk.html

[U20] Py：缓存函数结果
来源：http://hz.quarkkingdee.top/gthhnmvryt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.xuetiantiany.cn/gtgjmmflqf.html

[U21] Py：自定义上下文管理器
来源：http://hz.xingfuxueyuan.xyz/gtoidfiyhi.html

@contextlib.contextmanager
来源：http://hz.shangyingyoupin.top/gtbrozactu.html

[U22] Py：矩阵转置
来源：http://hz.quarkkingdee.top/gtzaypwdwc.html

list(zip(*m))
来源：http://hz.jinqigfzy.top/gtyoljtyrx.html

[U23] Py：分块读取大文件
来源：http://hz.yj202588.top/gtedxagpao.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.nwbrower.top/gteweblgbw.html

[U24] Py：路径操作
来源：http://hz.mhx1999.top/gtvposnqos.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yongpay.top/gtmmydmdkw.html

[U25] Py：CSV 按字典读
来源：http://hz.9152youxi.cn/gtdezkzmqn.html

csv.DictReader(f)
来源：http://hz.ywan-chungtsiang.top/gtithphmms.html

[U26] Py：并发下载
来源：http://hz.haohaochexian.top/gtagzjpjfw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shanyushiyangkeji.top/gtjboljdhc.html

[U27] Py：异步 HTTP
来源：http://hz.gzhubu.top/gtveimsxkp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.pycfn.com/gtcxiwopxu.html

[U28] Py：类型别名
来源：http://hz.xziqi.cn/gtwojgwkrw.html

UserId = int
来源：http://hz.9152youxi.cn/gtrvrpqvko.html

[U29] Py：属性校验
来源：http://hz.bjfxy.top/gtyipbpbst.html

@property 与 @x.setter 配合
来源：http://hz.hysaishi.cn/gtmmxjofjq.html

[U30] Py：数据类
来源：http://hz.shzxlz.cn/gtszwvbvit.html

@dataclass(slots=True)
来源：http://hz.ivvv.top/gtdxvnwydo.html

[U31] Py：单测
来源：http://hz.jyoumei.cn/gtkzluyljf.html

python -m pytest -q
来源：http://hz.yonumen.top/gtquqrgczo.html

[U32] Py：代码格式化
来源：http://hz.shuidangran.top/gttbbomjvq.html

ruff format . && ruff check --fix .
来源：http://hz.zhaomingkeji.xyz/gtwxmjwftp.html

[U33] Py：打包发布
来源：http://hz.yanxiufei.cn/gtpbkorzst.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.cashguo.top/gtqfdggiwu.html

[U34] Py：判断编码
来源：http://hz.yvedp.cn/gtfqrbheis.html

chardet.detect(raw)
来源：http://hz.zdqjudy.top/gtbwwdedpu.html

[U35] Py：发送邮件
来源：http://hz.yueranfly.top/gtsqsgrxts.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.pycfn.com/gtainmozvi.html

[U36] Py：定时任务
来源：http://hz.xuetiantiany.cn/gtzdeofcux.html

schedule.every(10).minutes.do(job)
来源：http://hz.nanxuanxn.top/gtsvavjslv.html

[U37] Py：读写 Excel
来源：http://hz.316326.xyz/gtmzejcwti.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xylfe.cn/gttejoubfp.html

[U38] Py：获取脚本所在目录
来源：http://hz.hfpthk.cn/gtimbnfpxq.html

Path(__file__).resolve().parent
来源：http://hz.shuidangran.top/gtsnmvxpyg.html

[U39] Py：判断是否在交互环境
来源：http://hz.vqdsnc.cn/gtfuszrhbm.html

sys.stdout.isatty()
来源：http://hz.jqgufenzy.top/gtsqkwgtaj.html

[U40] Py：打印到标准错误
来源：http://hz.meibo888.top/gtzmsljdzv.html

print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtlzgubnje.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yanxiufei.cn/gtlpatvwom.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ehwqpu.com/gtbuhqjlgp.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.fzhhl.top/gtkqiftory.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ppjwa.cn/gtnfwvelyn.html

[U43] PHP：声明命名空间
来源：http://hz.jianghu66.top/gtjsejeeol.html

namespace App\Http;
来源：http://hz.ydjk.org.cn/gthtchacpx.html

[U44] PHP：开启严格类型
来源：http://hz.jinghuilouyu.cn/gtzgstyadw.html

declare(strict_types=1);
来源：http://hz.yangfankeji.com/gtkigsqnii.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ppjwa.cn/gtulucvxsm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtkctmuvpu.html

[U46] PHP：可空类型
来源：http://hz.zhongyouzk.top/gtaawunvzm.html

?string $name = null
来源：http://hz.cqqwz.cn/gtkqfoqkmz.html

[U47] PHP：联合类型
来源：http://hz.hysaishi.cn/gtyeliushg.html

int|string $id
来源：http://hz.316326.xyz/gtzuuldssy.html

[U48] PHP：纯枚举
来源：http://hz.shangyingyoupin.top/gthkgtxpgi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.jianghu66.top/gtunexavty.html

[U49] PHP：只读属性
来源：http://hz.hongshengwenyu.top/gtvrhylzmh.html

public readonly string $name
来源：http://hz.cheryme.top/gtvomiztrr.html

[U50] PHP：构造器属性提升
来源：http://hz.xingfuxueyuan.xyz/gtsavaaqbv.html

public function __construct(private int $id) {}
来源：http://hz.dashuyun.cn/gtgkloyuxm.html

[U51] PHP：数组解构
来源：http://hz.tianlin.xyz/gtpdzshpva.html

[$a, $b] = $arr;
来源：http://hz.havefunace.top/gtljygixcf.html

[U52] PHP：箭头函数
来源：http://hz.andypj.xyz/gtqfznmgck.html

$double = fn($x) => $x * 2;
来源：http://hz.jqgfzy.top/gtprvplaks.html


<!-- 参考信息 -->