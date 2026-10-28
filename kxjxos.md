代发 wailian999

[S37] C++：set
来源：http://hz.redwolf501.top/gtgvmbowzf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxuanxn.top/gtoyfglehd.html

[S38] C++：排序
来源：http://hz.dianchejie.cn/gtjnbtvnly.html

std::sort(v.begin(), v.end());
来源：http://hz.zhiwuduotai.top/gtatrtgoxf.html

[S39] C++：自定义比较器排序
来源：http://hz.andypj.xyz/gtmntwdsll.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxuanxn.top/gtgxbnuotb.html

[S40] C++：查找元素
来源：http://hz.svipenyu.cn/gtapkyrigg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xziqi.cn/gtyumdmdsv.html

[S41] C++：类与构造函数
来源：http://hz.meibo888.top/gtfcjpkezq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.haohaochexian.top/gtcniwnoba.html

[S42] C++：继承与虚函数
来源：http://hz.hysaishi.cn/gtzibivgex.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj202588.top/gtikemavfh.html

[S43] C++：智能指针
来源：http://hz.feifeiyinyue.top/gtreuqdtbg.html

auto p = std::make_unique<int>(5);
来源：http://hz.feifeiyinyue.top/gteumkxwxj.html

[S44] C++：引用传参
来源：http://hz.pengpengdd.cyou/gttqzomnxp.html

void inc(int &x) { ++x; }
来源：http://hz.dashuyun.cn/gtuwwtwmbi.html

[S45] C++：lambda
来源：http://hz.yuanzhike.top/gtmtwbfnxw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.c1oappe.top/gtmkzesvsr.html

[S46] C++：函数模板
来源：http://hz.quarkkingdee.top/gttwflfzty.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yuxming.cn/gtjrooswxv.html

[S47] C++：结构化绑定遍历
来源：http://hz.pycfn.com/gtxhffenms.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.wangdashe.top/gtzcnzoqxv.html

[S48] C++：逐行读文件
来源：http://hz.jinqigufen.top/gtumxrnxxg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinyuanbaomall.cn/gtwdkprlmx.html

while (std::getline(in, line)) { }
来源：http://hz.ywan-chungtsiang.top/gtwauhgfya.html

[S49] C++：写文件
来源：http://hz.aizwys.cn/gtqzqhsxmf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nwbrower.top/gtquxjdtzn.html

[S50] C++：格式化数字
来源：http://hz.yonumen.top/gtqunrruee.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhijiandao.cn/gtoibuxekn.html

[S51] C++：显式类型转换
来源：http://hz.cashguo.top/gtmlsbelij.html

static_cast<double>(a) / b
来源：http://hz.tian-w.cn/gtfgopfltd.html

[S52] C++：const 与 noexcept
来源：http://hz.shzxlz.cn/gtjzmmpuel.html

int size() const noexcept { return n_; }
来源：http://hz.guannengcc.top/gtpirwsrkj.html

[S53] C++：移动语义
来源：http://hz.yuxming.cn/gtxfucavdf.html

std::vector<int> w = std::move(v);
来源：http://hz.yangfankeji.com/gtpennczlr.html

[S54] C++：异常处理
来源：http://hz.xinyue.icu/gtnlrioplc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sufxvd.cn/gtpdnjcyxc.html

[S55] C++：结构化绑定
来源：http://hz.vqdsnc.cn/gthrkloblv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jlsjyb.cn/gtbyvzbtfi.html

[S56] C++：optional
来源：http://hz.sysykeji.top/gtwpjjutgz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tian-w.cn/gtngyeqbjn.html

[S57] C++：编译期常量
来源：http://hz.guannengcc.top/gtuantklcn.html

constexpr int N = 10;
来源：http://hz.jqgufenzy.top/gtwuyzavzn.html

[S58] C++：命名空间
来源：http://hz.wangdashe.top/gtprpnseaa.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj202588.top/gtdzoslqic.html

[S59] C++：静态断言
来源：http://hz.jianghu66.top/gtjdgwlkyy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sweek.top/gtcgimvlor.html

[S60] C++：遍历并删除元素
来源：http://hz.ivvv.top/gtszktzgjc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.guannengcc.top/gtugjjiqab.html

================================================================================
来源：http://hz.haohaochexian.top/gtxiturxgw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fengsongda.top/gtskvxpqlr.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcupjvtmm.html

[T01] Kotlin：Hello World
来源：http://hz.sysykeji.top/gtgplmpylg.html

