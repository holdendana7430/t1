代发 wailian999

static int counter = 0;
来源：http://hz.xylfe.cn/gtrbzhsyaa.html

[S29] C：变参函数
来源：http://hz.fengsongda.top/gtmpakohna.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.smart0.xyz/gtqsftrnpt.html

[S30] C：头文件保护
来源：http://hz.kuanghao11.cn/gtirdwronq.html

#ifndef X_H
来源：http://hz.9152youxi.cn/gtwwwdlpfl.html

#define X_H
来源：http://hz.vqdsnc.cn/gtzukhiahf.html

#endif
来源：http://hz.gotoacloud.top/gtshaipscl.html

[S31] C++：Hello World
来源：http://hz.ybcxt.top/gtvwmhpflg.html

#include <iostream>
来源：http://hz.hfpthk.cn/gtoyxargon.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jinqigufen.top/gtszumrfhg.html

[S32] C++：字符串
来源：http://hz.aibaodan.cn/gtkszlcbwf.html

std::string s = "hi";  s += "!";
来源：http://hz.hongshengwenyu.top/gtlsocprrn.html

[S33] C++：vector 增删
来源：http://hz.dashuyun.cn/gtcwfqtdno.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangdashe.top/gtdgtpcvqv.html

[S34] C++：遍历 vector
来源：http://hz.jqgufenzy.top/gtqyvdpcvv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.smart0.xyz/gtahkejsjz.html

[S35] C++：map
来源：http://hz.xuanzx.com/gtjfjdmpip.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ehwqpu.com/gtzlcjluon.html

[S36] C++：unordered_map
来源：http://hz.yj20258.top/gtwxionhww.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.aibaodan.cn/gtcawyyrcb.html

[S37] C++：set
来源：http://hz.haohaochexian.top/gtqptzykhe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gogol.net.cn/gtsetmdael.html

[S38] C++：排序
来源：http://hz.zhixingplan.top/gtthmqfixm.html

std::sort(v.begin(), v.end());
来源：http://hz.0kj1m.cn/gtygbmoedj.html

[S39] C++：自定义比较器排序
来源：http://hz.cqqwz.cn/gtezazirom.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jqgufenzy.top/gtludoezss.html

[S40] C++：查找元素
来源：http://hz.316326.xyz/gtrklouioq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yongpay.top/gtgjtuxrcl.html

[S41] C++：类与构造函数
来源：http://hz.9152youxi.cn/gtvgnciitf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yongpay.top/gtmbxzpoyw.html

[S42] C++：继承与虚函数
来源：http://hz.yuanzhike.top/gthtezezyx.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangdashe.top/gtyjfwwtps.html

[S43] C++：智能指针
来源：http://hz.gotoacloud.top/gtnjpcopra.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj20258888.top/gtttekhzig.html

[S44] C++：引用传参
来源：http://hz.9152youxi.cn/gtydddvuie.html

void inc(int &x) { ++x; }
来源：http://hz.havefunace.top/gtwfhcceoy.html

[S45] C++：lambda
来源：http://hz.yueranfly.top/gttnnfqtyt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.snrcjt.cn/gtzppfucam.html

[S46] C++：函数模板
来源：http://hz.chenzaomai.com/gtopjwyqkf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tianlin.xyz/gteqngmevx.html

[S47] C++：结构化绑定遍历
来源：http://hz.shuidangran.top/gthghssuql.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pengpengdd.cyou/gtklscftre.html

[S48] C++：逐行读文件
来源：http://hz.hnqzz.top/gtthmgkvyy.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhoulong.xyz/gtysxzmwxy.html

while (std::getline(in, line)) { }
来源：http://hz.yj20258.top/gtooihgbuq.html

[S49] C++：写文件
来源：http://hz.chenzaomai.com/gtebhemnpd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ybcxt.top/gtsagznuss.html

[S50] C++：格式化数字
来源：http://hz.gogol.net.cn/gthikskdyj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hywenlv.cn/gtvvbxdhin.html

[S51] C++：显式类型转换
来源：http://hz.wangdashe.top/gtkomufyal.html

static_cast<double>(a) / b
来源：http://hz.yonumen.top/gtjjdzoloh.html

[S52] C++：const 与 noexcept
来源：http://hz.mhx1999.top/gtqfemfevm.html

int size() const noexcept { return n_; }
来源：http://hz.jyoumei.cn/gtnccnshjf.html

