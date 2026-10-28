代发 wailian999

[S35] C++：map
来源：http://hz.aibaodan.cn/gtvdkcmmpy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gturxydvpz.html

[S36] C++：unordered_map
来源：http://hz.52xcode.cn/gtmnthrmpe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yvedp.cn/gtfxnjmmja.html

[S37] C++：set
来源：http://hz.aibaodan.cn/gtghfabrsr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gaohongyu789.top/gtmccvlzon.html

[S38] C++：排序
来源：http://hz.yj202588.top/gtxmahqhcy.html

std::sort(v.begin(), v.end());
来源：http://hz.dashuyun.cn/gttvvtgfse.html

[S39] C++：自定义比较器排序
来源：http://hz.zhengqikj.top/gtkcbkpbci.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.mhx1999.top/gtgkkxcyyc.html

[S40] C++：查找元素
来源：http://hz.pengpengdd.cyou/gtncrcfckh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guowangkeji.top/gthldkttgt.html

[S41] C++：类与构造函数
来源：http://hz.ehwqpu.com/gtqdhimjfi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.aizwys.cn/gtpsinycez.html

[S42] C++：继承与虚函数
来源：http://hz.nwbrower.top/gtxeqcvauc.html

class B : public Base { public: void f() override {} };
来源：http://hz.yongpay.top/gtyorinwhe.html

[S43] C++：智能指针
来源：http://hz.ppjwa.cn/gtogjizcsx.html

auto p = std::make_unique<int>(5);
来源：http://hz.jqgfzy.top/gtyritpiiw.html

[S44] C++：引用传参
来源：http://hz.shangyingyoupin.top/gttgzikvcd.html

void inc(int &x) { ++x; }
来源：http://hz.jyoumei.cn/gtyciynbkb.html

[S45] C++：lambda
来源：http://hz.yj202588.top/gtejkfmuuq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.fzhhl.top/gtcnvuqywy.html

[S46] C++：函数模板
来源：http://hz.kuanghao11.cn/gtvpzbberb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ydzc1.top/gtvxaekvuz.html

[S47] C++：结构化绑定遍历
来源：http://hz.aizwys.cn/gtzxxvvuqx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cashguo.top/gtaqimcuft.html

[S48] C++：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtqcxrrjis.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yueranfly.top/gtkvswzdff.html

while (std::getline(in, line)) { }
来源：http://hz.xuanzx.com/gtkgffcvfg.html

[S49] C++：写文件
来源：http://hz.fzhhl.top/gtyohasyhy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jlsjyb.cn/gtchjvyjbi.html

[S50] C++：格式化数字
来源：http://hz.redwolf501.top/gtqohrygde.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxinkj.top/gtnmjxhkcf.html

[S51] C++：显式类型转换
来源：http://hz.jlsjyb.cn/gticdszvlh.html

static_cast<double>(a) / b
来源：http://hz.nanxinkj.top/gtirxberem.html

[S52] C++：const 与 noexcept
来源：http://hz.meibo888.top/gtudlnkdof.html

int size() const noexcept { return n_; }
来源：http://hz.fengsongda.top/gtxdazmcms.html

[S53] C++：移动语义
来源：http://hz.haohaochexian.top/gthormqlya.html

std::vector<int> w = std::move(v);
来源：http://hz.yueranfly.top/gtjijurlnb.html

[S54] C++：异常处理
来源：http://hz.nanxinkj.top/gthxjlpmkg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhiwuduotai.top/gtfynqfzma.html

[S55] C++：结构化绑定
来源：http://hz.zhiwuduotai.top/gtagqvhoqb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cashguo.top/gtexgmfvmr.html

[S56] C++：optional
来源：http://hz.xylfe.cn/gtfhxacfcj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cdnleiting.top/gtqmunxton.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gtopcqlaft.html

constexpr int N = 10;
来源：http://hz.daria6918.cn/gtwvpneimf.html

[S58] C++：命名空间
来源：http://hz.zhixingplan.top/gttumkwsmr.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj20258888.top/gtxrnlhmre.html

[S59] C++：静态断言
来源：http://hz.guannengcc.top/gttacwndjl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gaohongyu789.top/gtiuwajsqe.html

[S60] C++：遍历并删除元素
来源：http://hz.ywan-chungtsiang.top/gtqhszcpwd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yvedp.cn/gtalkcuauq.html

================================================================================
来源：http://hz.yueranfly.top/gtkifokgoy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.quarkkingdee.top/gtbtbdoier.html