println("Hello")
来源：http://hz.52xcode.cn/gthkwtthyw.html

[T02] Kotlin：变量
来源：http://hz.cucudq.cn/gtmcwegbkh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xylfe.cn/gtpxtxlgtp.html

[T03] Kotlin：字符串模板
来源：http://hz.guannengcc.top/gtlaiypekd.html

"值: $b"
来源：http://hz.shanyushiyangkeji.top/gtmmqyfvke.html

[T04] Kotlin：空安全
来源：http://hz.zhongyouzk.top/gtexvzyavf.html

val n: String? = null;  n?.length
来源：http://hz.shangyingyoupin.top/gtsohpcpul.html

[T05] Kotlin：when 表达式
来源：http://hz.jinyuanbaomall.cn/gtwxexzsgk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhengqikj.top/gtvfwunurh.html

[T06] Kotlin：集合映射
来源：http://hz.yonumen.top/gttbpprgfc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yonumen.top/gtrllbitmn.html

[T07] Kotlin：集合过滤
来源：http://hz.gaohongyu789.top/gtlwdlswas.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.andypj.xyz/gtkbejowfy.html

[T08] Kotlin：数据类
来源：http://hz.shzxlz.cn/gtqgngwmnz.html

data class User(val name: String, val age: Int)
来源：http://hz.yongpay.top/gtbhhwwtfg.html

[T09] Kotlin：扩展函数
来源：http://hz.hywenlv.cn/gtvqehnbyp.html

fun String.exclaim() = this + "!"
来源：http://hz.zhixingplan.top/gtgarsltoo.html

[T10] Kotlin：默认参数
来源：http://hz.haohaochexian.top/gtptsmojjy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hammf.cn/gtsqkdkoir.html

[T11] Kotlin：协程
来源：http://hz.snrcjt.cn/gtxzuexrjc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xinyue.icu/gtxgghgfpd.html

[T12] Kotlin：解构声明
来源：http://hz.gzhubu.top/gtsxtngblc.html

val (a, b) = Pair(1, 2)
来源：http://hz.gogol.net.cn/gtgiclpkjf.html

[T13] Kotlin：只读 Map
来源：http://hz.yonumen.top/gtnmrajnqn.html

val m = mapOf("a" to 1)
来源：http://hz.gaohongyu789.top/gtwexfzimd.html

[T14] Kotlin：循环
来源：http://hz.gzhubu.top/gtowqvvvap.html

for (i in 1..10) println(i)
来源：http://hz.jqgufenzy.top/gtciihpngj.html

[T15] Kotlin：接口
来源：http://hz.zycfv.cn/gtbktjohil.html

interface Shape { fun area(): Double }
来源：http://hz.yj202588.top/gtnwlfpmur.html

[T16] Swift：Hello World
来源：http://hz.chenzaomai.com/gthjytzcjp.html

print("Hello")
来源：http://hz.dashuyun.cn/gtybbxnqwp.html

[T17] Swift：变量与常量
来源：http://hz.chenlongwang.top/gtbuqkzmlb.html

var a = 1;  let b = 2
来源：http://hz.yueranfly.top/gtqxarohhb.html

[T18] Swift：字符串插值
来源：http://hz.mhx1999.top/gtqjujqjjf.html

"值: \(b)"
来源：http://hz.kuanghao11.cn/gtmamxnhnb.html

[T19] Swift：可选绑定
来源：http://hz.sufxvd.cn/gtacnkhouv.html

if let n = opt { print(n) }
来源：http://hz.ybcxt.top/gtszojqgsp.html

[T20] Swift：数组操作
来源：http://hz.shangyingyoupin.top/gtxqfdeegq.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenjidiqi.icu/gtbhbrtliz.html

[T21] Swift：遍历
来源：http://hz.hnqzz.top/gtosnupfna.html

for x in a { print(x) }
来源：http://hz.zhongyouzk.top/gtdgtfwuxx.html

[T22] Swift：字典
来源：http://hz.xziqi.cn/gtyenunvhj.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yj20258888.top/gtacvzxxse.html

[T23] Swift：函数
来源：http://hz.wangdashe.top/gtepvogrwc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.vqdsnc.cn/gtnxubegjs.html

[T24] Swift：闭包
来源：http://hz.sysykeji.top/gtohabsslc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.52xcode.cn/gtxahdqttg.html

[T25] Swift：结构体
来源：http://hz.iojbl.cn/gtgxjaoxia.html