[S53] C++：移动语义
来源：http://hz.tian-w.cn/gtlmqnvwux.html

std::vector<int> w = std::move(v);
来源：http://hz.tanke756.top/gtkoehpslb.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gtzdmyokww.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.tanke756.top/gtzzgjtadg.html

[S55] C++：结构化绑定
来源：http://hz.feifeiyinyue.top/gtspdrghrn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aibaodan.cn/gtxdffespv.html

[S56] C++：optional
来源：http://hz.xziqi.cn/gtmysvgtov.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.ybcxt.top/gtmcdrjcbm.html

[S57] C++：编译期常量
来源：http://hz.yj20258888.top/gtdjobhcxo.html

constexpr int N = 10;
来源：http://hz.birdmap.top/gtndwfvrdh.html

[S58] C++：命名空间
来源：http://hz.sweek.top/gthedwkjcv.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtdxtmeanh.html

[S59] C++：静态断言
来源：http://hz.redwolf501.top/gtwalasjxl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.nanxuanxn.top/gtbqnggvuo.html

[S60] C++：遍历并删除元素
来源：http://hz.zhengqikj.top/gtatyazegi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yvedp.cn/gtinzaphvt.html

================================================================================
来源：http://hz.ehwqpu.com/gtqtyasxtx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.quarkkingdee.top/gtwqhlkljo.html

================================================================================
来源：http://hz.daxiang520.top/gtettjlnmj.html

[T01] Kotlin：Hello World
来源：http://hz.hnqzz.top/gtdmgyugqb.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gtykipnbvk.html

[T02] Kotlin：变量
来源：http://hz.cqqwz.cn/gtqnqbgwoy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhongyouzk.top/gtrypvkbxf.html

[T03] Kotlin：字符串模板
来源：http://hz.daxiang520.top/gtzeveoagg.html

"值: $b"
来源：http://hz.shanyushiyangtech.top/gtykppnvmt.html

[T04] Kotlin：空安全
来源：http://hz.chenlongwang.top/gtcaofgeaz.html

val n: String? = null;  n?.length
来源：http://hz.kuanghao11.cn/gtavileazn.html

[T05] Kotlin：when 表达式
来源：http://hz.yvedp.cn/gtndldsqah.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cucudq.cn/gtqcxnbflw.html

[T06] Kotlin：集合映射
来源：http://hz.9152youxi.cn/gtkgwejozn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xingfuxueyuan.xyz/gtjyejvoyq.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258.top/gtattqppkj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ydjk.org.cn/gtzhecyrai.html

[T08] Kotlin：数据类
来源：http://hz.ehwqpu.com/gtgmekkcbt.html

data class User(val name: String, val age: Int)
来源：http://hz.svipenyu.cn/gtceuvcpsf.html

[T09] Kotlin：扩展函数
来源：http://hz.zdqjudy.top/gtzyfgyvfb.html

fun String.exclaim() = this + "!"
来源：http://hz.gaohongyu789.top/gtdmolsxwr.html

[T10] Kotlin：默认参数
来源：http://hz.jiagoushi.top/gtsceheurj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sysykeji.top/gthlosdrbq.html

[T11] Kotlin：协程
来源：http://hz.jqgufenzy.top/gtxspgfpxq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jyoumei.cn/gtfotzmrmm.html

[T12] Kotlin：解构声明
来源：http://hz.haohaochexian.top/gtesidnzkj.html

val (a, b) = Pair(1, 2)
来源：http://hz.fengsongda.top/gtgodwgbux.html

[T13] Kotlin：只读 Map
来源：http://hz.yuanzhike.top/gtohxqpymk.html

val m = mapOf("a" to 1)
来源：http://hz.chenzaomai.com/gtmtodmrgg.html

[T14] Kotlin：循环
来源：http://hz.dianchejie.cn/gtcupvvjzc.html

for (i in 1..10) println(i)
来源：http://hz.yuxming.cn/gtekersamx.html

[T15] Kotlin：接口
来源：http://hz.chenzaomai.com/gtavzblryk.html

interface Shape { fun area(): Double }
来源：http://hz.wangdashe.top/gtwpvaddvt.html

[T16] Swift：Hello World
来源：http://hz.chenzaomai.com/gtpnisuezx.html

print("Hello")
来源：http://hz.sysykeji.top/gtebmylibk.html

[T17] Swift：变量与常量
来源：http://hz.xuetiantiany.cn/gtpszkndmq.html