================================================================================
来源：http://hz.snrcjt.cn/gtdtcmvefu.html

[T01] Kotlin：Hello World
来源：http://hz.yongpay.top/gtrxcprzxh.html

println("Hello")
来源：http://hz.sweek.top/gtopajbfhr.html

[T02] Kotlin：变量
来源：http://hz.pengpengdd.cyou/gtzrygogkr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.redwolf501.top/gtggvlaprm.html

[T03] Kotlin：字符串模板
来源：http://hz.daria6918.cn/gtmrohjpam.html

"值: $b"
来源：http://hz.tianlin.xyz/gtimhoglda.html

[T04] Kotlin：空安全
来源：http://hz.jinghuilouyu.cn/gttjwbuqic.html

val n: String? = null;  n?.length
来源：http://hz.chenlongwang.top/gtyozxzjel.html

[T05] Kotlin：when 表达式
来源：http://hz.aizwys.cn/gtovtjbvlr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuanzhike.top/gtgeaibioq.html

[T06] Kotlin：集合映射
来源：http://hz.haohaochexian.top/gtnqgpzqdd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangshuangyany.cn/gtzvkfcknn.html

[T07] Kotlin：集合过滤
来源：http://hz.fzhhl.top/gtcojwqskj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gogol.net.cn/gtcbtnviqj.html

[T08] Kotlin：数据类
来源：http://hz.nwbrower.top/gtozqhvfhs.html

data class User(val name: String, val age: Int)
来源：http://hz.xuanzx.com/gtvumbbqas.html

[T09] Kotlin：扩展函数
来源：http://hz.tian-w.cn/gtphgaypjf.html

fun String.exclaim() = this + "!"
来源：http://hz.yvedp.cn/gtvnuluguh.html

[T10] Kotlin：默认参数
来源：http://hz.hnxiangtu.top/gtlkquospp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.gaohongyu789.top/gtlvfocheb.html

[T11] Kotlin：协程
来源：http://hz.jqgfzy.top/gtlykkjjbi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.nanxuanxn.top/gtakhwkdsd.html

[T12] Kotlin：解构声明
来源：http://hz.mhx1999.top/gtqpvjosjl.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj20258888.top/gtzwqlxkyn.html

[T13] Kotlin：只读 Map
来源：http://hz.shzxlz.cn/gthpcghlyj.html

val m = mapOf("a" to 1)
来源：http://hz.cdnleiting.top/gtvcmfxkjx.html

[T14] Kotlin：循环
来源：http://hz.jqgufenzy.top/gtnftmatrn.html

for (i in 1..10) println(i)
来源：http://hz.sysykeji.top/gtqjpkefyj.html

[T15] Kotlin：接口
来源：http://hz.ydjk.org.cn/gtgjqhqkii.html

interface Shape { fun area(): Double }
来源：http://hz.guannengcc.top/gtuoxzinmk.html

[T16] Swift：Hello World
来源：http://hz.fzhhl.top/gtnckcojaw.html

print("Hello")
来源：http://hz.hongshengwenyu.top/gtmmmlwlvl.html

[T17] Swift：变量与常量
来源：http://hz.nanxuanxn.top/gtuydglphn.html

var a = 1;  let b = 2
来源：http://hz.nanxuanxn.top/gthnewowll.html

[T18] Swift：字符串插值
来源：http://hz.zhoulong.xyz/gtwhdsemhd.html

"值: \(b)"
来源：http://hz.gaohongyu789.top/gtwclvijri.html

[T19] Swift：可选绑定
来源：http://hz.daxiang520.top/gtskcghdwv.html

if let n = opt { print(n) }
来源：http://hz.zhiwuduotai.top/gtvvtiurnb.html

[T20] Swift：数组操作
来源：http://hz.zhixingplan.top/gtnvhsdcqk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hnxiangtu.top/gtsawujndx.html

[T21] Swift：遍历
来源：http://hz.kuanghao11.cn/gtrnpdwauq.html

for x in a { print(x) }
来源：http://hz.yongpay.top/gtthfhfeii.html

[T22] Swift：字典
来源：http://hz.jyoumei.cn/gtjtwtqnwp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.shzxlz.cn/gtcvhsxdrt.html

[T23] Swift：函数
来源：http://hz.gotoacloud.top/gtcjrrtdfq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.vqdsnc.cn/gtjjtmxbju.html

