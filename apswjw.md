代发 wailian999

[S39] C++：自定义比较器排序
来源：http://hz.yj20258888.top/gtkgnqdtqz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ydzc1.top/gtmqfbdaes.html

[S40] C++：查找元素
来源：http://hz.yuanzhike.top/gtqvlqjcfj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guannengcc.top/gtspguxzwb.html

[S41] C++：类与构造函数
来源：http://hz.mhx1999.top/gtmrfslwjs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinghuilouyu.cn/gtunpebrgt.html

[S42] C++：继承与虚函数
来源：http://hz.sufxvd.cn/gthxuiugzo.html

class B : public Base { public: void f() override {} };
来源：http://hz.mhx1999.top/gtxnanoppi.html

[S43] C++：智能指针
来源：http://hz.ydzc1.top/gthyyivkxv.html

auto p = std::make_unique<int>(5);
来源：http://hz.fengsongda.top/gtyimwgjxj.html

[S44] C++：引用传参
来源：http://hz.zhixingplan.top/gtrieephcw.html

void inc(int &x) { ++x; }
来源：http://hz.zycfv.cn/gtqvsyekqc.html

[S45] C++：lambda
来源：http://hz.wangdashe.top/gtzoolgzco.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.vqdsnc.cn/gtryczbctd.html

[S46] C++：函数模板
来源：http://hz.shanyushiyangkeji.top/gtmlswyqkr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenlongwang.top/gtaiacsrjj.html

[S47] C++：结构化绑定遍历
来源：http://hz.sufxvd.cn/gtnpkkuxhq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgfzy.top/gtgwhenemo.html

[S48] C++：逐行读文件
来源：http://hz.nanxuanxn.top/gtofwcctvi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.smart0.xyz/gtofzwsdvg.html

while (std::getline(in, line)) { }
来源：http://hz.ybcxt.top/gtexcaqocn.html

[S49] C++：写文件
来源：http://hz.xziqi.cn/gtlgitxrbm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.ppjwa.cn/gtrgubnbej.html

[S50] C++：格式化数字
来源：http://hz.ehwqpu.com/gtwvszkfzu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ydjk.org.cn/gtjbypbges.html

[S51] C++：显式类型转换
来源：http://hz.nwbrower.top/gtwzkirmzg.html

static_cast<double>(a) / b
来源：http://hz.aizwys.cn/gtqhniofqx.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258888.top/gtuohhbhze.html

int size() const noexcept { return n_; }
来源：http://hz.52xcode.cn/gtlylhbbkx.html

[S53] C++：移动语义
来源：http://hz.zhengqikj.top/gtthosyefl.html

std::vector<int> w = std::move(v);
来源：http://hz.aizwys.cn/gthvzldncl.html

[S54] C++：异常处理
来源：http://hz.yongpay.top/gtkmynmcjf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ybcxt.top/gtfgjrnkba.html

[S55] C++：结构化绑定
来源：http://hz.jyoumei.cn/gtatelnhsw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhijiandao.cn/gtwoirgaob.html

[S56] C++：optional
来源：http://hz.shanyushiyangtech.top/gtxcjjjwqf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhongyouzk.top/gtxrlphyfl.html

[S57] C++：编译期常量
来源：http://hz.jinqigufen.top/gtzoprovcw.html

constexpr int N = 10;
来源：http://hz.shzxlz.cn/gtebyliwkf.html

[S58] C++：命名空间
来源：http://hz.meibo888.top/gtakclryzr.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigfzy.top/gtsplopnvi.html

[S59] C++：静态断言
来源：http://hz.316326.xyz/gtxmcpfokh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigufen.top/gtateixxtr.html

[S60] C++：遍历并删除元素
来源：http://hz.wangdashe.top/gtsyljqyut.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.havefunace.top/gtvwxbpact.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gthsqajspj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hfpthk.cn/gtxlsjhaxk.html

================================================================================
来源：http://hz.andypj.xyz/gtmzirnmmk.html

[T01] Kotlin：Hello World
来源：http://hz.yj202588.top/gtluweuzep.html

println("Hello")
来源：http://hz.cashguo.top/gtoaodlbje.html

[T02] Kotlin：变量
来源：http://hz.sxryk.cn/gtvepsrgvq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.bjfxy.top/gtmhrepvsp.html

[T03] Kotlin：字符串模板
来源：http://hz.xingfuxueyuan.xyz/gtfcfcllqu.html

