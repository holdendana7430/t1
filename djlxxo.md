代发 wailian999

[S33] C++：vector 增删
来源：http://hz.birdmap.top/gtatqgbdhi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hysaishi.cn/gtfhffjgsd.html

[S34] C++：遍历 vector
来源：http://hz.yongpay.top/gtpncyszjm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shuidangran.top/gthwufkygp.html

[S35] C++：map
来源：http://hz.hnxiangtu.top/gtnktckudg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gtkoctijgh.html

[S36] C++：unordered_map
来源：http://hz.redwolf501.top/gtoovtdkxe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.andypj.xyz/gtdizjsgmz.html

[S37] C++：set
来源：http://hz.sxryk.cn/gttemyjldb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shuidangran.top/gtqlhjhrcu.html

[S38] C++：排序
来源：http://hz.birdmap.top/gtxpcwoivf.html

std::sort(v.begin(), v.end());
来源：http://hz.chenjidiqi.icu/gtdauuzyll.html

[S39] C++：自定义比较器排序
来源：http://hz.dianchejie.cn/gtwszcxcpy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenzaomai.com/gtwgtgdend.html

[S40] C++：查找元素
来源：http://hz.cdnleiting.top/gtmzrnjwga.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.fzhhl.top/gtlpgkaqeh.html

[S41] C++：类与构造函数
来源：http://hz.bjfxy.top/gtgaomurmz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nanxinkj.top/gtehvjfarz.html

[S42] C++：继承与虚函数
来源：http://hz.quarkkingdee.top/gtxxmdtgwa.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhijiandao.cn/gtcmueccgi.html

[S43] C++：智能指针
来源：http://hz.chenjidiqi.icu/gtugnuzqdq.html

auto p = std::make_unique<int>(5);
来源：http://hz.havefunace.top/gtounqybhy.html

[S44] C++：引用传参
来源：http://hz.jinghuilouyu.cn/gtahflmxfi.html

void inc(int &x) { ++x; }
来源：http://hz.vqdsnc.cn/gtzujdwdde.html

[S45] C++：lambda
来源：http://hz.yonumen.top/gtzeldugjt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenlongwang.top/gtmdkcgodo.html

[S46] C++：函数模板
来源：http://hz.gaohongyu789.top/gtgicjmino.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jianghu66.top/gtomguirqv.html

[S47] C++：结构化绑定遍历
来源：http://hz.gotoacloud.top/gtmozlbwnn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.c1oappe.top/gtqhsdqdtr.html

[S48] C++：逐行读文件
来源：http://hz.ydzc1.top/gtkztpndrc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhijiandao.cn/gtwajcbpcw.html

while (std::getline(in, line)) { }
来源：http://hz.hammf.cn/gtsyrmsgmg.html

[S49] C++：写文件
来源：http://hz.aizwys.cn/gtbtpmsbus.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gtpgrznrxk.html

[S50] C++：格式化数字
来源：http://hz.jinqigfzy.top/gtpyzqmxxj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cqqwz.cn/gticqwwcxp.html

[S51] C++：显式类型转换
来源：http://hz.yj20258.top/gtwuvobjgk.html

static_cast<double>(a) / b
来源：http://hz.fengsongda.top/gtokvmvxbm.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gtmdxwczzr.html

int size() const noexcept { return n_; }
来源：http://hz.cheryme.top/gttclcfnxn.html

[S53] C++：移动语义
来源：http://hz.jinqigfzy.top/gtytkcpibr.html

std::vector<int> w = std::move(v);
来源：http://hz.jyoumei.cn/gtxayhbanv.html

[S54] C++：异常处理
来源：http://hz.chenlongwang.top/gtsyvworhv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.snrcjt.cn/gtqswhjidy.html

[S55] C++：结构化绑定
来源：http://hz.52xcode.cn/gtmqkjxuyt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinghuilouyu.cn/gtzozaxgwx.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gtoqbgoxga.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.smart0.xyz/gtwxiswhqe.html

[S57] C++：编译期常量
来源：http://hz.mhx1999.top/gthoosqkwk.html

constexpr int N = 10;
来源：http://hz.kuanghao11.cn/gtthuqejvd.html

[S58] C++：命名空间
来源：http://hz.yuanzhike.top/gttqcgypgv.html

namespace ns { int f() { return 1; } }
来源：http://hz.ydjk.org.cn/gtvhywyima.html

[S59] C++：静态断言
来源：http://hz.fengsongda.top/gtfyqhtifz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zdqjudy.top/gtyvnnzwbw.html