var a = 1;  let b = 2
来源：http://hz.xuanzx.com/gtjiusiezq.html

[T18] Swift：字符串插值
来源：http://hz.yj20258888.top/gtywscgmfq.html

"值: \(b)"
来源：http://hz.snrcjt.cn/gtbbomrkbr.html

[T19] Swift：可选绑定
来源：http://hz.yonumen.top/gthdcyfuuv.html

if let n = opt { print(n) }
来源：http://hz.feifeiyinyue.top/gtpoqzjvqb.html

[T20] Swift：数组操作
来源：http://hz.sysykeji.top/gtojbkcwhr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shuidangran.top/gtygmmxiyw.html

[T21] Swift：遍历
来源：http://hz.dashuyun.cn/gttllznltj.html

for x in a { print(x) }
来源：http://hz.ywan-chungtsiang.top/gtqwjerkqp.html

[T22] Swift：字典
来源：http://hz.chenlongwang.top/gtczsslhtu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daxiang520.top/gtgnzbcgme.html

[T23] Swift：函数
来源：http://hz.nanxuanxn.top/gtnhwrofqa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.andypj.xyz/gtelzkqmig.html

[T24] Swift：闭包
来源：http://hz.svipenyu.cn/gtniofwpwg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xingfuxueyuan.xyz/gtvgmuyeew.html

[T25] Swift：结构体
来源：http://hz.jqgfzy.top/gtiukopadn.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gtrmvofsiu.html

[T26] Swift：类与重写
来源：http://hz.meibo888.top/gtxmgntkuu.html

class A: Base { override func f() {} }
来源：http://hz.9152youxi.cn/gteikqkdio.html

[T27] Swift：错误处理
来源：http://hz.feifeiyinyue.top/gtirnugldt.html

do { try f() } catch { print(error) }
来源：http://hz.hongshengwenyu.top/gtfxrdgfkb.html

[T28] Swift：枚举
来源：http://hz.kuanghao11.cn/gtjenqzueb.html

enum Color { case red, green }
来源：http://hz.snrcjt.cn/gtfugxnyzg.html

[T29] Swift：guard 提前返回
来源：http://hz.jiagoushi.top/gteisulnco.html

guard let x = opt else { return }
来源：http://hz.yangfankeji.com/gtfrujgmfm.html

[T30] Swift：协议
来源：http://hz.shangyingyoupin.top/gtefnrtbyv.html

protocol Shape { func area() -> Double }
来源：http://hz.pycfn.com/gtknxrdyfz.html

[T31] Lua：Hello World
来源：http://hz.yueranfly.top/gtyjeaxmgf.html

print("Hello")
来源：http://hz.smart0.xyz/gtblmcelar.html

[T32] Lua：局部变量
来源：http://hz.feifeiyinyue.top/gtsfqatwww.html

local a = 1
来源：http://hz.sufxvd.cn/gtmgsicngw.html

[T33] Lua：表（数组）
来源：http://hz.nanxinkj.top/gtzorfxfkr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sxryk.cn/gtbajcmmod.html

[T34] Lua：遍历表
来源：http://hz.hywenlv.cn/gtvlvoxhzo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zycfv.cn/gtowimawek.html

[T35] Lua：字典表
来源：http://hz.9152youxi.cn/gtsasicqov.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jqgufenzy.top/gtdecummdt.html

[T36] Lua：函数
来源：http://hz.ehwqpu.com/gtkagjfrhw.html

function add(a, b) return a + b end
来源：http://hz.gotoacloud.top/gtsxgjwolt.html

[T37] Lua：字符串拼接
来源：http://hz.tanke756.top/gtfaojrlei.html

"a" .. "b"
来源：http://hz.52xcode.cn/gttkubnwja.html

[T38] Lua：条件
来源：http://hz.ppjwa.cn/gtvsadupic.html

if x > 0 then print("正") end
来源：http://hz.kuanghao11.cn/gtenuhrahr.html

[T39] Lua：模式匹配
来源：http://hz.redwolf501.top/gthrzdnjkv.html

string.find(s, "%d+")
来源：http://hz.hongshengwenyu.top/gtbeuuaicd.html

[T40] Lua：元表
来源：http://hz.yj202588.top/gtcxsmozkg.html

setmetatable({}, { __index = base })
来源：http://hz.havefunace.top/gtkvedoogb.html

[T41] Perl：Hello World
来源：http://hz.iojbl.cn/gtpzuhsljh.html