struct P { var x: Int }
来源：http://hz.yanxiufei.cn/gtotgigoyj.html

[T26] Swift：类与重写
来源：http://hz.hongshengwenyu.top/gtzcvuhvcu.html

class A: Base { override func f() {} }
来源：http://hz.xingfuxueyuan.xyz/gtijkwoscc.html

[T27] Swift：错误处理
来源：http://hz.meibo888.top/gtxkdiupug.html

do { try f() } catch { print(error) }
来源：http://hz.wangshuangyany.cn/gtmqcsvord.html

[T28] Swift：枚举
来源：http://hz.hammf.cn/gtxjernyup.html

enum Color { case red, green }
来源：http://hz.shanyushiyangkeji.top/gtdquqdiwj.html

[T29] Swift：guard 提前返回
来源：http://hz.jyoumei.cn/gtqmbplvsh.html

guard let x = opt else { return }
来源：http://hz.smart0.xyz/gthkrhckov.html

[T30] Swift：协议
来源：http://hz.hongshengwenyu.top/gtvqcwrfox.html

protocol Shape { func area() -> Double }
来源：http://hz.kuanghao11.cn/gtybgotivf.html

[T31] Lua：Hello World
来源：http://hz.zhengqikj.top/gtfwqnjebc.html

print("Hello")
来源：http://hz.ehwqpu.com/gtzkbmlqpx.html

[T32] Lua：局部变量
来源：http://hz.gogol.net.cn/gthlpeuodd.html

local a = 1
来源：http://hz.zhengqikj.top/gtbargbkaf.html

[T33] Lua：表（数组）
来源：http://hz.chenlongwang.top/gtuyqzliep.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.gaohongyu789.top/gtfaghxesc.html

[T34] Lua：遍历表
来源：http://hz.dashuyun.cn/gtusynchlo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yangfankeji.com/gtvgwyhvjq.html

[T35] Lua：字典表
来源：http://hz.c1oappe.top/gtjdzhyndr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangdashe.top/gtxreeymyb.html

[T36] Lua：函数
来源：http://hz.xuetiantiany.cn/gtbcufwobl.html

function add(a, b) return a + b end
来源：http://hz.svipenyu.cn/gtbevlopma.html

[T37] Lua：字符串拼接
来源：http://hz.tanke756.top/gtpibjbdac.html

"a" .. "b"
来源：http://hz.yuanzhike.top/gtoasucamu.html

[T38] Lua：条件
来源：http://hz.chenzaomai.com/gtfxmgufdb.html

if x > 0 then print("正") end
来源：http://hz.wangdashe.top/gtascbbtuq.html

[T39] Lua：模式匹配
来源：http://hz.yonumen.top/gtvzgrhvll.html

string.find(s, "%d+")
来源：http://hz.yueranfly.top/gtislsdoqp.html

[T40] Lua：元表
来源：http://hz.ydzc1.top/gtnbaqkioj.html

setmetatable({}, { __index = base })
来源：http://hz.aizwys.cn/gtsqhkbodu.html

[T41] Perl：Hello World
来源：http://hz.yanxiufei.cn/gtcjznashb.html

print "Hello\n";
来源：http://hz.sysykeji.top/gtkznfgwqx.html

[T42] Perl：变量类型
来源：http://hz.sysykeji.top/gtbdxkyugb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hysaishi.cn/gtxgoxltxo.html

[T43] Perl：字符串插值
来源：http://hz.jinqigufen.top/gtzbpdwhih.html

"值: $a"
来源：http://hz.guowangkeji.top/gtnaeylcoj.html

[T44] Perl：条件
来源：http://hz.xinyue.icu/gtkgqfbpof.html

if ($a > 0) { print "正"; }
来源：http://hz.cdnleiting.top/gtvmwpguro.html

[T45] Perl：数组遍历
来源：http://hz.yueranfly.top/gtyzhqivpg.html

for my $x (@arr) { print $x; }
来源：http://hz.jinqigufen.top/gtwiojwbxa.html

[T46] Perl：哈希操作
来源：http://hz.xuanzx.com/gtandyjmor.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zdqjudy.top/gtmecbogbt.html

[T47] Perl：正则捕获
来源：http://hz.cheryme.top/gtlnbvwtga.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cdnleiting.top/gtdfxemdty.html

[T48] Perl：正则替换
来源：http://hz.vqdsnc.cn/gtretlhtcp.html

$s =~ s/old/new/g;
来源：http://hz.zhixingplan.top/gtenhnxfxz.html

