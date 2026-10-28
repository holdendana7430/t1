代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xuetiantiany.cn/gtdhubwjtl.html

[S25] C：内存拷贝
来源：http://hz.0kj1m.cn/gtqttlzvwz.html

memcpy(dst, src, n);
来源：http://hz.tanke756.top/gtywhvzmyl.html

[S26] C：内存清零
来源：http://hz.bjfxy.top/gtwifotsnd.html

memset(a, 0, sizeof a);
来源：http://hz.iojbl.cn/gtqcqtqtng.html

[S27] C：定义常量
来源：http://hz.yvedp.cn/gtdchyoird.html

const double PI = 3.14159;
来源：http://hz.daxiang520.top/gtsyzutlvw.html

[S28] C：静态变量
来源：http://hz.316326.xyz/gteawktkra.html

static int counter = 0;
来源：http://hz.ybcxt.top/gtohkisgwa.html

[S29] C：变参函数
来源：http://hz.jiagoushi.top/gtbynuympa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.andypj.xyz/gtyjznongl.html

[S30] C：头文件保护
来源：http://hz.guowangkeji.top/gttcfaypsf.html

#ifndef X_H
来源：http://hz.meibo888.top/gtaytroemc.html

#define X_H
来源：http://hz.jianghu66.top/gtpzpnqayz.html

#endif
来源：http://hz.quarkkingdee.top/gthwiooduv.html

[S31] C++：Hello World
来源：http://hz.yj20258.top/gtqkkvhwdt.html

#include <iostream>
来源：http://hz.hnxiangtu.top/gtaszektgj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shanyushiyangkeji.top/gtsthfnfah.html

[S32] C++：字符串
来源：http://hz.52xcode.cn/gtgwvojmre.html

std::string s = "hi";  s += "!";
来源：http://hz.sxryk.cn/gtqkquvuwc.html

[S33] C++：vector 增删
来源：http://hz.shuidangran.top/gtsklobifp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj20258888.top/gtprqgcdeq.html

[S34] C++：遍历 vector
来源：http://hz.sysykeji.top/gtnzbjqsjg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fzhhl.top/gtefaehxtp.html

[S35] C++：map
来源：http://hz.shzxlz.cn/gtanfaipfg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtotsabsec.html

[S36] C++：unordered_map
来源：http://hz.hnqzz.top/gtdiahflzd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.birdmap.top/gtbxwroumu.html

[S37] C++：set
来源：http://hz.tianlin.xyz/gtfibpzudg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.redwolf501.top/gtgxbejcmm.html

[S38] C++：排序
来源：http://hz.jinyuanbaomall.cn/gtgjrbpfxk.html

std::sort(v.begin(), v.end());
来源：http://hz.chenlongwang.top/gtznnexiho.html

[S39] C++：自定义比较器排序
来源：http://hz.shanyushiyangkeji.top/gtmkvyxaoq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.pengpengdd.cyou/gtwajwzxhb.html

[S40] C++：查找元素
来源：http://hz.meibo888.top/gtqsrkdbtc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.kuanghao11.cn/gtqiipvist.html

[S41] C++：类与构造函数
来源：http://hz.guowangkeji.top/gtrmhymcqp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yuxming.cn/gtwmgyrjvl.html

[S42] C++：继承与虚函数
来源：http://hz.sysykeji.top/gthcqojchy.html

class B : public Base { public: void f() override {} };
来源：http://hz.hysaishi.cn/gtwdhvcjye.html

[S43] C++：智能指针
来源：http://hz.birdmap.top/gthckbbwmo.html

auto p = std::make_unique<int>(5);
来源：http://hz.kuanghao11.cn/gtgycjhdlq.html

[S44] C++：引用传参
来源：http://hz.chenjidiqi.icu/gtukucmunq.html

void inc(int &x) { ++x; }
来源：http://hz.zhoulong.xyz/gtxpdyesge.html

[S45] C++：lambda
来源：http://hz.yj20258888.top/gtoapmuiqb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xinyue.icu/gtothjqjuk.html

[S46] C++：函数模板
来源：http://hz.nanxuanxn.top/gtlqncmweb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhixingplan.top/gtkgndlqyv.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhengqikj.top/gtuyqxnaif.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hammf.cn/gtyitzedbi.html

[S48] C++：逐行读文件
来源：http://hz.nanxuanxn.top/gtywhftqqs.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhongyouzk.top/gtmqlrdmww.html