[S60] C++：遍历并删除元素
来源：http://hz.sweek.top/gtptvztiiv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.andypj.xyz/gthrsegebd.html

================================================================================
来源：http://hz.jqgufenzy.top/gtkprvrieu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.haohaochexian.top/gtmzpfuctf.html

================================================================================
来源：http://hz.yj202588.top/gtrhhdhyys.html

[T01] Kotlin：Hello World
来源：http://hz.gogol.net.cn/gtlvlbqeyq.html

println("Hello")
来源：http://hz.ydjk.org.cn/gtvzgwjacb.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtpmpbumal.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.kuanghao11.cn/gtmmbkcxoo.html

[T03] Kotlin：字符串模板
来源：http://hz.nwbrower.top/gtthtinryc.html

"值: $b"
来源：http://hz.fzhhl.top/gtskgursov.html

[T04] Kotlin：空安全
来源：http://hz.nanxuanxn.top/gtsqabluhh.html

val n: String? = null;  n?.length
来源：http://hz.cdnleiting.top/gtvrbnvtck.html

[T05] Kotlin：when 表达式
来源：http://hz.zhijiandao.cn/gtsjjlrthm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.c1oappe.top/gtehyubvjy.html

[T06] Kotlin：集合映射
来源：http://hz.sweek.top/gtghdiripc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.fengsongda.top/gtnzvnnjnf.html

[T07] Kotlin：集合过滤
来源：http://hz.wangdashe.top/gtdspdowni.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shzxlz.cn/gtgvfogqiw.html

[T08] Kotlin：数据类
来源：http://hz.zhengqikj.top/gtdsblnyyk.html

data class User(val name: String, val age: Int)
来源：http://hz.tianlin.xyz/gtlimtbwhb.html

[T09] Kotlin：扩展函数
来源：http://hz.haohaochexian.top/gtdfbuprmf.html

fun String.exclaim() = this + "!"
来源：http://hz.ybcxt.top/gttpivgolc.html

[T10] Kotlin：默认参数
来源：http://hz.fzhhl.top/gtzvuuqyqx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sufxvd.cn/gtzqoqkwjf.html

[T11] Kotlin：协程
来源：http://hz.chenlongwang.top/gtxyytqbry.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ywan-chungtsiang.top/gtxopmenzd.html

[T12] Kotlin：解构声明
来源：http://hz.ivvv.top/gtvrnovjmi.html

val (a, b) = Pair(1, 2)
来源：http://hz.cucudq.cn/gtzdibjvaj.html

[T13] Kotlin：只读 Map
来源：http://hz.jianghu66.top/gtibjegtip.html

val m = mapOf("a" to 1)
来源：http://hz.hongshengwenyu.top/gteszktkah.html

[T14] Kotlin：循环
来源：http://hz.smart0.xyz/gtjczspbcx.html

for (i in 1..10) println(i)
来源：http://hz.cdnleiting.top/gtrfvhzkoh.html

[T15] Kotlin：接口
来源：http://hz.svipenyu.cn/gtonjgisen.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtncxqslwa.html

[T16] Swift：Hello World
来源：http://hz.ywan-chungtsiang.top/gtobdfqkhv.html

print("Hello")
来源：http://hz.gotoacloud.top/gtkulnyuwc.html

[T17] Swift：变量与常量
来源：http://hz.pengpengdd.cyou/gtfcdvfwgp.html

var a = 1;  let b = 2
来源：http://hz.havefunace.top/gtxfmafxro.html

[T18] Swift：字符串插值
来源：http://hz.kuanghao11.cn/gtbdjxvzat.html

"值: \(b)"
来源：http://hz.chenzaomai.com/gtbjfdziwl.html

[T19] Swift：可选绑定
来源：http://hz.andypj.xyz/gtjlorddcu.html

if let n = opt { print(n) }
来源：http://hz.yvedp.cn/gtquuhlkgu.html

[T20] Swift：数组操作
来源：http://hz.guowangkeji.top/gtqpjvzyht.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ybcxt.top/gttcbhuopw.html

[T21] Swift：遍历
来源：http://hz.pengpengdd.cyou/gtrzunraqu.html

for x in a { print(x) }
来源：http://hz.pycfn.com/gtvppcoxlh.html

[T22] Swift：字典
来源：http://hz.yongpay.top/gtagukrcax.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hfpthk.cn/gtbxyrazgp.html