print "Hello\n";
来源：http://hz.ydzc1.top/gtthxcpevn.html

[T42] Perl：变量类型
来源：http://hz.chenzaomai.com/gtynmrgjbn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.aizwys.cn/gttmkzxecy.html

[T43] Perl：字符串插值
来源：http://hz.xziqi.cn/gtpcharhrp.html

"值: $a"
来源：http://hz.guannengcc.top/gtsygiuhjl.html

[T44] Perl：条件
来源：http://hz.daria6918.cn/gtakwdmemt.html

if ($a > 0) { print "正"; }
来源：http://hz.cucudq.cn/gtwvumxtip.html

[T45] Perl：数组遍历
来源：http://hz.chenjidiqi.icu/gtzcblfnzt.html

for my $x (@arr) { print $x; }
来源：http://hz.daria6918.cn/gtymfpwlwm.html

[T46] Perl：哈希操作
来源：http://hz.gotoacloud.top/gtemzltshc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhoulong.xyz/gtoeschnbk.html

[T47] Perl：正则捕获
来源：http://hz.aizwys.cn/gtizatayqn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xuetiantiany.cn/gtnzqncpkz.html

[T48] Perl：正则替换
来源：http://hz.52xcode.cn/gtwbaejffi.html

$s =~ s/old/new/g;
来源：http://hz.zhijiandao.cn/gtqyqppvvf.html

[T49] Perl：函数
来源：http://hz.jqgufenzy.top/gtstbwvvgd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shuidangran.top/gtuqdbsexk.html

[T50] Perl：逐行读文件
来源：http://hz.yj202588.top/gtrbfvleiw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.feifeiyinyue.top/gtoymanvhb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.aibaodan.cn/gtebyfbqza.html

[T51] Scala：Hello World
来源：http://hz.tian-w.cn/gterwshxzt.html

println("Hello")
来源：http://hz.shangyingyoupin.top/gthfevxrhd.html

[T52] Scala：变量
来源：http://hz.chenlongwang.top/gthvksxrnp.html

val a = 1;  var b = 2
来源：http://hz.wangshuangyany.cn/gtfvendaht.html

[T53] Scala：字符串插值
来源：http://hz.zycfv.cn/gtnfrypzxb.html

s"值: $b"
来源：http://hz.jinghuilouyu.cn/gthzxdivjv.html

[T54] Scala：集合映射
来源：http://hz.chenjidiqi.icu/gtjszeltvb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuanzhike.top/gtttustven.html

[T55] Scala：集合过滤
来源：http://hz.yonumen.top/gtzjwyffez.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.aizwys.cn/gtgnzuaapp.html

[T56] Scala：样例类
来源：http://hz.0kj1m.cn/gthkczswiq.html

case class User(name: String, age: Int)
来源：http://hz.fzhhl.top/gtvasdzazg.html

[T57] Scala：模式匹配
来源：http://hz.nwbrower.top/gtndybvmvv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.316326.xyz/gtwfmsbgbp.html

[T58] Scala：函数定义
来源：http://hz.aibaodan.cn/gtqgkljwfr.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shanyushiyangtech.top/gttuspzcaq.html

[T59] Scala：循环
来源：http://hz.jiagoushi.top/gtrbyilofk.html

for (i <- 1 to 10) println(i)
来源：http://hz.smart0.xyz/gtdmzxtbbe.html

[T60] Scala：折叠
来源：http://hz.sysykeji.top/gtfzrzwave.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.cdnleiting.top/gtqnhmflaz.html

================================================================================
来源：http://hz.jlsjyb.cn/gtclbumtoi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhiwuduotai.top/gtzioxnjjd.html

================================================================================
来源：http://hz.sweek.top/gtkmlywjxh.html

[U01] Py：创建虚拟环境
来源：http://hz.ehwqpu.com/gtwcundvkt.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hammf.cn/gtcqmdlfta.html

[U02] Py：导出 / 安装依赖
来源：http://hz.redwolf501.top/gtomxpiqiu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.9152youxi.cn/gtiojrztil.html

[U03] Py：加载 .env 配置
来源：http://hz.yj202588.top/gtfjojyuez.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhaomingkeji.xyz/gtxzowdull.html

[U04] Py：变量调试打印
来源：http://hz.sysykeji.top/gtjgddwuws.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xylfe.cn/gtvfmrzjtz.html