while (std::getline(in, line)) { }
来源：http://hz.zhijiandao.cn/gtxgvikzhm.html

[S49] C++：写文件
来源：http://hz.tian-w.cn/gtypwccyej.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuanzhike.top/gtopcxuqdz.html

[S50] C++：格式化数字
来源：http://hz.fzhhl.top/gtfavhhqbl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cdnleiting.top/gtaycionsi.html

[S51] C++：显式类型转换
来源：http://hz.xylfe.cn/gtkhblgfxy.html

static_cast<double>(a) / b
来源：http://hz.9152youxi.cn/gtrafgbtxq.html

[S52] C++：const 与 noexcept
来源：http://hz.xinyue.icu/gtyabvhyvf.html

int size() const noexcept { return n_; }
来源：http://hz.hfpthk.cn/gtvhfmvmhv.html

[S53] C++：移动语义
来源：http://hz.shangyingyoupin.top/gtkhabngha.html

std::vector<int> w = std::move(v);
来源：http://hz.xinyue.icu/gtqdhnoxuc.html

[S54] C++：异常处理
来源：http://hz.sufxvd.cn/gthbibqjvf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.shuidangran.top/gtzjdubeeu.html

[S55] C++：结构化绑定
来源：http://hz.9152youxi.cn/gtqlsgzrba.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.316326.xyz/gtanxiqffc.html

[S56] C++：optional
来源：http://hz.sxryk.cn/gtouapbtul.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aibaodan.cn/gtcrdxzmam.html

[S57] C++：编译期常量
来源：http://hz.dashuyun.cn/gtjfnglzpn.html

constexpr int N = 10;
来源：http://hz.haohaochexian.top/gtecqqsgje.html

[S58] C++：命名空间
来源：http://hz.cqqwz.cn/gtbukwtulu.html

namespace ns { int f() { return 1; } }
来源：http://hz.hysaishi.cn/gtxayygumk.html

[S59] C++：静态断言
来源：http://hz.jinghuilouyu.cn/gtccqnopqm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhaomingkeji.xyz/gtcovvtdse.html

[S60] C++：遍历并删除元素
来源：http://hz.shzxlz.cn/gtawqjemie.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hnqzz.top/gtwbpexuzw.html

================================================================================
来源：http://hz.ivvv.top/gtykbqwzkq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgufenzy.top/gtetuvcivh.html

================================================================================
来源：http://hz.xuanzx.com/gthyvntkbp.html

[T01] Kotlin：Hello World
来源：http://hz.aibaodan.cn/gtgillchvh.html

println("Hello")
来源：http://hz.0kj1m.cn/gtalthetkk.html

[T02] Kotlin：变量
来源：http://hz.tianlin.xyz/gtzyfaalkg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jianghu66.top/gtnnpcdfra.html

[T03] Kotlin：字符串模板
来源：http://hz.shuidangran.top/gtcwznnsei.html

"值: $b"
来源：http://hz.aizwys.cn/gtxmbbfrxk.html

[T04] Kotlin：空安全
来源：http://hz.chenzaomai.com/gtevrhbufr.html

val n: String? = null;  n?.length
来源：http://hz.zhijiandao.cn/gtvkvqyvzz.html

[T05] Kotlin：when 表达式
来源：http://hz.shzxlz.cn/gtgmaofbcu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yueranfly.top/gtkxncxklc.html

[T06] Kotlin：集合映射
来源：http://hz.fzhhl.top/gtjegypmpb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xuanzx.com/gtafaptugc.html

[T07] Kotlin：集合过滤
来源：http://hz.tianlin.xyz/gthlsaruaw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinyuanbaomall.cn/gtnhtvreab.html

[T08] Kotlin：数据类
来源：http://hz.iojbl.cn/gtemkqoayr.html

data class User(val name: String, val age: Int)
来源：http://hz.yvedp.cn/gtzqicyumo.html

[T09] Kotlin：扩展函数
来源：http://hz.shuidangran.top/gtvwdoqdev.html

fun String.exclaim() = this + "!"
来源：http://hz.fengsongda.top/gtbtgdhsfb.html

[T10] Kotlin：默认参数
来源：http://hz.ehwqpu.com/gtwfbdswls.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.pycfn.com/gtbdureyan.html

[T11] Kotlin：协程
来源：http://hz.havefunace.top/gtecgmrbnp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yuxming.cn/gtboicwfwd.html

[T12] Kotlin：解构声明
来源：http://hz.zycfv.cn/gteqcaqzbv.html