[T23] Swift：函数
来源：http://hz.jinqigufen.top/gtilsiiqao.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ehwqpu.com/gtsfpirnaf.html

[T24] Swift：闭包
来源：http://hz.mhx1999.top/gtynvydxkb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yvedp.cn/gtrqgbdxfw.html

[T25] Swift：结构体
来源：http://hz.jyoumei.cn/gtccxwkhqp.html

struct P { var x: Int }
来源：http://hz.yanxiufei.cn/gtstjtadei.html

[T26] Swift：类与重写
来源：http://hz.ydzc1.top/gtobaptkde.html

class A: Base { override func f() {} }
来源：http://hz.shanyushiyangkeji.top/gtjnxfsbbe.html

[T27] Swift：错误处理
来源：http://hz.wangshuangyany.cn/gtjberxsfy.html

do { try f() } catch { print(error) }
来源：http://hz.gaohongyu789.top/gtgdloqhss.html

[T28] Swift：枚举
来源：http://hz.52xcode.cn/gtylftcmsa.html

enum Color { case red, green }
来源：http://hz.gaohongyu789.top/gtexmmdjyh.html

[T29] Swift：guard 提前返回
来源：http://hz.jqgufenzy.top/gtpfhhhpxb.html

guard let x = opt else { return }
来源：http://hz.andypj.xyz/gthwsvnbeu.html

[T30] Swift：协议
来源：http://hz.gaohongyu789.top/gtxayflwah.html

protocol Shape { func area() -> Double }
来源：http://hz.tianlin.xyz/gtuqqkfbrp.html

[T31] Lua：Hello World
来源：http://hz.shuidangran.top/gtsvtvtivz.html

print("Hello")
来源：http://hz.chenlongwang.top/gtgnrkdksn.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gtscltaspe.html

local a = 1
来源：http://hz.9152youxi.cn/gteegkxenn.html

[T33] Lua：表（数组）
来源：http://hz.zhixingplan.top/gtmeosogbo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj202588.top/gtvqqxvpmj.html

[T34] Lua：遍历表
来源：http://hz.gotoacloud.top/gthrvmjuqk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xingfuxueyuan.xyz/gtvolckjxc.html

[T35] Lua：字典表
来源：http://hz.ydzc1.top/gtawxfcqwl.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sxryk.cn/gtaqxuikng.html

[T36] Lua：函数
来源：http://hz.aizwys.cn/gtsbpwvgct.html

function add(a, b) return a + b end
来源：http://hz.9152youxi.cn/gtuvswhvsu.html

[T37] Lua：字符串拼接
来源：http://hz.9152youxi.cn/gtnrmjuvwi.html

"a" .. "b"
来源：http://hz.shanyushiyangkeji.top/gttnirsdex.html

[T38] Lua：条件
来源：http://hz.sxryk.cn/gtmtrdhknv.html

if x > 0 then print("正") end
来源：http://hz.sufxvd.cn/gtzedhqwgy.html

[T39] Lua：模式匹配
来源：http://hz.hongshengwenyu.top/gtgkaenmcr.html

string.find(s, "%d+")
来源：http://hz.dashuyun.cn/gthqhyxtpj.html

[T40] Lua：元表
来源：http://hz.daxiang520.top/gtsmbcalth.html

setmetatable({}, { __index = base })
来源：http://hz.gzhubu.top/gtrlywoipv.html

[T41] Perl：Hello World
来源：http://hz.yuanzhike.top/gtsixhvisa.html

print "Hello\n";
来源：http://hz.xylfe.cn/gtfaranski.html

[T42] Perl：变量类型
来源：http://hz.xinyue.icu/gtmtlplncj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgufenzy.top/gthiepxvtn.html

[T43] Perl：字符串插值
来源：http://hz.yj20258.top/gtmuwxtfew.html

"值: $a"
来源：http://hz.jinqigfzy.top/gttnznjdel.html

[T44] Perl：条件
来源：http://hz.dashuyun.cn/gtqrdjrknd.html

if ($a > 0) { print "正"; }
来源：http://hz.daxiang520.top/gtqqktfljp.html

[T45] Perl：数组遍历
来源：http://hz.shangyingyoupin.top/gtrnxvmdof.html

for my $x (@arr) { print $x; }
来源：http://hz.svipenyu.cn/gtdtotgrve.html

[T46] Perl：哈希操作
来源：http://hz.daxiang520.top/gtzddcpqtv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ydjk.org.cn/gtwxabpdmf.html