"值: $b"
来源：http://hz.zycfv.cn/gtecfaazoc.html

[T04] Kotlin：空安全
来源：http://hz.yueranfly.top/gtcvsmnrlg.html

val n: String? = null;  n?.length
来源：http://hz.smart0.xyz/gtblggttoa.html

[T05] Kotlin：when 表达式
来源：http://hz.xinyue.icu/gtxnubgeze.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sweek.top/gtoiggmhyf.html

[T06] Kotlin：集合映射
来源：http://hz.yangfankeji.com/gteetanvoe.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yvedp.cn/gtkvjwutnq.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgfzy.top/gtnglyopbt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnqzz.top/gtevpjvznc.html

[T08] Kotlin：数据类
来源：http://hz.yueranfly.top/gtwnxwrfib.html

data class User(val name: String, val age: Int)
来源：http://hz.nanxinkj.top/gtgznjnuip.html

[T09] Kotlin：扩展函数
来源：http://hz.0kj1m.cn/gtgxlaznbj.html

fun String.exclaim() = this + "!"
来源：http://hz.shuidangran.top/gtawvrqyre.html

[T10] Kotlin：默认参数
来源：http://hz.zhongyouzk.top/gtycxlfhjt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.haohaochexian.top/gtvgsrrrbn.html

[T11] Kotlin：协程
来源：http://hz.hammf.cn/gtuifepvjw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.shangyingyoupin.top/gtdnmfspyx.html

[T12] Kotlin：解构声明
来源：http://hz.daxiang520.top/gtigibedwv.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhoulong.xyz/gtusmlahko.html

[T13] Kotlin：只读 Map
来源：http://hz.gogol.net.cn/gtzjlintmx.html

val m = mapOf("a" to 1)
来源：http://hz.0kj1m.cn/gtspnujbig.html

[T14] Kotlin：循环
来源：http://hz.daria6918.cn/gtynzsjcow.html

for (i in 1..10) println(i)
来源：http://hz.cqqwz.cn/gtegdiftjy.html

[T15] Kotlin：接口
来源：http://hz.shzxlz.cn/gtdikfpthi.html

interface Shape { fun area(): Double }
来源：http://hz.ydjk.org.cn/gtgvkqmavh.html

[T16] Swift：Hello World
来源：http://hz.jlsjyb.cn/gteqillzcm.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtuxycntlg.html

[T17] Swift：变量与常量
来源：http://hz.shangyingyoupin.top/gtffpdhpkd.html

var a = 1;  let b = 2
来源：http://hz.sweek.top/gtsnqmfkbq.html

[T18] Swift：字符串插值
来源：http://hz.jiagoushi.top/gtayvvizug.html

"值: \(b)"
来源：http://hz.hnxiangtu.top/gtkzmsdvox.html

[T19] Swift：可选绑定
来源：http://hz.316326.xyz/gtkzipvvzf.html

if let n = opt { print(n) }
来源：http://hz.ydjk.org.cn/gttipdcivp.html

[T20] Swift：数组操作
来源：http://hz.bjfxy.top/gtoganxlsl.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yangfankeji.com/gtjfgncsyg.html

[T21] Swift：遍历
来源：http://hz.xuanzx.com/gtmejratkb.html

for x in a { print(x) }
来源：http://hz.smart0.xyz/gttucbikgt.html

[T22] Swift：字典
来源：http://hz.9152youxi.cn/gtoautjqym.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hywenlv.cn/gttxygsgqr.html

[T23] Swift：函数
来源：http://hz.nanxuanxn.top/gtsprdsibl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cashguo.top/gtdlrftnrp.html

[T24] Swift：闭包
来源：http://hz.guowangkeji.top/gtxfzcsxrt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.vqdsnc.cn/gtbcoumyvb.html

[T25] Swift：结构体
来源：http://hz.yonumen.top/gtyddeyevq.html

struct P { var x: Int }
来源：http://hz.ppjwa.cn/gtbxyrcmpj.html

[T26] Swift：类与重写
来源：http://hz.sweek.top/gtnqbcfhbg.html

class A: Base { override func f() {} }
来源：http://hz.hongshengwenyu.top/gtupttzpaz.html

[T27] Swift：错误处理
来源：http://hz.jiagoushi.top/gtpddrwolj.html

do { try f() } catch { print(error) }
来源：http://hz.zhiwuduotai.top/gtlupausgw.html