[T24] Swift：闭包
来源：http://hz.sufxvd.cn/gtpmovunml.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhongyouzk.top/gttlujomel.html

[T25] Swift：结构体
来源：http://hz.tian-w.cn/gtgjgmcnaq.html

struct P { var x: Int }
来源：http://hz.yonumen.top/gtiigewsve.html

[T26] Swift：类与重写
来源：http://hz.gotoacloud.top/gthoxhldcp.html

class A: Base { override func f() {} }
来源：http://hz.daria6918.cn/gtdbnnwyan.html

[T27] Swift：错误处理
来源：http://hz.fengsongda.top/gtqatdvqjf.html

do { try f() } catch { print(error) }
来源：http://hz.xingfuxueyuan.xyz/gtpgsrpkow.html

[T28] Swift：枚举
来源：http://hz.havefunace.top/gtmzwhivii.html

enum Color { case red, green }
来源：http://hz.jlsjyb.cn/gtorgprxkf.html

[T29] Swift：guard 提前返回
来源：http://hz.haohaochexian.top/gtosvddoge.html

guard let x = opt else { return }
来源：http://hz.nanxinkj.top/gtwnqdmfxt.html

[T30] Swift：协议
来源：http://hz.aizwys.cn/gtwhcinnlp.html

protocol Shape { func area() -> Double }
来源：http://hz.yonumen.top/gtvwlmqiqn.html

[T31] Lua：Hello World
来源：http://hz.jinyuanbaomall.cn/gtfknxhlit.html

print("Hello")
来源：http://hz.shzxlz.cn/gtkledskms.html

[T32] Lua：局部变量
来源：http://hz.jinghuilouyu.cn/gtzlkqmksm.html

local a = 1
来源：http://hz.xingfuxueyuan.xyz/gtifgemwlz.html

[T33] Lua：表（数组）
来源：http://hz.hywenlv.cn/gtvnynmhps.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangshuangyany.cn/gtfqsxnpdx.html

[T34] Lua：遍历表
来源：http://hz.snrcjt.cn/gtxicgiidy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shanyushiyangtech.top/gtxrbslvgj.html

[T35] Lua：字典表
来源：http://hz.fengsongda.top/gtmabecgkz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtfddyvvaw.html

[T36] Lua：函数
来源：http://hz.zhoulong.xyz/gtyavkoamt.html

function add(a, b) return a + b end
来源：http://hz.dashuyun.cn/gtnsnqwumo.html

[T37] Lua：字符串拼接
来源：http://hz.jianghu66.top/gtgximbphe.html

"a" .. "b"
来源：http://hz.smart0.xyz/gtvdpnbbfd.html

[T38] Lua：条件
来源：http://hz.vqdsnc.cn/gtjukytyxy.html

if x > 0 then print("正") end
来源：http://hz.hnxiangtu.top/gtnelphxfn.html

[T39] Lua：模式匹配
来源：http://hz.ppjwa.cn/gtvdmxgdki.html

string.find(s, "%d+")
来源：http://hz.wangdashe.top/gtkzwuchmm.html

[T40] Lua：元表
来源：http://hz.ywan-chungtsiang.top/gtlgpoqxwk.html

setmetatable({}, { __index = base })
来源：http://hz.xingfuxueyuan.xyz/gtwnaermaq.html

[T41] Perl：Hello World
来源：http://hz.shanyushiyangkeji.top/gtfbvrdeui.html

print "Hello\n";
来源：http://hz.sufxvd.cn/gtinzcalar.html

[T42] Perl：变量类型
来源：http://hz.jqgufenzy.top/gtpagvlnwo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.havefunace.top/gtcdxzkfux.html

[T43] Perl：字符串插值
来源：http://hz.daria6918.cn/gtdvxgnund.html

"值: $a"
来源：http://hz.gaohongyu789.top/gtiztnuact.html

[T44] Perl：条件
来源：http://hz.jqgfzy.top/gtsozqkyhb.html

if ($a > 0) { print "正"; }
来源：http://hz.jinyuanbaomall.cn/gtynznsznn.html

[T45] Perl：数组遍历
来源：http://hz.redwolf501.top/gttcqverok.html

for my $x (@arr) { print $x; }
来源：http://hz.zhixingplan.top/gtdifrdfvn.html

[T46] Perl：哈希操作
来源：http://hz.shzxlz.cn/gtgvdafclw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.bjfxy.top/gtchahnzeu.html