val (a, b) = Pair(1, 2)
来源：http://hz.yvedp.cn/gtkvxqzhdg.html

[T13] Kotlin：只读 Map
来源：http://hz.zhiwuduotai.top/gtreqomoce.html

val m = mapOf("a" to 1)
来源：http://hz.dianchejie.cn/gtfsyhbwtz.html

[T14] Kotlin：循环
来源：http://hz.ywan-chungtsiang.top/gtjohucotd.html

for (i in 1..10) println(i)
来源：http://hz.yuxming.cn/gtynakohmx.html

[T15] Kotlin：接口
来源：http://hz.meibo888.top/gtbqcopasr.html

interface Shape { fun area(): Double }
来源：http://hz.hnqzz.top/gtxntqbvyp.html

[T16] Swift：Hello World
来源：http://hz.sufxvd.cn/gtezmloqjw.html

print("Hello")
来源：http://hz.ywan-chungtsiang.top/gtuncuyikg.html

[T17] Swift：变量与常量
来源：http://hz.sweek.top/gtgghlozzs.html

var a = 1;  let b = 2
来源：http://hz.zhengqikj.top/gtgzipefhx.html

[T18] Swift：字符串插值
来源：http://hz.xylfe.cn/gtixrinzdx.html

"值: \(b)"
来源：http://hz.pengpengdd.cyou/gtujgrdhea.html

[T19] Swift：可选绑定
来源：http://hz.quarkkingdee.top/gtijuoozks.html

if let n = opt { print(n) }
来源：http://hz.kuanghao11.cn/gttwflozmj.html

[T20] Swift：数组操作
来源：http://hz.bjfxy.top/gteuaejvzj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jianghu66.top/gtfsjufphj.html

[T21] Swift：遍历
来源：http://hz.chenzaomai.com/gtkjlzaxjg.html

for x in a { print(x) }
来源：http://hz.zhixingplan.top/gtqidtcpmv.html

[T22] Swift：字典
来源：http://hz.chenlongwang.top/gtjlnskbnn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.snrcjt.cn/gtxubyamrt.html

[T23] Swift：函数
来源：http://hz.iojbl.cn/gtmwelysri.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.fzhhl.top/gtprksdxai.html

[T24] Swift：闭包
来源：http://hz.cashguo.top/gtuzwepldn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.0kj1m.cn/gtlkhnfope.html

[T25] Swift：结构体
来源：http://hz.zhongyouzk.top/gtzokhvqwv.html

struct P { var x: Int }
来源：http://hz.dianchejie.cn/gtsojvuxct.html

[T26] Swift：类与重写
来源：http://hz.zycfv.cn/gtbosivekn.html

class A: Base { override func f() {} }
来源：http://hz.jyoumei.cn/gtnnyeopdk.html

[T27] Swift：错误处理
来源：http://hz.fengsongda.top/gttxnpuksi.html

do { try f() } catch { print(error) }
来源：http://hz.shuidangran.top/gtyeyxravo.html

[T28] Swift：枚举
来源：http://hz.ivvv.top/gtakuzdhgf.html

enum Color { case red, green }
来源：http://hz.jinqigufen.top/gtasbzpjzf.html

[T29] Swift：guard 提前返回
来源：http://hz.havefunace.top/gtbwfimihb.html

guard let x = opt else { return }
来源：http://hz.pengpengdd.cyou/gtihyelemb.html

[T30] Swift：协议
来源：http://hz.aizwys.cn/gtddknelvf.html

protocol Shape { func area() -> Double }
来源：http://hz.cucudq.cn/gtnefkbzvq.html

[T31] Lua：Hello World
来源：http://hz.dianchejie.cn/gtzfmfdqhg.html

print("Hello")
来源：http://hz.xuetiantiany.cn/gtkzknpmry.html

[T32] Lua：局部变量
来源：http://hz.hysaishi.cn/gthzuskotz.html

local a = 1
来源：http://hz.hysaishi.cn/gtladwjjbn.html

[T33] Lua：表（数组）
来源：http://hz.gaohongyu789.top/gtvoafziyc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.chenlongwang.top/gtlzollmzo.html

[T34] Lua：遍历表
来源：http://hz.jiagoushi.top/gtbpgjtfcf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.9152youxi.cn/gtgqckgscw.html

[T35] Lua：字典表
来源：http://hz.hnqzz.top/gtqxjpzrdf.html

local d = { a = 1 };  d.b = 2
来源：http://hz.daxiang520.top/gtujcmdzsw.html