[T28] Swift：枚举
来源：http://hz.mhx1999.top/gtywnweigb.html

enum Color { case red, green }
来源：http://hz.jinqigfzy.top/gtfnnhzifl.html

[T29] Swift：guard 提前返回
来源：http://hz.gzhubu.top/gtjzfulaen.html

guard let x = opt else { return }
来源：http://hz.birdmap.top/gtxemzpxcl.html

[T30] Swift：协议
来源：http://hz.pengpengdd.cyou/gtupbkrxiy.html

protocol Shape { func area() -> Double }
来源：http://hz.haohaochexian.top/gtshqooqyc.html

[T31] Lua：Hello World
来源：http://hz.jianghu66.top/gtjrhvykny.html

print("Hello")
来源：http://hz.aibaodan.cn/gtauoceinz.html

[T32] Lua：局部变量
来源：http://hz.yanxiufei.cn/gtvoeojkmi.html

local a = 1
来源：http://hz.hnqzz.top/gthgwpixgs.html

[T33] Lua：表（数组）
来源：http://hz.tanke756.top/gtnojftssc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nanxinkj.top/gtupngkezw.html

[T34] Lua：遍历表
来源：http://hz.zycfv.cn/gtdxihqkov.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.wangdashe.top/gtqikmfwiz.html

[T35] Lua：字典表
来源：http://hz.zhongyouzk.top/gtmsddzuly.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ivvv.top/gtdjfkedbo.html

[T36] Lua：函数
来源：http://hz.yangfankeji.com/gtdzciktyd.html

function add(a, b) return a + b end
来源：http://hz.hongshengwenyu.top/gtjdlhaiti.html

[T37] Lua：字符串拼接
来源：http://hz.fengsongda.top/gtbfeemoxh.html

"a" .. "b"
来源：http://hz.cashguo.top/gtodocxpxj.html

[T38] Lua：条件
来源：http://hz.316326.xyz/gtxmbzpfrd.html

if x > 0 then print("正") end
来源：http://hz.hnqzz.top/gtgwjpigfh.html

[T39] Lua：模式匹配
来源：http://hz.chenlongwang.top/gtubpntdbm.html

string.find(s, "%d+")
来源：http://hz.xylfe.cn/gtbulvhkfv.html

[T40] Lua：元表
来源：http://hz.c1oappe.top/gtvxgaxatk.html

setmetatable({}, { __index = base })
来源：http://hz.chenlongwang.top/gtkmvxsyjj.html

[T41] Perl：Hello World
来源：http://hz.ydjk.org.cn/gtfmennsjy.html

print "Hello\n";
来源：http://hz.xuanzx.com/gtimspwyak.html

[T42] Perl：变量类型
来源：http://hz.svipenyu.cn/gtxygrxarm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.hammf.cn/gthapngflz.html

[T43] Perl：字符串插值
来源：http://hz.hfpthk.cn/gtoavdbmrk.html

"值: $a"
来源：http://hz.chenzaomai.com/gtxukmrhlj.html

[T44] Perl：条件
来源：http://hz.cdnleiting.top/gtfejidaui.html

if ($a > 0) { print "正"; }
来源：http://hz.pengpengdd.cyou/gtqucewhfc.html

[T45] Perl：数组遍历
来源：http://hz.316326.xyz/gtlqxztwxc.html

for my $x (@arr) { print $x; }
来源：http://hz.birdmap.top/gtqytjfrnk.html

[T46] Perl：哈希操作
来源：http://hz.jlsjyb.cn/gtjbfwspdz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hysaishi.cn/gtzohfknxh.html

[T47] Perl：正则捕获
来源：http://hz.hfpthk.cn/gtfjtmlsuw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cashguo.top/gtxgpjolzt.html

[T48] Perl：正则替换
来源：http://hz.xinyue.icu/gtmevashhe.html

$s =~ s/old/new/g;
来源：http://hz.yj202588.top/gtvlzwrqwl.html

[T49] Perl：函数
来源：http://hz.ehwqpu.com/gttfjwutqe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.haohaochexian.top/gtxjhbgpeu.html

[T50] Perl：逐行读文件
来源：http://hz.yvedp.cn/gtvoiaovzr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cashguo.top/gtzfvugbib.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jiagoushi.top/gtornrtfrm.html

[T51] Scala：Hello World
来源：http://hz.shanyushiyangkeji.top/gtunoxavny.html

println("Hello")
来源：http://hz.smart0.xyz/gtwrxzuojd.html