[T49] Perl：函数
来源：http://hz.mhx1999.top/gtkswxlfsh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zdqjudy.top/gtirmwbfjh.html

[T50] Perl：逐行读文件
来源：http://hz.vqdsnc.cn/gtcepmdfkn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj202588.top/gteluksdgn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhoulong.xyz/gtzisurnkk.html

[T51] Scala：Hello World
来源：http://hz.ydjk.org.cn/gtsiarzeps.html

println("Hello")
来源：http://hz.zhiwuduotai.top/gtfceidkib.html

[T52] Scala：变量
来源：http://hz.yj202588.top/gtzsyexydz.html

val a = 1;  var b = 2
来源：http://hz.birdmap.top/gtvswzcyea.html

[T53] Scala：字符串插值
来源：http://hz.52xcode.cn/gtrxtcjega.html

s"值: $b"
来源：http://hz.ehwqpu.com/gtkdomamzq.html

[T54] Scala：集合映射
来源：http://hz.yj20258.top/gtthwsfnrd.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jyoumei.cn/gtjxciqhls.html

[T55] Scala：集合过滤
来源：http://hz.shzxlz.cn/gtwkmsslww.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ehwqpu.com/gtdindrxpt.html

[T56] Scala：样例类
来源：http://hz.xinyue.icu/gtreyntxux.html

case class User(name: String, age: Int)
来源：http://hz.nanxuanxn.top/gtrpukovxy.html

[T57] Scala：模式匹配
来源：http://hz.jianghu66.top/gtershfhin.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hywenlv.cn/gtibtqpgav.html

[T58] Scala：函数定义
来源：http://hz.gzhubu.top/gteayfwvvm.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.chenjidiqi.icu/gtyycmxaog.html

[T59] Scala：循环
来源：http://hz.pengpengdd.cyou/gtzzkjqvuq.html

for (i <- 1 to 10) println(i)
来源：http://hz.guowangkeji.top/gtrijgjtjy.html

[T60] Scala：折叠
来源：http://hz.jinghuilouyu.cn/gtpvkxdpny.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yueranfly.top/gtfnnzrhyd.html

================================================================================
来源：http://hz.zhixingplan.top/gtfydppioa.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xuetiantiany.cn/gtnqrxeamz.html

================================================================================
来源：http://hz.daxiang520.top/gtqxmvfzvo.html

[U01] Py：创建虚拟环境
来源：http://hz.yj20258.top/gtgatqssif.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhiwuduotai.top/gtzsyjwftw.html

[U02] Py：导出 / 安装依赖
来源：http://hz.quarkkingdee.top/gtewqxatlw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.kuanghao11.cn/gtihcbuiom.html

[U03] Py：加载 .env 配置
来源：http://hz.cqqwz.cn/gtbebtgstz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.meibo888.top/gthweltfqq.html

[U04] Py：变量调试打印
来源：http://hz.dashuyun.cn/gttmqdzrtx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.quarkkingdee.top/gtbddxiays.html

[U05] Py：列表去重且保序
来源：http://hz.sxryk.cn/gtzigznmjb.html

list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gtuwprnkym.html

[U06] Py：合并两个字典
来源：http://hz.nanxuanxn.top/gthfpxqnzm.html

{**a, **b}
来源：http://hz.redwolf501.top/gtxcmmdhyz.html

[U07] Py：反转字典键值
来源：http://hz.mhx1999.top/gtcwwxeztu.html

{v: k for k, v in d.items()}
来源：http://hz.ybcxt.top/gtmclvjdek.html

[U08] Py：展平二维列表
来源：http://hz.shangyingyoupin.top/gtjrefqbgy.html

[y for x in nested for y in x]
来源：http://hz.xziqi.cn/gtsrxwajhv.html

[U09] Py：字典取最大值的键
来源：http://hz.dashuyun.cn/gtpewlfqlw.html

max(d, key=d.get)
来源：http://hz.chenlongwang.top/gtkbcsyoqt.html

[U10] Py：按值排序字典
来源：http://hz.52xcode.cn/gtfuvankaf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhixingplan.top/gtrshaceub.html

[U11] Py：生成器表达式
来源：http://hz.hywenlv.cn/gtbkjvcmar.html

(x * 2 for x in arr)
来源：http://hz.chenlongwang.top/gtnyhbqjcp.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.quarkkingdee.top/gtzrnppymm.html

Counter(arr).most_common(3)
来源：http://hz.snrcjt.cn/gtezzpizkn.html