[T47] Perl：正则捕获
来源：http://hz.ydjk.org.cn/gtvjlcxzyw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cqqwz.cn/gtuzjgxrhc.html

[T48] Perl：正则替换
来源：http://hz.jyoumei.cn/gtqrnxajsj.html

$s =~ s/old/new/g;
来源：http://hz.c1oappe.top/gtrwetejnd.html

[T49] Perl：函数
来源：http://hz.gaohongyu789.top/gtxmmpxxim.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jyoumei.cn/gttqlpbyqp.html

[T50] Perl：逐行读文件
来源：http://hz.0kj1m.cn/gtnueyjxqp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.mhx1999.top/gtjxggpert.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.9152youxi.cn/gtcirrowuk.html

[T51] Scala：Hello World
来源：http://hz.ehwqpu.com/gtnbonnezz.html

println("Hello")
来源：http://hz.zhaomingkeji.xyz/gtpobdmyks.html

[T52] Scala：变量
来源：http://hz.pycfn.com/gtlilercpr.html

val a = 1;  var b = 2
来源：http://hz.jinyuanbaomall.cn/gtiozlqahb.html

[T53] Scala：字符串插值
来源：http://hz.aizwys.cn/gtujrumvxr.html

s"值: $b"
来源：http://hz.xuetiantiany.cn/gtehqplgua.html

[T54] Scala：集合映射
来源：http://hz.mhx1999.top/gtnzzhkcxy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhixingplan.top/gtvhewbutj.html

[T55] Scala：集合过滤
来源：http://hz.jyoumei.cn/gtstngutka.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.hnxiangtu.top/gtqtgbnhqp.html

[T56] Scala：样例类
来源：http://hz.cheryme.top/gtivmvvyjw.html

case class User(name: String, age: Int)
来源：http://hz.ehwqpu.com/gtgylkvcbj.html

[T57] Scala：模式匹配
来源：http://hz.cqqwz.cn/gttpzgrhhk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinghuilouyu.cn/gtkscffchl.html

[T58] Scala：函数定义
来源：http://hz.gotoacloud.top/gtkvnnhpjl.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhaomingkeji.xyz/gthfetgjpt.html

[T59] Scala：循环
来源：http://hz.xuanzx.com/gtfhwwwxge.html

for (i <- 1 to 10) println(i)
来源：http://hz.nwbrower.top/gttxaxzzlk.html

[T60] Scala：折叠
来源：http://hz.ybcxt.top/gtnacknfkr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hfpthk.cn/gtvpliatbu.html

================================================================================
来源：http://hz.ppjwa.cn/gtfvpblabr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hysaishi.cn/gtjktdppub.html

================================================================================
来源：http://hz.hammf.cn/gtazpdswzh.html

[U01] Py：创建虚拟环境
来源：http://hz.jinyuanbaomall.cn/gtlcefrllx.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.ybcxt.top/gtvqurgylg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.chenzaomai.com/gtzsftpseq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yuanzhike.top/gtdfhlazuq.html

[U03] Py：加载 .env 配置
来源：http://hz.aizwys.cn/gtdwyqyjbw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.fengsongda.top/gtkdoqngvp.html

[U04] Py：变量调试打印
来源：http://hz.quarkkingdee.top/gtqjdelgvg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.52xcode.cn/gtmgjqkwly.html

[U05] Py：列表去重且保序
来源：http://hz.aibaodan.cn/gtycdvlylz.html

list(dict.fromkeys(arr))
来源：http://hz.quarkkingdee.top/gtvbuyvwqe.html

[U06] Py：合并两个字典
来源：http://hz.ywan-chungtsiang.top/gtrbcctcki.html

{**a, **b}
来源：http://hz.zhixingplan.top/gtedoxitqz.html

[U07] Py：反转字典键值
来源：http://hz.jqgufenzy.top/gtmwbeflqi.html

{v: k for k, v in d.items()}
来源：http://hz.yuxming.cn/gtwgpoumci.html

[U08] Py：展平二维列表
来源：http://hz.pengpengdd.cyou/gttbbakrhe.html

[y for x in nested for y in x]
来源：http://hz.zhoulong.xyz/gtydloauux.html

[U09] Py：字典取最大值的键
来源：http://hz.sufxvd.cn/gtiqdfjjlb.html

max(d, key=d.get)
来源：http://hz.hnxiangtu.top/gtzqqnnpiz.html