[T52] Scala：变量
来源：http://hz.meibo888.top/gtbqmrvsyz.html

val a = 1;  var b = 2
来源：http://hz.shangyingyoupin.top/gtfwuiudcq.html

[T53] Scala：字符串插值
来源：http://hz.zdqjudy.top/gtyblbqakd.html

s"值: $b"
来源：http://hz.jinyuanbaomall.cn/gtayvxtqaj.html

[T54] Scala：集合映射
来源：http://hz.yj20258888.top/gtdminptob.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.dashuyun.cn/gtabpnpvnm.html

[T55] Scala：集合过滤
来源：http://hz.jinqigufen.top/gtrbugjgit.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.dianchejie.cn/gtgjzahutl.html

[T56] Scala：样例类
来源：http://hz.jqgufenzy.top/gtpmzrhjej.html

case class User(name: String, age: Int)
来源：http://hz.hywenlv.cn/gtzzutewiy.html

[T57] Scala：模式匹配
来源：http://hz.cashguo.top/gtmmmaqosd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yangfankeji.com/gtculknhza.html

[T58] Scala：函数定义
来源：http://hz.yj202588.top/gtahpwnqye.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.xinyue.icu/gtbziysbfe.html

[T59] Scala：循环
来源：http://hz.yangfankeji.com/gtzlabwvdp.html

for (i <- 1 to 10) println(i)
来源：http://hz.cqqwz.cn/gtnglrbpoi.html

[T60] Scala：折叠
来源：http://hz.haohaochexian.top/gtqvohhpxx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenjidiqi.icu/gtccvmkuth.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgojkijhq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yanxiufei.cn/gtmqympwih.html

================================================================================
来源：http://hz.aizwys.cn/gtdfclfrpd.html

[U01] Py：创建虚拟环境
来源：http://hz.yongpay.top/gtehcgtely.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.nanxinkj.top/gtssbkjkvg.html

[U02] Py：导出 / 安装依赖
来源：http://hz.andypj.xyz/gtlwqoirdd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.chenlongwang.top/gtgsnqpygc.html

[U03] Py：加载 .env 配置
来源：http://hz.zhiwuduotai.top/gtkwhwoeel.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zhaomingkeji.xyz/gtegnjwlle.html

[U04] Py：变量调试打印
来源：http://hz.mhx1999.top/gtthkjzjtq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ydjk.org.cn/gtnjolajoy.html

[U05] Py：列表去重且保序
来源：http://hz.svipenyu.cn/gtesxlhala.html

list(dict.fromkeys(arr))
来源：http://hz.feifeiyinyue.top/gtcxotoyjc.html

[U06] Py：合并两个字典
来源：http://hz.chenzaomai.com/gtzsvuzcfz.html

{**a, **b}
来源：http://hz.haohaochexian.top/gtagfgxwov.html

[U07] Py：反转字典键值
来源：http://hz.yuxming.cn/gtdbdeyleb.html

{v: k for k, v in d.items()}
来源：http://hz.zycfv.cn/gtxhgjmoyt.html

[U08] Py：展平二维列表
来源：http://hz.xuetiantiany.cn/gtrhxmeyoi.html

[y for x in nested for y in x]
来源：http://hz.sufxvd.cn/gtsyakkqhz.html

[U09] Py：字典取最大值的键
来源：http://hz.cqqwz.cn/gtxkfzydbl.html

max(d, key=d.get)
来源：http://hz.meibo888.top/gtmghcaubg.html

[U10] Py：按值排序字典
来源：http://hz.bjfxy.top/gtwcsihihf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.zhoulong.xyz/gtufonobso.html

[U11] Py：生成器表达式
来源：http://hz.cdnleiting.top/gtribotpqv.html

(x * 2 for x in arr)
来源：http://hz.aizwys.cn/gtxaeesbqf.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.nanxuanxn.top/gtkshtsbye.html

Counter(arr).most_common(3)
来源：http://hz.andypj.xyz/gtpuafxxmz.html

[U13] Py：固定长度队列
来源：http://hz.aibaodan.cn/gtmbmlffau.html

deque(maxlen=10)
来源：http://hz.sufxvd.cn/gtqokexcwg.html

[U14] Py：分组收集到列表
来源：http://hz.hammf.cn/gtkmknzuxh.html

defaultdict(list)
来源：http://hz.gaohongyu789.top/gtlroqazsl.html