[T36] Lua：函数
来源：http://hz.birdmap.top/gtkhehoxge.html

function add(a, b) return a + b end
来源：http://hz.nanxinkj.top/gtpikgmgst.html

[T37] Lua：字符串拼接
来源：http://hz.zycfv.cn/gtewqemmnv.html

"a" .. "b"
来源：http://hz.hnqzz.top/gtsltgntpi.html

[T38] Lua：条件
来源：http://hz.svipenyu.cn/gtcscyqura.html

if x > 0 then print("正") end
来源：http://hz.yongpay.top/gtrxxizchc.html

[T39] Lua：模式匹配
来源：http://hz.guannengcc.top/gtcnvvzfid.html

string.find(s, "%d+")
来源：http://hz.hnqzz.top/gtfnwrpzoh.html

[T40] Lua：元表
来源：http://hz.ywan-chungtsiang.top/gtpnmeiynx.html

setmetatable({}, { __index = base })
来源：http://hz.hnxiangtu.top/gtulzpvanc.html

[T41] Perl：Hello World
来源：http://hz.chenlongwang.top/gtitlydmhw.html

print "Hello\n";
来源：http://hz.jinqigufen.top/gtzqienvxr.html

[T42] Perl：变量类型
来源：http://hz.aizwys.cn/gtalnoevsa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.chenzaomai.com/gtydvbxsmv.html

[T43] Perl：字符串插值
来源：http://hz.redwolf501.top/gtvjorizzn.html

"值: $a"
来源：http://hz.yongpay.top/gtgadpqher.html

[T44] Perl：条件
来源：http://hz.iojbl.cn/gtunfpgnav.html

if ($a > 0) { print "正"; }
来源：http://hz.gotoacloud.top/gtfgmofhug.html

[T45] Perl：数组遍历
来源：http://hz.yongpay.top/gtlbmeclnv.html

for my $x (@arr) { print $x; }
来源：http://hz.sweek.top/gtrbpjspse.html

[T46] Perl：哈希操作
来源：http://hz.yvedp.cn/gtgbvmxvpy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cqqwz.cn/gtbpuemhmi.html

[T47] Perl：正则捕获
来源：http://hz.sweek.top/gtjahkptgk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jyoumei.cn/gtnzulygiz.html

[T48] Perl：正则替换
来源：http://hz.sufxvd.cn/gtebynwrhi.html

$s =~ s/old/new/g;
来源：http://hz.zycfv.cn/gtmnragaal.html

[T49] Perl：函数
来源：http://hz.yongpay.top/gtmyjdwyjo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.aizwys.cn/gtwrywggxf.html

[T50] Perl：逐行读文件
来源：http://hz.pengpengdd.cyou/gtsthdhfqh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.316326.xyz/gtkeogzeqt.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.sysykeji.top/gthctodcak.html

[T51] Scala：Hello World
来源：http://hz.havefunace.top/gtrfkesyae.html

println("Hello")
来源：http://hz.snrcjt.cn/gtrezshdzy.html

[T52] Scala：变量
来源：http://hz.haohaochexian.top/gtihngvcqf.html

val a = 1;  var b = 2
来源：http://hz.hnqzz.top/gtoxhepsxw.html

[T53] Scala：字符串插值
来源：http://hz.zhijiandao.cn/gtpkmjvtmk.html

s"值: $b"
来源：http://hz.hfpthk.cn/gtcbsutker.html

[T54] Scala：集合映射
来源：http://hz.ehwqpu.com/gtrvffgusq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.daxiang520.top/gtavclmggv.html

[T55] Scala：集合过滤
来源：http://hz.ivvv.top/gtowxtxcbp.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hywenlv.cn/gtjssvbiyh.html

[T56] Scala：样例类
来源：http://hz.nanxinkj.top/gtzvvodhby.html

case class User(name: String, age: Int)
来源：http://hz.hongshengwenyu.top/gthtsgilqu.html

[T57] Scala：模式匹配
来源：http://hz.ehwqpu.com/gtjvrmgbjg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.pengpengdd.cyou/gtpxclsdpl.html

[T58] Scala：函数定义
来源：http://hz.wangshuangyany.cn/gtgxxfhiaq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.wangdashe.top/gtyhamjomk.html

[T59] Scala：循环
来源：http://hz.nwbrower.top/gtyhwviywa.html

for (i <- 1 to 10) println(i)
来源：http://hz.daria6918.cn/gtjblboevy.html