[U10] Py：按值排序字典
来源：http://hz.tianlin.xyz/gtoqgoysml.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.wangshuangyany.cn/gtfgzzplio.html

[U11] Py：生成器表达式
来源：http://hz.gogol.net.cn/gtjhrishdd.html

(x * 2 for x in arr)
来源：http://hz.jqgufenzy.top/gtoqbzmugw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhengqikj.top/gtgdukaihl.html

Counter(arr).most_common(3)
来源：http://hz.316326.xyz/gtkylysxat.html

[U13] Py：固定长度队列
来源：http://hz.hnqzz.top/gtfikkeclj.html

deque(maxlen=10)
来源：http://hz.hongshengwenyu.top/gtqmjczwmn.html

[U14] Py：分组收集到列表
来源：http://hz.nanxuanxn.top/gtuughslzh.html

defaultdict(list)
来源：http://hz.sweek.top/gtparnlcxp.html

[U15] Py：高精度计时
来源：http://hz.ywan-chungtsiang.top/gtqremiryz.html

t = time.perf_counter()
来源：http://hz.yuxming.cn/gtwtxrjigz.html

[U16] Py：命令行参数解析
来源：http://hz.dashuyun.cn/gtlqlcnvar.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhongyouzk.top/gtrlfpiftn.html

[U17] Py：初始化日志
来源：http://hz.nwbrower.top/gtncuwugmf.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jinyuanbaomall.cn/gtoxponsux.html

[U18] Py：预编译正则
来源：http://hz.chenlongwang.top/gtklekoeyk.html

pat = re.compile(r"\d+")
来源：http://hz.aibaodan.cn/gtrwkkzvzh.html

[U19] Py：正则替换带回调
来源：http://hz.yj202588.top/gtujzdclsl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hnxiangtu.top/gtfxaguwjm.html

[U20] Py：缓存函数结果
来源：http://hz.yj20258.top/gtsntjcufu.html

@functools.lru_cache(maxsize=None)
来源：http://hz.mhx1999.top/gtgozpmepv.html

[U21] Py：自定义上下文管理器
来源：http://hz.nwbrower.top/gtrfnatvxa.html

@contextlib.contextmanager
来源：http://hz.pycfn.com/gtcgipxdtt.html

[U22] Py：矩阵转置
来源：http://hz.tanke756.top/gtwyaaoxfa.html

list(zip(*m))
来源：http://hz.aibaodan.cn/gtquwedpya.html

[U23] Py：分块读取大文件
来源：http://hz.gzhubu.top/gtcevysrqz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.gogol.net.cn/gtskturvux.html

[U24] Py：路径操作
来源：http://hz.chenlongwang.top/gtgqovsyne.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.haohaochexian.top/gtsewdbfhx.html

[U25] Py：CSV 按字典读
来源：http://hz.0kj1m.cn/gtstutqzab.html

csv.DictReader(f)
来源：http://hz.zhixingplan.top/gtrfvaggok.html

[U26] Py：并发下载
来源：http://hz.fzhhl.top/gtrrmuazkn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhengqikj.top/gtthzjqwbb.html

[U27] Py：异步 HTTP
来源：http://hz.wangshuangyany.cn/gtuvbomfqk.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sufxvd.cn/gtzwszpytt.html

[U28] Py：类型别名
来源：http://hz.yonumen.top/gtbljbvjwe.html

UserId = int
来源：http://hz.ivvv.top/gtvjmeezso.html

[U29] Py：属性校验
来源：http://hz.zhongyouzk.top/gtxnpwqerg.html

@property 与 @x.setter 配合
来源：http://hz.hysaishi.cn/gthexkxmrk.html

[U30] Py：数据类
来源：http://hz.hfpthk.cn/gtqrsbefdk.html

@dataclass(slots=True)
来源：http://hz.dashuyun.cn/gtuqdyjxzv.html

[U31] Py：单测
来源：http://hz.pengpengdd.cyou/gtaqealmmm.html

python -m pytest -q
来源：http://hz.tanke756.top/gtlwrhonsm.html

[U32] Py：代码格式化
来源：http://hz.pengpengdd.cyou/gthbjudxtw.html

ruff format . && ruff check --fix .
来源：http://hz.snrcjt.cn/gtidtlnaol.html

[U33] Py：打包发布
来源：http://hz.xziqi.cn/gtooohhipp.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.sufxvd.cn/gthzdeeqdj.html

[U34] Py：判断编码
来源：http://hz.zycfv.cn/gtldbmrgon.html