[U15] Py：高精度计时
来源：http://hz.zhiwuduotai.top/gtuscnixjr.html

t = time.perf_counter()
来源：http://hz.feifeiyinyue.top/gtvnzcrvdl.html

[U16] Py：命令行参数解析
来源：http://hz.chenzaomai.com/gtusnctljb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cucudq.cn/gtbfyhnkbr.html

[U17] Py：初始化日志
来源：http://hz.nwbrower.top/gtiphinyaa.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.ybcxt.top/gttrxgwhoo.html

[U18] Py：预编译正则
来源：http://hz.jinyuanbaomall.cn/gtmsrlemko.html

pat = re.compile(r"\d+")
来源：http://hz.0kj1m.cn/gttujrtmyb.html

[U19] Py：正则替换带回调
来源：http://hz.jianghu66.top/gtkqhbtorl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jqgfzy.top/gtoaoqrdmo.html

[U20] Py：缓存函数结果
来源：http://hz.daxiang520.top/gtwwdnlpke.html

@functools.lru_cache(maxsize=None)
来源：http://hz.316326.xyz/gtxauoxbsm.html

[U21] Py：自定义上下文管理器
来源：http://hz.yuanzhike.top/gtjkzodoed.html

@contextlib.contextmanager
来源：http://hz.meibo888.top/gtlsuwprnk.html

[U22] Py：矩阵转置
来源：http://hz.hfpthk.cn/gtnpmtcnsw.html

list(zip(*m))
来源：http://hz.jiagoushi.top/gtndtpgiyn.html

[U23] Py：分块读取大文件
来源：http://hz.jlsjyb.cn/gtydmwsrhq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.zhaomingkeji.xyz/gtclcwmlnc.html

[U24] Py：路径操作
来源：http://hz.havefunace.top/gtaicwjpgt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.dianchejie.cn/gtnrcricfy.html

[U25] Py：CSV 按字典读
来源：http://hz.daria6918.cn/gttlswbwth.html

csv.DictReader(f)
来源：http://hz.cucudq.cn/gtbsrtvlmr.html

[U26] Py：并发下载
来源：http://hz.chenzaomai.com/gtrlplefga.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.aizwys.cn/gtqhcyptlj.html

[U27] Py：异步 HTTP
来源：http://hz.zhijiandao.cn/gtvunbynwg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ydzc1.top/gttanxybot.html

[U28] Py：类型别名
来源：http://hz.tian-w.cn/gtegmmuofv.html

UserId = int
来源：http://hz.nanxinkj.top/gtzxitnpls.html

[U29] Py：属性校验
来源：http://hz.zhiwuduotai.top/gttvjknnqq.html

@property 与 @x.setter 配合
来源：http://hz.cucudq.cn/gtsehjpglx.html

[U30] Py：数据类
来源：http://hz.cucudq.cn/gtxzkyblrp.html

@dataclass(slots=True)
来源：http://hz.xziqi.cn/gttrmhhdkz.html

[U31] Py：单测
来源：http://hz.xziqi.cn/gtslskflea.html

python -m pytest -q
来源：http://hz.feifeiyinyue.top/gttnoqgvos.html

[U32] Py：代码格式化
来源：http://hz.gotoacloud.top/gtbqaskfwu.html

ruff format . && ruff check --fix .
来源：http://hz.yj20258888.top/gtblytmsvq.html

[U33] Py：打包发布
来源：http://hz.ydjk.org.cn/gtbdflfahk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.shzxlz.cn/gteyulhbhe.html

[U34] Py：判断编码
来源：http://hz.ivvv.top/gtprzaunqd.html

chardet.detect(raw)
来源：http://hz.xziqi.cn/gtxykfvmof.html

[U35] Py：发送邮件
来源：http://hz.haohaochexian.top/gtyxuspwnt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xuetiantiany.cn/gtmypsukdq.html

[U36] Py：定时任务
来源：http://hz.hfpthk.cn/gtmjsgeqld.html

schedule.every(10).minutes.do(job)
来源：http://hz.xingfuxueyuan.xyz/gtpxfobhzq.html

[U37] Py：读写 Excel
来源：http://hz.fengsongda.top/gtixkvtaai.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.jyoumei.cn/gtmhydliml.html

[U38] Py：获取脚本所在目录
来源：http://hz.hammf.cn/gteqzqrgto.html

Path(__file__).resolve().parent
来源：http://hz.chenjidiqi.icu/gtaaxpeger.html