[T47] Perl：正则捕获
来源：http://hz.0kj1m.cn/gtlwuwizpf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.daxiang520.top/gtisdzfakt.html

[T48] Perl：正则替换
来源：http://hz.ybcxt.top/gtubwlnwwd.html

$s =~ s/old/new/g;
来源：http://hz.jqgfzy.top/gtwxnyrbhy.html

[T49] Perl：函数
来源：http://hz.cqqwz.cn/gtjbmkqlpr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.quarkkingdee.top/gtvwdtlket.html

[T50] Perl：逐行读文件
来源：http://hz.nanxinkj.top/gtmxwoccbl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.sufxvd.cn/gtyalfkpob.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jyoumei.cn/gturauklyv.html

[T51] Scala：Hello World
来源：http://hz.zhengqikj.top/gtsrliheqk.html

println("Hello")
来源：http://hz.smart0.xyz/gtkvcqvozj.html

[T52] Scala：变量
来源：http://hz.ivvv.top/gtymvdkytf.html

val a = 1;  var b = 2
来源：http://hz.jyoumei.cn/gtzavufvne.html

[T53] Scala：字符串插值
来源：http://hz.hnxiangtu.top/gtcijzzpbs.html

s"值: $b"
来源：http://hz.feifeiyinyue.top/gtyaasloeb.html

[T54] Scala：集合映射
来源：http://hz.svipenyu.cn/gtjwxqetwt.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.iojbl.cn/gtgakekhur.html

[T55] Scala：集合过滤
来源：http://hz.dashuyun.cn/gtsrnaxjlh.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.iojbl.cn/gtoopnzdvu.html

[T56] Scala：样例类
来源：http://hz.dianchejie.cn/gtropmvopr.html

case class User(name: String, age: Int)
来源：http://hz.yj202588.top/gteamwpzzc.html

[T57] Scala：模式匹配
来源：http://hz.zycfv.cn/gtmgvgapdy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.vqdsnc.cn/gtmptkywzp.html

[T58] Scala：函数定义
来源：http://hz.xuanzx.com/gtloifzzas.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ehwqpu.com/gthpxiasee.html

[T59] Scala：循环
来源：http://hz.c1oappe.top/gtcsqiqnuq.html

for (i <- 1 to 10) println(i)
来源：http://hz.chenlongwang.top/gtcfcbghro.html

[T60] Scala：折叠
来源：http://hz.jianghu66.top/gtwtkwdokp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hnqzz.top/gthbgiliww.html

================================================================================
来源：http://hz.yueranfly.top/gtykshzrut.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.fengsongda.top/gtwbjfpbuq.html

================================================================================
来源：http://hz.gotoacloud.top/gtpfvnzjhy.html

[U01] Py：创建虚拟环境
来源：http://hz.chenjidiqi.icu/gtodaqkndw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhongyouzk.top/gtugambczz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ydjk.org.cn/gtcbupwbws.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.mhx1999.top/gtuoxfdnjq.html

[U03] Py：加载 .env 配置
来源：http://hz.haohaochexian.top/gtauplisnd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.redwolf501.top/gthwkjfacn.html

[U04] Py：变量调试打印
来源：http://hz.andypj.xyz/gtaogoxrlv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.daxiang520.top/gtivdcscue.html

[U05] Py：列表去重且保序
来源：http://hz.9152youxi.cn/gtkiktniav.html

list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gttyemsckr.html

[U06] Py：合并两个字典
来源：http://hz.gogol.net.cn/gtcwypbybz.html

{**a, **b}
来源：http://hz.dashuyun.cn/gtzrbgsclj.html

[U07] Py：反转字典键值
来源：http://hz.tian-w.cn/gtpqlkdrta.html

{v: k for k, v in d.items()}
来源：http://hz.hfpthk.cn/gthplkpquw.html

[U08] Py：展平二维列表
来源：http://hz.tanke756.top/gtyqqbfqfi.html

[y for x in nested for y in x]
来源：http://hz.xziqi.cn/gtvrnobkry.html

[U09] Py：字典取最大值的键
来源：http://hz.quarkkingdee.top/gtsajcvjpv.html

max(d, key=d.get)
来源：http://hz.ywan-chungtsiang.top/gtvsvdplzl.html

[U10] Py：按值排序字典
来源：http://hz.wangdashe.top/gtkmzrbeoh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.hongshengwenyu.top/gthgstgzqs.html

[U11] Py：生成器表达式
来源：http://hz.316326.xyz/gtvqemzhua.html