[U13] Py：固定长度队列
来源：http://hz.jinghuilouyu.cn/gtuiruuptg.html

deque(maxlen=10)
来源：http://hz.yuanzhike.top/gtuvpjkdvg.html

[U14] Py：分组收集到列表
来源：http://hz.chenzaomai.com/gtwhzqldyk.html

defaultdict(list)
来源：http://hz.zhoulong.xyz/gtubeibmsz.html

[U15] Py：高精度计时
来源：http://hz.pengpengdd.cyou/gtzirceagm.html

t = time.perf_counter()
来源：http://hz.cdnleiting.top/gtqsvhckzw.html

[U16] Py：命令行参数解析
来源：http://hz.chenjidiqi.icu/gtmezdggmf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.ivvv.top/gtfifdzkqd.html

[U17] Py：初始化日志
来源：http://hz.ehwqpu.com/gtlupexhlh.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.guannengcc.top/gtwuqaojzs.html

[U18] Py：预编译正则
来源：http://hz.chenjidiqi.icu/gtfccoqgib.html

pat = re.compile(r"\d+")
来源：http://hz.iojbl.cn/gtmsnsdzej.html

[U19] Py：正则替换带回调
来源：http://hz.nwbrower.top/gtqyzdeesx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.redwolf501.top/gtldcetyya.html

[U20] Py：缓存函数结果
来源：http://hz.tian-w.cn/gtxadcyncs.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sufxvd.cn/gttjiaffzv.html

[U21] Py：自定义上下文管理器
来源：http://hz.daria6918.cn/gteytfiqxo.html

@contextlib.contextmanager
来源：http://hz.gaohongyu789.top/gtndxpvxle.html

[U22] Py：矩阵转置
来源：http://hz.316326.xyz/gtpbzwdicg.html

list(zip(*m))
来源：http://hz.sysykeji.top/gtzitqwzil.html

[U23] Py：分块读取大文件
来源：http://hz.jinghuilouyu.cn/gtorrwbkal.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.cheryme.top/gtkhxieolj.html

[U24] Py：路径操作
来源：http://hz.yueranfly.top/gtebqrhkdb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zycfv.cn/gtpwaepzcn.html

[U25] Py：CSV 按字典读
来源：http://hz.ywan-chungtsiang.top/gtzfzhehxi.html

csv.DictReader(f)
来源：http://hz.chenjidiqi.icu/gtjlrjvcam.html

[U26] Py：并发下载
来源：http://hz.shzxlz.cn/gttorduuse.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gaohongyu789.top/gtkdszrhke.html

[U27] Py：异步 HTTP
来源：http://hz.xylfe.cn/gtxdwykdfo.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.gogol.net.cn/gtbmzqbaos.html

[U28] Py：类型别名
来源：http://hz.zhiwuduotai.top/gtxamfythk.html

UserId = int
来源：http://hz.jyoumei.cn/gtlgpfkins.html

[U29] Py：属性校验
来源：http://hz.hywenlv.cn/gtlkrpstuh.html

@property 与 @x.setter 配合
来源：http://hz.jianghu66.top/gthsqejeea.html

[U30] Py：数据类
来源：http://hz.dashuyun.cn/gtnhfsqerk.html

@dataclass(slots=True)
来源：http://hz.pengpengdd.cyou/gtwqakocwh.html

[U31] Py：单测
来源：http://hz.hnxiangtu.top/gtznehvwsj.html

python -m pytest -q
来源：http://hz.quarkkingdee.top/gtvttjbjak.html

[U32] Py：代码格式化
来源：http://hz.0kj1m.cn/gtsysgpftf.html

ruff format . && ruff check --fix .
来源：http://hz.guannengcc.top/gttjqqyjyw.html

[U33] Py：打包发布
来源：http://hz.ehwqpu.com/gtisxkzguq.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.nanxuanxn.top/gtpuytdniq.html

[U34] Py：判断编码
来源：http://hz.tianlin.xyz/gtpkprjpub.html

chardet.detect(raw)
来源：http://hz.tanke756.top/gtsmulataj.html

[U35] Py：发送邮件
来源：http://hz.sysykeji.top/gtlgbehvbd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.tianlin.xyz/gtqrlkeowy.html

[U36] Py：定时任务
来源：http://hz.yanxiufei.cn/gtahzzzirv.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhixingplan.top/gtqqoirlsc.html

[U37] Py：读写 Excel
来源：http://hz.jqgufenzy.top/gtgsbrhkgv.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.sysykeji.top/gtpuvxfdww.html