chardet.detect(raw)
来源：http://hz.aibaodan.cn/gtizdvbail.html

[U35] Py：发送邮件
来源：http://hz.daria6918.cn/gtthgwvbth.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xziqi.cn/gtjxgpjuxf.html

[U36] Py：定时任务
来源：http://hz.birdmap.top/gtkthnljxw.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhongyouzk.top/gtzutehevb.html

[U37] Py：读写 Excel
来源：http://hz.chenzaomai.com/gtqskvynml.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jlsjyb.cn/gtzcpwqkjp.html

[U38] Py：获取脚本所在目录
来源：http://hz.jlsjyb.cn/gtehbsxebz.html

Path(__file__).resolve().parent
来源：http://hz.hywenlv.cn/gtwasemwvn.html

[U39] Py：判断是否在交互环境
来源：http://hz.yangfankeji.com/gtfchaowca.html

sys.stdout.isatty()
来源：http://hz.dashuyun.cn/gtwloqtgaq.html

[U40] Py：打印到标准错误
来源：http://hz.yangfankeji.com/gtozssiplf.html

print("err", file=sys.stderr)
来源：http://hz.guowangkeji.top/gtemsnajro.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.c1oappe.top/gtiihhdalb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.pengpengdd.cyou/gtucqqnaoe.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.smart0.xyz/gtlbebrkhl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gaohongyu789.top/gtmnvpcxzn.html

[U43] PHP：声明命名空间
来源：http://hz.yongpay.top/gtubkmrepf.html

namespace App\Http;
来源：http://hz.yongpay.top/gtzeizgjco.html

[U44] PHP：开启严格类型
来源：http://hz.jlsjyb.cn/gtuxtcgkai.html

declare(strict_types=1);
来源：http://hz.jqgfzy.top/gtqztjwgdi.html

[U45] PHP：类型声明与返回类型
来源：http://hz.wangshuangyany.cn/gtghhvlgjt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gtuiainjij.html

[U46] PHP：可空类型
来源：http://hz.cucudq.cn/gtidrecowk.html

?string $name = null
来源：http://hz.ywan-chungtsiang.top/gtnnpdbqoe.html

[U47] PHP：联合类型
来源：http://hz.daxiang520.top/gtbpgbhfdi.html

int|string $id
来源：http://hz.daria6918.cn/gtclcqraas.html

[U48] PHP：纯枚举
来源：http://hz.meibo888.top/gtiwonyopi.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yonumen.top/gtersigxoe.html

[U49] PHP：只读属性
来源：http://hz.xylfe.cn/gtidolxsjp.html

public readonly string $name
来源：http://hz.aizwys.cn/gtchrgrcij.html

[U50] PHP：构造器属性提升
来源：http://hz.ydjk.org.cn/gtxvazagrd.html

public function __construct(private int $id) {}
来源：http://hz.jyoumei.cn/gtlssidmvd.html

[U51] PHP：数组解构
来源：http://hz.jqgufenzy.top/gttpklsqon.html

[$a, $b] = $arr;
来源：http://hz.birdmap.top/gtmewhiotu.html

[U52] PHP：箭头函数
来源：http://hz.sweek.top/gtumtvadyk.html

$double = fn($x) => $x * 2;
来源：http://hz.zhengqikj.top/gtgfhtpbpz.html

[U53] PHP：空合并运算符
来源：http://hz.ydjk.org.cn/gtiliwkxox.html

$v = $a ?? $b ?? "default";
来源：http://hz.52xcode.cn/gtguqrcucx.html

[U54] PHP：空安全调用
来源：http://hz.gogol.net.cn/gtqvprqpkr.html

$obj?->method()
来源：http://hz.yueranfly.top/gtgatzxqpt.html

[U55] PHP：match 表达式
来源：http://hz.yj202588.top/gtubgvyzpd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.gotoacloud.top/gteatcfzbg.html

[U56] PHP：命名参数
来源：http://hz.xuanzx.com/gtoqkynwfu.html

f(a: 1, b: 2)
来源：http://hz.zhengqikj.top/gtkaklqlxc.html

[U57] PHP：字符串插值
来源：http://hz.hfpthk.cn/gtytgmnllz.html

"值: {$a}"
来源：http://hz.tian-w.cn/gtqzmkbrkp.html

[U58] PHP：数组三件套
来源：http://hz.zycfv.cn/gtgucwzywr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.havefunace.top/gtggfesqak.html


<!-- 参考信息 -->