(x * 2 for x in arr)
来源：http://hz.zhaomingkeji.xyz/gtbgeehnrp.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.guannengcc.top/gtbcccukdq.html

Counter(arr).most_common(3)
来源：http://hz.hfpthk.cn/gtpopvmybp.html

[U13] Py：固定长度队列
来源：http://hz.wangdashe.top/gtpegcfdrz.html

deque(maxlen=10)
来源：http://hz.ehwqpu.com/gtxbiyevzt.html

[U14] Py：分组收集到列表
来源：http://hz.dashuyun.cn/gtbcfklwss.html

defaultdict(list)
来源：http://hz.yuxming.cn/gtonqyqlrj.html

[U15] Py：高精度计时
来源：http://hz.guowangkeji.top/gtucgrqaxd.html

t = time.perf_counter()
来源：http://hz.daxiang520.top/gtehxcoizr.html

[U16] Py：命令行参数解析
来源：http://hz.zhengqikj.top/gtzaikwxwu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gotoacloud.top/gtowebljni.html

[U17] Py：初始化日志
来源：http://hz.smart0.xyz/gtboxmzgoy.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.feifeiyinyue.top/gtjuwhcbyd.html

[U18] Py：预编译正则
来源：http://hz.ywan-chungtsiang.top/gtokwhkqtr.html

pat = re.compile(r"\d+")
来源：http://hz.meibo888.top/gtdmhrteks.html

[U19] Py：正则替换带回调
来源：http://hz.cheryme.top/gtludcrmoz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xylfe.cn/gtqzhdcjhm.html

[U20] Py：缓存函数结果
来源：http://hz.ivvv.top/gtetlgyejc.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zycfv.cn/gtanojnhdh.html

[U21] Py：自定义上下文管理器
来源：http://hz.shuidangran.top/gtnffombet.html

@contextlib.contextmanager
来源：http://hz.feifeiyinyue.top/gthgmrgoqt.html

[U22] Py：矩阵转置
来源：http://hz.hywenlv.cn/gtajwbqtwo.html

list(zip(*m))
来源：http://hz.9152youxi.cn/gtsviahmlk.html

[U23] Py：分块读取大文件
来源：http://hz.sweek.top/gtrsnprzbr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yj20258888.top/gtmtmotaxo.html

[U24] Py：路径操作
来源：http://hz.pengpengdd.cyou/gtvhqhupql.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yuanzhike.top/gtnttuspvd.html

[U25] Py：CSV 按字典读
来源：http://hz.xziqi.cn/gtcbkptqot.html

csv.DictReader(f)
来源：http://hz.wangshuangyany.cn/gtjgwaewxz.html

[U26] Py：并发下载
来源：http://hz.yj202588.top/gtxkapoyvv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jianghu66.top/gtowepffkl.html

[U27] Py：异步 HTTP
来源：http://hz.daria6918.cn/gtsmcqczkg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.52xcode.cn/gtqnyedqtg.html

[U28] Py：类型别名
来源：http://hz.xinyue.icu/gtjkrdutod.html

UserId = int
来源：http://hz.daxiang520.top/gtpmarppuy.html

[U29] Py：属性校验
来源：http://hz.bjfxy.top/gtawbpzvqi.html

@property 与 @x.setter 配合
来源：http://hz.pengpengdd.cyou/gtzwfgnine.html

[U30] Py：数据类
来源：http://hz.cheryme.top/gtwzzuicjt.html

@dataclass(slots=True)
来源：http://hz.ybcxt.top/gtwrktggla.html

[U31] Py：单测
来源：http://hz.yj202588.top/gtinsfukzj.html

python -m pytest -q
来源：http://hz.meibo888.top/gtidunmzcj.html

[U32] Py：代码格式化
来源：http://hz.gogol.net.cn/gtdbnvhcjr.html

ruff format . && ruff check --fix .
来源：http://hz.zhiwuduotai.top/gthmckjipp.html

[U33] Py：打包发布
来源：http://hz.zhixingplan.top/gtfmryaimr.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ybcxt.top/gtnycqefza.html

[U34] Py：判断编码
来源：http://hz.fengsongda.top/gtkabhybzv.html

chardet.detect(raw)
来源：http://hz.zhiwuduotai.top/gtocnwxzwp.html

[U35] Py：发送邮件
来源：http://hz.fengsongda.top/gteiejpwjv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yuanzhike.top/gtoprhzgnx.html