[U05] Py：列表去重且保序
来源：http://hz.dianchejie.cn/gtmoyfdsdt.html

list(dict.fromkeys(arr))
来源：http://hz.shuidangran.top/gtqoihnwzp.html

[U06] Py：合并两个字典
来源：http://hz.cqqwz.cn/gtrfsnqhty.html

{**a, **b}
来源：http://hz.feifeiyinyue.top/gttvyaxjau.html

[U07] Py：反转字典键值
来源：http://hz.hnxiangtu.top/gteghjhuxk.html

{v: k for k, v in d.items()}
来源：http://hz.andypj.xyz/gtwbdsqlcm.html

[U08] Py：展平二维列表
来源：http://hz.jyoumei.cn/gtauzsldvw.html

[y for x in nested for y in x]
来源：http://hz.daria6918.cn/gtvjhvdtpm.html

[U09] Py：字典取最大值的键
来源：http://hz.zhixingplan.top/gtlydptcci.html

max(d, key=d.get)
来源：http://hz.gzhubu.top/gtrlaczvvo.html

[U10] Py：按值排序字典
来源：http://hz.sweek.top/gtcmhbgvwc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ivvv.top/gtqnxftqnv.html

[U11] Py：生成器表达式
来源：http://hz.zhengqikj.top/gtsbpglxba.html

(x * 2 for x in arr)
来源：http://hz.wangshuangyany.cn/gtdxsboleo.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.9152youxi.cn/gtaeivfgnw.html

Counter(arr).most_common(3)
来源：http://hz.yvedp.cn/gthjrvuiii.html

[U13] Py：固定长度队列
来源：http://hz.jianghu66.top/gtmuitrrbv.html

deque(maxlen=10)
来源：http://hz.haohaochexian.top/gtouqbioyf.html

[U14] Py：分组收集到列表
来源：http://hz.haohaochexian.top/gtmdslgloi.html

defaultdict(list)
来源：http://hz.jiagoushi.top/gtdroerowx.html

[U15] Py：高精度计时
来源：http://hz.hywenlv.cn/gttxzrsrgg.html

t = time.perf_counter()
来源：http://hz.yangfankeji.com/gtdcpuzsdt.html

[U16] Py：命令行参数解析
来源：http://hz.wangshuangyany.cn/gtodlteepe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.daria6918.cn/gtlbwptdjh.html

[U17] Py：初始化日志
来源：http://hz.jianghu66.top/gtgdkxcgdd.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.wangshuangyany.cn/gtsbuooabn.html

[U18] Py：预编译正则
来源：http://hz.yongpay.top/gtuwhrihbo.html

pat = re.compile(r"\d+")
来源：http://hz.ybcxt.top/gtkfnaobna.html

[U19] Py：正则替换带回调
来源：http://hz.tian-w.cn/gtrqyzvpom.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.316326.xyz/gtlmwcqrpd.html

[U20] Py：缓存函数结果
来源：http://hz.jqgfzy.top/gtowvnusrd.html

@functools.lru_cache(maxsize=None)
来源：http://hz.chenlongwang.top/gtqbwjrzpj.html

[U21] Py：自定义上下文管理器
来源：http://hz.sweek.top/gtovsbqcqp.html

@contextlib.contextmanager
来源：http://hz.vqdsnc.cn/gthfskpwwx.html

[U22] Py：矩阵转置
来源：http://hz.haohaochexian.top/gtbalirnpa.html

list(zip(*m))
来源：http://hz.jqgfzy.top/gtehruxglw.html

[U23] Py：分块读取大文件
来源：http://hz.haohaochexian.top/gtjqrsyuel.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jyoumei.cn/gtbxgmggbg.html

[U24] Py：路径操作
来源：http://hz.jianghu66.top/gtmepfzwij.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gtwtafdjes.html

[U25] Py：CSV 按字典读
来源：http://hz.9152youxi.cn/gtrcfvisxe.html

csv.DictReader(f)
来源：http://hz.ehwqpu.com/gtcmwavelj.html

[U26] Py：并发下载
来源：http://hz.xinyue.icu/gtspayoelw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jiagoushi.top/gtlmrflfvp.html

[U27] Py：异步 HTTP
来源：http://hz.redwolf501.top/gtowhhglof.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.svipenyu.cn/gtsfsjaxft.html

[U28] Py：类型别名
来源：http://hz.yuanzhike.top/gtirztjxkw.html