[U38] Py：获取脚本所在目录
来源：http://hz.zhixingplan.top/gtyiqrjspt.html

Path(__file__).resolve().parent
来源：http://hz.chenjidiqi.icu/gthfuvdiip.html

[U39] Py：判断是否在交互环境
来源：http://hz.guannengcc.top/gtklgjavwc.html

sys.stdout.isatty()
来源：http://hz.zycfv.cn/gtddhdtekq.html

[U40] Py：打印到标准错误
来源：http://hz.ywan-chungtsiang.top/gtizxjievi.html

print("err", file=sys.stderr)
来源：http://hz.redwolf501.top/gtgnzssijj.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.mhx1999.top/gtoehtiseu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cheryme.top/gtbwrcsvws.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jqgufenzy.top/gtfuappgpy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.ivvv.top/gtibjqwfha.html

[U43] PHP：声明命名空间
来源：http://hz.zycfv.cn/gtyaokwype.html

namespace App\Http;
来源：http://hz.ppjwa.cn/gtgnwqlexf.html

[U44] PHP：开启严格类型
来源：http://hz.smart0.xyz/gtlcfhkjxp.html

declare(strict_types=1);
来源：http://hz.0kj1m.cn/gtelragdht.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ppjwa.cn/gtwpwhidlr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jyoumei.cn/gtbjypnybt.html

[U46] PHP：可空类型
来源：http://hz.tanke756.top/gttrcvudgy.html

?string $name = null
来源：http://hz.cqqwz.cn/gthvtqiyvw.html

[U47] PHP：联合类型
来源：http://hz.jiagoushi.top/gtlpzxnlzr.html

int|string $id
来源：http://hz.svipenyu.cn/gtgdmkjava.html

[U48] PHP：纯枚举
来源：http://hz.aibaodan.cn/gtrzxxgtgc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.zhiwuduotai.top/gtnoybsoyd.html

[U49] PHP：只读属性
来源：http://hz.cheryme.top/gtqxdvmoon.html

public readonly string $name
来源：http://hz.nanxuanxn.top/gtjuvsjbau.html

[U50] PHP：构造器属性提升
来源：http://hz.cashguo.top/gtmjuhhmeq.html

public function __construct(private int $id) {}
来源：http://hz.shuidangran.top/gtiducskpv.html

[U51] PHP：数组解构
来源：http://hz.gzhubu.top/gtyyisxcbl.html

[$a, $b] = $arr;
来源：http://hz.ppjwa.cn/gtlzkjosqz.html

[U52] PHP：箭头函数
来源：http://hz.yj20258888.top/gtolsdnmey.html

$double = fn($x) => $x * 2;
来源：http://hz.fengsongda.top/gtvxvbldbv.html

[U53] PHP：空合并运算符
来源：http://hz.hywenlv.cn/gtbjcbvcum.html

$v = $a ?? $b ?? "default";
来源：http://hz.shangyingyoupin.top/gtiqcttakr.html

[U54] PHP：空安全调用
来源：http://hz.guannengcc.top/gtthwnjubq.html

$obj?->method()
来源：http://hz.quarkkingdee.top/gtxhwdhsgs.html

[U55] PHP：match 表达式
来源：http://hz.ivvv.top/gthllfwtko.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.dianchejie.cn/gtwofgjaoc.html

[U56] PHP：命名参数
来源：http://hz.yanxiufei.cn/gtqkjgdwew.html

f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtfdezlofx.html

[U57] PHP：字符串插值
来源：http://hz.gogol.net.cn/gtkougybvb.html

"值: {$a}"
来源：http://hz.shuidangran.top/gtprjxnjir.html

[U58] PHP：数组三件套
来源：http://hz.hongshengwenyu.top/gtvhediynf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinqigufen.top/gtbgffjxfx.html

[U59] PHP：自定义排序
来源：http://hz.mhx1999.top/gtbwdvweli.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.meibo888.top/gtaocxfvil.html

[U60] PHP：JSON 编解码
来源：http://hz.jinghuilouyu.cn/gtpvhgcwbo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hnxiangtu.top/gtzbmiusme.html

[U61] PHP：正则
来源：http://hz.jinghuilouyu.cn/gtornavopl.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cdnleiting.top/gtsgyovqff.html

[U62] PHP：日期对象
来源：http://hz.daxiang520.top/gtvcraafqu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.nwbrower.top/gtlprqmuhw.html


<!-- 参考信息 -->