[U36] Py：定时任务
来源：http://hz.gzhubu.top/gtybjuyosf.html

schedule.every(10).minutes.do(job)
来源：http://hz.hammf.cn/gtwrhifnyr.html

[U37] Py：读写 Excel
来源：http://hz.chenlongwang.top/gtwvglznbg.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.c1oappe.top/gtcmlvvjgp.html

[U38] Py：获取脚本所在目录
来源：http://hz.xziqi.cn/gtoogwyffq.html

Path(__file__).resolve().parent
来源：http://hz.aizwys.cn/gtozqecmnu.html

[U39] Py：判断是否在交互环境
来源：http://hz.aizwys.cn/gtyomcvwrd.html

sys.stdout.isatty()
来源：http://hz.zhiwuduotai.top/gtfqrftxha.html

[U40] Py：打印到标准错误
来源：http://hz.zhijiandao.cn/gtjjadbnfv.html

print("err", file=sys.stderr)
来源：http://hz.0kj1m.cn/gtegiwuaum.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.quarkkingdee.top/gtnogkdmgz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hywenlv.cn/gtiqtysxsn.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hysaishi.cn/gtrdzrduex.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hywenlv.cn/gtiawcdnqf.html

[U43] PHP：声明命名空间
来源：http://hz.tanke756.top/gtnfrmhosy.html

namespace App\Http;
来源：http://hz.dianchejie.cn/gtvrhohbnn.html

[U44] PHP：开启严格类型
来源：http://hz.zhaomingkeji.xyz/gttaduqmne.html

declare(strict_types=1);
来源：http://hz.vqdsnc.cn/gteguezekz.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ivvv.top/gtazjkeder.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtpijctskz.html

[U46] PHP：可空类型
来源：http://hz.aizwys.cn/gtyxwrpwsi.html

?string $name = null
来源：http://hz.jqgfzy.top/gtqjhcfyaz.html

[U47] PHP：联合类型
来源：http://hz.316326.xyz/gtkrsqirqn.html

int|string $id
来源：http://hz.ehwqpu.com/gtpwoeraek.html

[U48] PHP：纯枚举
来源：http://hz.dashuyun.cn/gtfyknwbag.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhiwuduotai.top/gteacaalei.html

[U49] PHP：只读属性
来源：http://hz.gzhubu.top/gtjplxfpkr.html

public readonly string $name
来源：http://hz.hfpthk.cn/gtoqalbctg.html

[U50] PHP：构造器属性提升
来源：http://hz.jinqigufen.top/gtkamodilb.html

public function __construct(private int $id) {}
来源：http://hz.hnxiangtu.top/gtjlsslwqa.html

[U51] PHP：数组解构
来源：http://hz.shangyingyoupin.top/gtbyasjyfg.html

[$a, $b] = $arr;
来源：http://hz.yj202588.top/gtofyxjnwo.html

[U52] PHP：箭头函数
来源：http://hz.yueranfly.top/gtphhopdyx.html

$double = fn($x) => $x * 2;
来源：http://hz.jiagoushi.top/gtldhlokiq.html

[U53] PHP：空合并运算符
来源：http://hz.zycfv.cn/gtdfexigdo.html

$v = $a ?? $b ?? "default";
来源：http://hz.hfpthk.cn/gtxdnxwknh.html

[U54] PHP：空安全调用
来源：http://hz.yvedp.cn/gtnfdriazx.html

$obj?->method()
来源：http://hz.xylfe.cn/gthkooahst.html

[U55] PHP：match 表达式
来源：http://hz.meibo888.top/gtkiyihyvg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhengqikj.top/gtzvacpqsh.html

[U56] PHP：命名参数
来源：http://hz.iojbl.cn/gtoxzuoczm.html

f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtfevtvlhz.html

[U57] PHP：字符串插值
来源：http://hz.shanyushiyangkeji.top/gttncqieus.html

"值: {$a}"
来源：http://hz.xuanzx.com/gtcfgoxvws.html

[U58] PHP：数组三件套
来源：http://hz.ehwqpu.com/gtujwlgcvo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.zhengqikj.top/gtyjkmltvk.html

[U59] PHP：自定义排序
来源：http://hz.guowangkeji.top/gtdmubkuhf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.mhx1999.top/gtjndwxvlq.html

[U60] PHP：JSON 编解码
来源：http://hz.vqdsnc.cn/gtsqvfjjlw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hfpthk.cn/gtbflitotx.html


<!-- 参考信息 -->