[T60] Scala：折叠
来源：http://hz.bjfxy.top/gtwlswoorh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.mhx1999.top/gtmhgvpbqp.html

================================================================================
来源：http://hz.nanxinkj.top/gtpnrmochr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinyuanbaomall.cn/gtzecttkep.html

================================================================================
来源：http://hz.gogol.net.cn/gtdezpauhk.html

[U01] Py：创建虚拟环境
来源：http://hz.tianlin.xyz/gtdfegmedl.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.feifeiyinyue.top/gtcefwohze.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jyoumei.cn/gtujxuppcl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yongpay.top/gtezacraiu.html

[U03] Py：加载 .env 配置
来源：http://hz.zhixingplan.top/gtqhkskekt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.9152youxi.cn/gtjqtggtfn.html

[U04] Py：变量调试打印
来源：http://hz.shanyushiyangtech.top/gtujaykswg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yangfankeji.com/gtcvbiauwq.html

[U05] Py：列表去重且保序
来源：http://hz.meibo888.top/gtcpelwvkl.html

list(dict.fromkeys(arr))
来源：http://hz.hammf.cn/gtyubkwmkg.html

[U06] Py：合并两个字典
来源：http://hz.wangshuangyany.cn/gtxyjsysxm.html

{**a, **b}
来源：http://hz.guannengcc.top/gtotnpzvsw.html

[U07] Py：反转字典键值
来源：http://hz.tianlin.xyz/gtzqdexzvr.html

{v: k for k, v in d.items()}
来源：http://hz.dianchejie.cn/gtbyqvhglr.html

[U08] Py：展平二维列表
来源：http://hz.9152youxi.cn/gtjjazgzpp.html

[y for x in nested for y in x]
来源：http://hz.gzhubu.top/gthmtxezrl.html

[U09] Py：字典取最大值的键
来源：http://hz.andypj.xyz/gticseqwjk.html

max(d, key=d.get)
来源：http://hz.ywan-chungtsiang.top/gticvwimtm.html

[U10] Py：按值排序字典
来源：http://hz.zdqjudy.top/gtoqkhvdnn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.guowangkeji.top/gtelvxmyme.html

[U11] Py：生成器表达式
来源：http://hz.guowangkeji.top/gtruusmzfh.html

(x * 2 for x in arr)
来源：http://hz.zhoulong.xyz/gtbgrjblyv.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.jiagoushi.top/gtezzukjhe.html

Counter(arr).most_common(3)
来源：http://hz.jqgfzy.top/gtmlvpppvt.html

[U13] Py：固定长度队列
来源：http://hz.cucudq.cn/gtltyoovjn.html

deque(maxlen=10)
来源：http://hz.aibaodan.cn/gtvngnmprc.html

[U14] Py：分组收集到列表
来源：http://hz.birdmap.top/gtrdicdvgd.html

defaultdict(list)
来源：http://hz.andypj.xyz/gtssxazzkt.html

[U15] Py：高精度计时
来源：http://hz.xinyue.icu/gtxgqadqes.html

t = time.perf_counter()
来源：http://hz.jianghu66.top/gtsatukylc.html

[U16] Py：命令行参数解析
来源：http://hz.hywenlv.cn/gticujvptr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.daria6918.cn/gtiemblhqe.html

[U17] Py：初始化日志
来源：http://hz.chenzaomai.com/gteotvryem.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.cdnleiting.top/gtnhvtyvrt.html

[U18] Py：预编译正则
来源：http://hz.mhx1999.top/gtoqblfhhz.html

pat = re.compile(r"\d+")
来源：http://hz.gzhubu.top/gtpqgqnrsp.html

[U19] Py：正则替换带回调
来源：http://hz.jinghuilouyu.cn/gtebreptnm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.shuidangran.top/gtczntujal.html

[U20] Py：缓存函数结果
来源：http://hz.yongpay.top/gtbzofckdg.html

@functools.lru_cache(maxsize=None)
来源：http://hz.wangshuangyany.cn/gtssqlzmpe.html

[U21] Py：自定义上下文管理器
来源：http://hz.zdqjudy.top/gtyjpzhpqb.html

@contextlib.contextmanager
来源：http://hz.xylfe.cn/gtlkopgxef.html

[U22] Py：矩阵转置
来源：http://hz.wangshuangyany.cn/gtugaufyyu.html

list(zip(*m))
来源：http://hz.pycfn.com/gtorkqidwn.html