[U39] Py：判断是否在交互环境
来源：http://hz.meibo888.top/gtvhxeggwl.html

sys.stdout.isatty()
来源：http://hz.xylfe.cn/gthpwwvevn.html

[U40] Py：打印到标准错误
来源：http://hz.ydzc1.top/gtklbfjcka.html

print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtaugatjeh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.sweek.top/gtezqjjwii.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.cheryme.top/gtpanzumhc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.ydjk.org.cn/gtvoblqhal.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hysaishi.cn/gtkjvefpam.html

[U43] PHP：声明命名空间
来源：http://hz.xylfe.cn/gtyotosrrr.html

namespace App\Http;
来源：http://hz.guowangkeji.top/gttzrngith.html

[U44] PHP：开启严格类型
来源：http://hz.dianchejie.cn/gtmbhixrcc.html

declare(strict_types=1);
来源：http://hz.nwbrower.top/gtweuxdvvv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.fzhhl.top/gtpdrptwaz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gtlsxkbhye.html

[U46] PHP：可空类型
来源：http://hz.andypj.xyz/gttlwtuuxj.html

?string $name = null
来源：http://hz.jyoumei.cn/gtutdqdnda.html

[U47] PHP：联合类型
来源：http://hz.tianlin.xyz/gthfwrkclh.html

int|string $id
来源：http://hz.chenjidiqi.icu/gtokwiwtij.html

[U48] PHP：纯枚举
来源：http://hz.fzhhl.top/gtlijlcuhs.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.snrcjt.cn/gtwmpbqxvd.html

[U49] PHP：只读属性
来源：http://hz.zhiwuduotai.top/gtxaixnqty.html

public readonly string $name
来源：http://hz.jianghu66.top/gtiwzbxczv.html

[U50] PHP：构造器属性提升
来源：http://hz.andypj.xyz/gtcsxfzqmm.html

public function __construct(private int $id) {}
来源：http://hz.cheryme.top/gtxasfhlke.html

[U51] PHP：数组解构
来源：http://hz.c1oappe.top/gtpqicwrkw.html

[$a, $b] = $arr;
来源：http://hz.ivvv.top/gtucfrqrtd.html

[U52] PHP：箭头函数
来源：http://hz.haohaochexian.top/gtixfqbjha.html

$double = fn($x) => $x * 2;
来源：http://hz.jianghu66.top/gthtlvoizi.html

[U53] PHP：空合并运算符
来源：http://hz.xinyue.icu/gtuyeaanfh.html

$v = $a ?? $b ?? "default";
来源：http://hz.gogol.net.cn/gtnmyfyisg.html

[U54] PHP：空安全调用
来源：http://hz.guannengcc.top/gtreqrzmxu.html

$obj?->method()
来源：http://hz.dianchejie.cn/gtrzdnltta.html

[U55] PHP：match 表达式
来源：http://hz.snrcjt.cn/gtnjxfmhev.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.mhx1999.top/gtxywyioft.html

[U56] PHP：命名参数
来源：http://hz.quarkkingdee.top/gtpoocuzms.html

f(a: 1, b: 2)
来源：http://hz.yj20258.top/gtonmurctc.html

[U57] PHP：字符串插值
来源：http://hz.aibaodan.cn/gtszfvduzt.html

"值: {$a}"
来源：http://hz.ydjk.org.cn/gtksjizohl.html

[U58] PHP：数组三件套
来源：http://hz.shuidangran.top/gtotimzqje.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.svipenyu.cn/gtlmcdsxyx.html

[U59] PHP：自定义排序
来源：http://hz.shuidangran.top/gtbrbtfoir.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gtekzaibph.html

[U60] PHP：JSON 编解码
来源：http://hz.snrcjt.cn/gtmtvsiggn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.xuanzx.com/gtbxrppbwe.html

[U61] PHP：正则
来源：http://hz.yj202588.top/gtrfxljzac.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydjk.org.cn/gthsyvrhzv.html

[U62] PHP：日期对象
来源：http://hz.havefunace.top/gtnwfavalp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.9152youxi.cn/gtqpsfykqv.html

[U63] PHP：文件读写
来源：http://hz.hysaishi.cn/gtlixvrwtu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.cucudq.cn/gtvvrlbyyq.html

[U64] PHP：目录遍历
来源：http://hz.zdqjudy.top/gtatixxjtq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sysykeji.top/gtkvhgpxac.html


<!-- 参考信息 -->