UserId = int
来源：http://hz.hnqzz.top/gtzeixklwh.html

[U29] Py：属性校验
来源：http://hz.daxiang520.top/gtjnahfcrm.html

@property 与 @x.setter 配合
来源：http://hz.yvedp.cn/gtriwsgqhb.html

[U30] Py：数据类
来源：http://hz.xziqi.cn/gtdcgcjmrg.html

@dataclass(slots=True)
来源：http://hz.zhijiandao.cn/gtegxdulnl.html

[U31] Py：单测
来源：http://hz.zhongyouzk.top/gtiemqmezc.html

python -m pytest -q
来源：http://hz.xuanzx.com/gtujeevomx.html

[U32] Py：代码格式化
来源：http://hz.bjfxy.top/gtikigohpp.html

ruff format . && ruff check --fix .
来源：http://hz.shanyushiyangtech.top/gttociqkpp.html

[U33] Py：打包发布
来源：http://hz.xinyue.icu/gtfryudvbm.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.wangshuangyany.cn/gtdlnpvcgl.html

[U34] Py：判断编码
来源：http://hz.vqdsnc.cn/gtdqxdigim.html

chardet.detect(raw)
来源：http://hz.zhaomingkeji.xyz/gtitpiixcb.html

[U35] Py：发送邮件
来源：http://hz.zhiwuduotai.top/gtothefshj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zdqjudy.top/gtyxiozzny.html

[U36] Py：定时任务
来源：http://hz.jyoumei.cn/gthwuzatjw.html

schedule.every(10).minutes.do(job)
来源：http://hz.yuanzhike.top/gtchuiqtap.html

[U37] Py：读写 Excel
来源：http://hz.shzxlz.cn/gtcrplpzuq.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.c1oappe.top/gtvaxmmirq.html

[U38] Py：获取脚本所在目录
来源：http://hz.hfpthk.cn/gtvlyovkqe.html

Path(__file__).resolve().parent
来源：http://hz.aizwys.cn/gtkgkjudqg.html

[U39] Py：判断是否在交互环境
来源：http://hz.aizwys.cn/gthvosuruj.html

sys.stdout.isatty()
来源：http://hz.mhx1999.top/gtajwpdkwo.html

[U40] Py：打印到标准错误
来源：http://hz.shanyushiyangtech.top/gtqjdktyjl.html

print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtbhddfshh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhijiandao.cn/gtiyhynpmi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.andypj.xyz/gtpibccdje.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.cashguo.top/gtfatwjhwu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.havefunace.top/gtjgqftkbh.html

[U43] PHP：声明命名空间
来源：http://hz.jlsjyb.cn/gtbakdwnlx.html

namespace App\Http;
来源：http://hz.jinghuilouyu.cn/gtnrkcogqa.html

[U44] PHP：开启严格类型
来源：http://hz.jinghuilouyu.cn/gtzyeifybt.html

declare(strict_types=1);
来源：http://hz.dashuyun.cn/gtncjkluxl.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yuxming.cn/gtntibhjqw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtroemrnbn.html

[U46] PHP：可空类型
来源：http://hz.jlsjyb.cn/gtgpdxzcwg.html

?string $name = null
来源：http://hz.xylfe.cn/gtafrfuqul.html

[U47] PHP：联合类型
来源：http://hz.iojbl.cn/gtlpurisbb.html

int|string $id
来源：http://hz.jinghuilouyu.cn/gtdbnsskws.html

[U48] PHP：纯枚举
来源：http://hz.pengpengdd.cyou/gtjvmraqya.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.aizwys.cn/gtlqgfyqds.html

[U49] PHP：只读属性
来源：http://hz.birdmap.top/gtcoqtjnts.html

public readonly string $name
来源：http://hz.yangfankeji.com/gttskcfbst.html

[U50] PHP：构造器属性提升
来源：http://hz.ydzc1.top/gtbaipurxz.html

public function __construct(private int $id) {}
来源：http://hz.gaohongyu789.top/gtynlepsxg.html

[U51] PHP：数组解构
来源：http://hz.snrcjt.cn/gtgfwsuauh.html

[$a, $b] = $arr;
来源：http://hz.daria6918.cn/gtoyfysnev.html

[U52] PHP：箭头函数
来源：http://hz.sxryk.cn/gtijvffikj.html

$double = fn($x) => $x * 2;
来源：http://hz.yonumen.top/gtvgpzcgar.html


<!-- 参考信息 -->