[U23] Py：分块读取大文件
来源：http://hz.zhaomingkeji.xyz/gtmpgmudaz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhijiandao.cn/gtxtmxjxop.html

[U24] Py：路径操作
来源：http://hz.ehwqpu.com/gtabovycpy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zhiwuduotai.top/gtzuexighm.html

[U25] Py：CSV 按字典读
来源：http://hz.xziqi.cn/gtalalmhow.html

csv.DictReader(f)
来源：http://hz.mhx1999.top/gtbnzkmwnh.html

[U26] Py：并发下载
来源：http://hz.sxryk.cn/gttjduwkjy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.yonumen.top/gtxzskrlgt.html

[U27] Py：异步 HTTP
来源：http://hz.daria6918.cn/gtbcjxuibq.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.kuanghao11.cn/gtgyoqqdia.html

[U28] Py：类型别名
来源：http://hz.snrcjt.cn/gtnninetxt.html

UserId = int
来源：http://hz.shanyushiyangkeji.top/gtcsvmabta.html

[U29] Py：属性校验
来源：http://hz.zdqjudy.top/gtdtdgaayh.html

@property 与 @x.setter 配合
来源：http://hz.hywenlv.cn/gtinoagjuc.html

[U30] Py：数据类
来源：http://hz.chenzaomai.com/gtdhyglpuw.html

@dataclass(slots=True)
来源：http://hz.sufxvd.cn/gthnzkbvrr.html

[U31] Py：单测
来源：http://hz.jiagoushi.top/gtkwaouvnn.html

python -m pytest -q
来源：http://hz.meibo888.top/gtfqywzgrr.html

[U32] Py：代码格式化
来源：http://hz.xylfe.cn/gtdklagyoc.html

ruff format . && ruff check --fix .
来源：http://hz.jianghu66.top/gtoqudxcho.html

[U33] Py：打包发布
来源：http://hz.gaohongyu789.top/gtagbkpdjg.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.316326.xyz/gtuudmspkm.html

[U34] Py：判断编码
来源：http://hz.hongshengwenyu.top/gtucnrvmdq.html

chardet.detect(raw)
来源：http://hz.zhaomingkeji.xyz/gtihtkzjrn.html

[U35] Py：发送邮件
来源：http://hz.ywan-chungtsiang.top/gtoltohlsf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sweek.top/gtauuiygxk.html

[U36] Py：定时任务
来源：http://hz.shuidangran.top/gtvnyvivef.html

schedule.every(10).minutes.do(job)
来源：http://hz.dashuyun.cn/gtfpvkcens.html

[U37] Py：读写 Excel
来源：http://hz.hnxiangtu.top/gtcbykkxiw.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.tanke756.top/gtgqxhecnt.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhengqikj.top/gtwchojune.html

Path(__file__).resolve().parent
来源：http://hz.guannengcc.top/gtqvwyamzh.html

[U39] Py：判断是否在交互环境
来源：http://hz.ydjk.org.cn/gtobkwhmps.html

sys.stdout.isatty()
来源：http://hz.wangdashe.top/gtzchseuys.html

[U40] Py：打印到标准错误
来源：http://hz.guannengcc.top/gtfuemjlde.html

print("err", file=sys.stderr)
来源：http://hz.iojbl.cn/gttbniswsp.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.nanxinkj.top/gtdlfevqvd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.meibo888.top/gtiudbdajd.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.aizwys.cn/gtziertqxz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.sxryk.cn/gtuvqambqr.html

[U43] PHP：声明命名空间
来源：http://hz.jinqigfzy.top/gtodclkcob.html

namespace App\Http;
来源：http://hz.hongshengwenyu.top/gtmnmauzpg.html

[U44] PHP：开启严格类型
来源：http://hz.jqgfzy.top/gtjthlzgbm.html

declare(strict_types=1);
来源：http://hz.zhoulong.xyz/gtsqfycywt.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yuanzhike.top/gtgpboxjxl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gtykiqzczy.html

[U46] PHP：可空类型
来源：http://hz.ydjk.org.cn/gtbbnzyjcr.html

?string $name = null
来源：http://hz.iojbl.cn/gtureqlboy.html

[U47] PHP：联合类型
来源：http://hz.ybcxt.top/gttxqldrum.html

int|string $id
来源：http://hz.c1oappe.top/gtedirghsy.html

[U48] PHP：纯枚举
来源：http://hz.gogol.net.cn/gtobktimjt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.c1oappe.top/gtzneaspli.html


<!-- 参考信息 -->