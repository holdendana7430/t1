代发 wailian999

[S41] C++：类与构造函数
来源：http://hz.guowangkeji.top/gtnibhlmoa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cucudq.cn/gtbzfktyqj.html

[S42] C++：继承与虚函数
来源：http://hz.jlsjyb.cn/gtbbblglfi.html

class B : public Base { public: void f() override {} };
来源：http://hz.xuetiantiany.cn/gtwinhgdlj.html

[S43] C++：智能指针
来源：http://hz.9152youxi.cn/gtylzefciy.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxinkj.top/gtuietpkoq.html

[S44] C++：引用传参
来源：http://hz.zhengqikj.top/gtqmgbhsls.html

void inc(int &x) { ++x; }
来源：http://hz.quarkkingdee.top/gtcawyytoj.html

[S45] C++：lambda
来源：http://hz.ehwqpu.com/gtkqgpxvmo.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yanxiufei.cn/gtipvzxmtn.html

[S46] C++：函数模板
来源：http://hz.c1oappe.top/gtkmkiugwf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zdqjudy.top/gtnijnbaiu.html

[S47] C++：结构化绑定遍历
来源：http://hz.yangfankeji.com/gtjluenxeh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jqgufenzy.top/gtqjpogbux.html

[S48] C++：逐行读文件
来源：http://hz.hammf.cn/gtzdztnnso.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sweek.top/gtsdrpanaa.html

while (std::getline(in, line)) { }
来源：http://hz.zhongyouzk.top/gtxadvzmjf.html

[S49] C++：写文件
来源：http://hz.yuanzhike.top/gttfzdzcdc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xuanzx.com/gtkpjkxvvq.html

[S50] C++：格式化数字
来源：http://hz.andypj.xyz/gttqdkbnyj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.0kj1m.cn/gtcmmtxxka.html

[S51] C++：显式类型转换
来源：http://hz.hammf.cn/gtcedyoxxp.html

static_cast<double>(a) / b
来源：http://hz.daria6918.cn/gtzycptjel.html

[S52] C++：const 与 noexcept
来源：http://hz.jinqigfzy.top/gtxwutplyl.html

int size() const noexcept { return n_; }
来源：http://hz.cucudq.cn/gtjikiitpz.html

[S53] C++：移动语义
来源：http://hz.pengpengdd.cyou/gtlvskzpbl.html

std::vector<int> w = std::move(v);
来源：http://hz.52xcode.cn/gtdzgolwhe.html

[S54] C++：异常处理
来源：http://hz.meibo888.top/gthyozubbj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yonumen.top/gtfoypeejm.html

[S55] C++：结构化绑定
来源：http://hz.chenjidiqi.icu/gtefrgwksq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.daxiang520.top/gtnkbmsfdd.html

[S56] C++：optional
来源：http://hz.birdmap.top/gtcwfanukt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jyoumei.cn/gtkbqbsstq.html

[S57] C++：编译期常量
来源：http://hz.sxryk.cn/gtzuiecnoz.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gtajunbjhs.html

[S58] C++：命名空间
来源：http://hz.gzhubu.top/gtaqbtdspq.html

namespace ns { int f() { return 1; } }
来源：http://hz.dashuyun.cn/gthvsdieyr.html

[S59] C++：静态断言
来源：http://hz.hywenlv.cn/gtyouyfzsw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xylfe.cn/gtigykaqib.html

[S60] C++：遍历并删除元素
来源：http://hz.nanxuanxn.top/gtujevnyvo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xinyue.icu/gtjxciwett.html

================================================================================
来源：http://hz.0kj1m.cn/gtablysipk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.0kj1m.cn/gtiiqshozf.html

================================================================================
来源：http://hz.xuanzx.com/gtzquxjlnd.html

[T01] Kotlin：Hello World
来源：http://hz.zhengqikj.top/gtgcmhjkui.html

println("Hello")
来源：http://hz.gaohongyu789.top/gtcsgdovie.html

[T02] Kotlin：变量
来源：http://hz.yongpay.top/gtjpjnjgso.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj20258888.top/gtbqexowwz.html

[T03] Kotlin：字符串模板
来源：http://hz.vqdsnc.cn/gtggeaambk.html

"值: $b"
来源：http://hz.jianghu66.top/gtjgvqazlo.html

[T04] Kotlin：空安全
来源：http://hz.aibaodan.cn/gttcunjemh.html

val n: String? = null;  n?.length
来源：http://hz.yvedp.cn/gtguspcxul.html

[T05] Kotlin：when 表达式
来源：http://hz.jiagoushi.top/gtfwqsican.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cqqwz.cn/gtzriesdso.html

[T06] Kotlin：集合映射
来源：http://hz.ehwqpu.com/gtuuwrotvq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yuxming.cn/gtnwwiosnc.html

[T07] Kotlin：集合过滤
来源：http://hz.jianghu66.top/gtftttteag.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj202588.top/gtxhxoikwn.html

[T08] Kotlin：数据类
来源：http://hz.cashguo.top/gtdlzgtwcp.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gtvplozlmm.html

[T09] Kotlin：扩展函数
来源：http://hz.guannengcc.top/gtveewzszb.html

fun String.exclaim() = this + "!"
来源：http://hz.kuanghao11.cn/gtrtooiwdg.html

[T10] Kotlin：默认参数
来源：http://hz.birdmap.top/gtzcduqhwu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xingfuxueyuan.xyz/gtoebbkisw.html

[T11] Kotlin：协程
来源：http://hz.cucudq.cn/gtwtljcbbz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gzhubu.top/gtiipdrzhe.html

[T12] Kotlin：解构声明
来源：http://hz.yangfankeji.com/gtygektizu.html

val (a, b) = Pair(1, 2)
来源：http://hz.aizwys.cn/gtsqasweyu.html

[T13] Kotlin：只读 Map
来源：http://hz.zdqjudy.top/gtqskphxph.html

val m = mapOf("a" to 1)
来源：http://hz.chenzaomai.com/gtmxpuztcr.html

[T14] Kotlin：循环
来源：http://hz.xingfuxueyuan.xyz/gtiztaptql.html

for (i in 1..10) println(i)
来源：http://hz.chenzaomai.com/gtnjbbwmlr.html

[T15] Kotlin：接口
来源：http://hz.ybcxt.top/gtcyekpaxr.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258888.top/gtsmimffnx.html

[T16] Swift：Hello World
来源：http://hz.jlsjyb.cn/gtcbzqwsfo.html

print("Hello")
来源：http://hz.316326.xyz/gtcevntfao.html

[T17] Swift：变量与常量
来源：http://hz.zhongyouzk.top/gttxexunxl.html

var a = 1;  let b = 2
来源：http://hz.quarkkingdee.top/gtmzmnjsxd.html

[T18] Swift：字符串插值
来源：http://hz.shangyingyoupin.top/gtearzhamk.html

"值: \(b)"
来源：http://hz.ydjk.org.cn/gtwqdpyjoj.html

[T19] Swift：可选绑定
来源：http://hz.jinghuilouyu.cn/gtjbmtybio.html

if let n = opt { print(n) }
来源：http://hz.mhx1999.top/gtyktnbaqu.html

[T20] Swift：数组操作
来源：http://hz.zhaomingkeji.xyz/gtngbkjitw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hongshengwenyu.top/gtjceihpap.html

[T21] Swift：遍历
来源：http://hz.guowangkeji.top/gtrzvonpit.html

for x in a { print(x) }
来源：http://hz.ydjk.org.cn/gtiehggfrs.html

[T22] Swift：字典
来源：http://hz.yonumen.top/gtnslmzinu.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhoulong.xyz/gtrtstwgoo.html

[T23] Swift：函数
来源：http://hz.zhaomingkeji.xyz/gtcxrwidse.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhijiandao.cn/gtguxrcjfb.html

[T24] Swift：闭包
来源：http://hz.hammf.cn/gtffutltbl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhiwuduotai.top/gtvxoquics.html

[T25] Swift：结构体
来源：http://hz.hongshengwenyu.top/gtcoehpljz.html

struct P { var x: Int }
来源：http://hz.tian-w.cn/gtupykgdch.html

[T26] Swift：类与重写
来源：http://hz.hywenlv.cn/gthdetninu.html

class A: Base { override func f() {} }
来源：http://hz.wangdashe.top/gtkeujmvcs.html

[T27] Swift：错误处理
来源：http://hz.daxiang520.top/gtvnuxdndf.html

do { try f() } catch { print(error) }
来源：http://hz.chenjidiqi.icu/gtfuuzcwvq.html

[T28] Swift：枚举
来源：http://hz.wangdashe.top/gtghskqjbq.html

enum Color { case red, green }
来源：http://hz.hfpthk.cn/gtpyqvdxst.html

[T29] Swift：guard 提前返回
来源：http://hz.sysykeji.top/gtctrxvgim.html

guard let x = opt else { return }
来源：http://hz.cdnleiting.top/gtcqniusur.html

[T30] Swift：协议
来源：http://hz.chenlongwang.top/gtacvzfrnk.html

protocol Shape { func area() -> Double }
来源：http://hz.sweek.top/gtcybkwxmk.html

[T31] Lua：Hello World
来源：http://hz.hywenlv.cn/gtovorwend.html

print("Hello")
来源：http://hz.zhoulong.xyz/gtekbnrpil.html

[T32] Lua：局部变量
来源：http://hz.shuidangran.top/gtpvapfxmr.html

local a = 1
来源：http://hz.gotoacloud.top/gtowfronfm.html

[T33] Lua：表（数组）
来源：http://hz.316326.xyz/gtwittkhph.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nwbrower.top/gtpjmilwkj.html

[T34] Lua：遍历表
来源：http://hz.ivvv.top/gtvabzbiqr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.hysaishi.cn/gtwlmtiuif.html

[T35] Lua：字典表
来源：http://hz.hywenlv.cn/gtxuozxcse.html

local d = { a = 1 };  d.b = 2
来源：http://hz.nwbrower.top/gtgfvwuvfv.html

[T36] Lua：函数
来源：http://hz.yj202588.top/gtrlbsoohy.html

function add(a, b) return a + b end
来源：http://hz.xingfuxueyuan.xyz/gtnyqxuhiq.html

[T37] Lua：字符串拼接
来源：http://hz.cqqwz.cn/gtmklreyvw.html

"a" .. "b"
来源：http://hz.feifeiyinyue.top/gtztwbzkgh.html

[T38] Lua：条件
来源：http://hz.c1oappe.top/gtwdzgbzen.html

if x > 0 then print("正") end
来源：http://hz.dashuyun.cn/gthnreyfoy.html

[T39] Lua：模式匹配
来源：http://hz.sweek.top/gtgcprnsek.html

string.find(s, "%d+")
来源：http://hz.jinqigufen.top/gthhemvamo.html

[T40] Lua：元表
来源：http://hz.dashuyun.cn/gtkwchwtqo.html

setmetatable({}, { __index = base })
来源：http://hz.haohaochexian.top/gtdmdqrwud.html

[T41] Perl：Hello World
来源：http://hz.redwolf501.top/gtbafnotif.html

print "Hello\n";
来源：http://hz.svipenyu.cn/gtdqgqybgy.html

[T42] Perl：变量类型
来源：http://hz.smart0.xyz/gtccczmlhe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ehwqpu.com/gtxwuclpjn.html

[T43] Perl：字符串插值
来源：http://hz.shuidangran.top/gtdzakbmgq.html

"值: $a"
来源：http://hz.jinqigufen.top/gthqqyhmrx.html

[T44] Perl：条件
来源：http://hz.snrcjt.cn/gtxuakocmd.html

if ($a > 0) { print "正"; }
来源：http://hz.jinqigufen.top/gtcqbmhwce.html

[T45] Perl：数组遍历
来源：http://hz.ydjk.org.cn/gtopmnixqg.html

for my $x (@arr) { print $x; }
来源：http://hz.zdqjudy.top/gtovmzhkcq.html

[T46] Perl：哈希操作
来源：http://hz.cucudq.cn/gthmlczrbx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xuetiantiany.cn/gtshruwuwh.html

[T47] Perl：正则捕获
来源：http://hz.hysaishi.cn/gtwpkvvfxv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.smart0.xyz/gtpucpqxuq.html

[T48] Perl：正则替换
来源：http://hz.haohaochexian.top/gtgjyrjfic.html

$s =~ s/old/new/g;
来源：http://hz.havefunace.top/gtfaljlwqj.html

[T49] Perl：函数
来源：http://hz.zhaomingkeji.xyz/gtbeesiicm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.0kj1m.cn/gtsopvkrvn.html

[T50] Perl：逐行读文件
来源：http://hz.hongshengwenyu.top/gtnrbmvoxn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cdnleiting.top/gtvhoivzwj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zycfv.cn/gtxzjcfklj.html

[T51] Scala：Hello World
来源：http://hz.hnxiangtu.top/gtvxjvdlwp.html

println("Hello")
来源：http://hz.jqgufenzy.top/gtioxnnltg.html

[T52] Scala：变量
来源：http://hz.birdmap.top/gtdnwhzniy.html

val a = 1;  var b = 2
来源：http://hz.jianghu66.top/gtktkbtclf.html

[T53] Scala：字符串插值
来源：http://hz.sysykeji.top/gtutpexgcx.html

s"值: $b"
来源：http://hz.daria6918.cn/gtuzijrdgy.html

[T54] Scala：集合映射
来源：http://hz.jqgufenzy.top/gtmzctdpca.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xziqi.cn/gtmhzroanx.html

[T55] Scala：集合过滤
来源：http://hz.vqdsnc.cn/gthdyxhnpg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.vqdsnc.cn/gtyzenovhu.html

[T56] Scala：样例类
来源：http://hz.nwbrower.top/gtblvzygrt.html

case class User(name: String, age: Int)
来源：http://hz.sysykeji.top/gtnuckiwmk.html

[T57] Scala：模式匹配
来源：http://hz.yongpay.top/gtifjnsvfd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.vqdsnc.cn/gtoffkgzjd.html

[T58] Scala：函数定义
来源：http://hz.smart0.xyz/gtgkrhpcle.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shanyushiyangtech.top/gtdrjhwzbl.html

[T59] Scala：循环
来源：http://hz.vqdsnc.cn/gtbahuwjdk.html

for (i <- 1 to 10) println(i)
来源：http://hz.hysaishi.cn/gtckpkjtge.html

[T60] Scala：折叠
来源：http://hz.zhengqikj.top/gtgjqpgwpi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sufxvd.cn/gtbtklekgf.html

================================================================================
来源：http://hz.tian-w.cn/gtkrulykxx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gtdtactwsk.html

================================================================================
来源：http://hz.birdmap.top/gtkeqnhyrl.html

[U01] Py：创建虚拟环境
来源：http://hz.hysaishi.cn/gtdeejbekv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sxryk.cn/gtvwudopna.html

[U02] Py：导出 / 安装依赖
来源：http://hz.nwbrower.top/gtkjhwzdiw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yongpay.top/gtoymaawxj.html

[U03] Py：加载 .env 配置
来源：http://hz.yueranfly.top/gttavxuvrj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.fzhhl.top/gthzughjdt.html

[U04] Py：变量调试打印
来源：http://hz.yvedp.cn/gtgdamwjhl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.ehwqpu.com/gtnfztmmhl.html

[U05] Py：列表去重且保序
来源：http://hz.xziqi.cn/gtexuiohus.html

list(dict.fromkeys(arr))
来源：http://hz.xinyue.icu/gtybfsnlmq.html

[U06] Py：合并两个字典
来源：http://hz.jiagoushi.top/gtupicvsqv.html

{**a, **b}
来源：http://hz.yj202588.top/gttbuosqgb.html

[U07] Py：反转字典键值
来源：http://hz.jinyuanbaomall.cn/gtuoxfbwkj.html

{v: k for k, v in d.items()}
来源：http://hz.ppjwa.cn/gtlenfgjci.html

[U08] Py：展平二维列表
来源：http://hz.chenjidiqi.icu/gthcseaioi.html

[y for x in nested for y in x]
来源：http://hz.yangfankeji.com/gtqwvyuesc.html

[U09] Py：字典取最大值的键
来源：http://hz.tianlin.xyz/gtazruweqs.html

max(d, key=d.get)
来源：http://hz.pengpengdd.cyou/gtoekekokj.html

[U10] Py：按值排序字典
来源：http://hz.zhixingplan.top/gtjfbvypqc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.aibaodan.cn/gtpeujkqkd.html

[U11] Py：生成器表达式
来源：http://hz.feifeiyinyue.top/gtpupfmhyj.html

(x * 2 for x in arr)
来源：http://hz.nwbrower.top/gtlrpiyznn.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.zhijiandao.cn/gtcgjksmri.html

Counter(arr).most_common(3)
来源：http://hz.ivvv.top/gttejdxcrz.html

[U13] Py：固定长度队列
来源：http://hz.cucudq.cn/gtbocjvdyq.html

deque(maxlen=10)
来源：http://hz.gzhubu.top/gtodvssqpf.html

[U14] Py：分组收集到列表
来源：http://hz.snrcjt.cn/gtbfguwpzd.html

defaultdict(list)
来源：http://hz.hywenlv.cn/gtcfuuwoan.html

[U15] Py：高精度计时
来源：http://hz.meibo888.top/gtybpuetdp.html

t = time.perf_counter()
来源：http://hz.xziqi.cn/gtabvydqht.html

[U16] Py：命令行参数解析
来源：http://hz.tianlin.xyz/gtrzqseyqs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.vqdsnc.cn/gtaqbxtuzb.html

[U17] Py：初始化日志
来源：http://hz.ivvv.top/gtunduwjyj.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.sufxvd.cn/gtayuespet.html

[U18] Py：预编译正则
来源：http://hz.tian-w.cn/gtdwvmkowa.html

pat = re.compile(r"\d+")
来源：http://hz.sweek.top/gtxsdoqnfa.html

[U19] Py：正则替换带回调
来源：http://hz.gaohongyu789.top/gtfrbuhbcy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jyoumei.cn/gttwiburcr.html

[U20] Py：缓存函数结果
来源：http://hz.zycfv.cn/gtjbbhahds.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinqigfzy.top/gtlkmquses.html

[U21] Py：自定义上下文管理器
来源：http://hz.ybcxt.top/gtctjovinh.html

@contextlib.contextmanager
来源：http://hz.yj202588.top/gtrzuskfai.html

[U22] Py：矩阵转置
来源：http://hz.hnxiangtu.top/gtrfuwyruv.html

list(zip(*m))
来源：http://hz.shuidangran.top/gtcfkrzpbs.html

[U23] Py：分块读取大文件
来源：http://hz.hnqzz.top/gtwhdecmlq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.birdmap.top/gtqpcwdirq.html

[U24] Py：路径操作
来源：http://hz.pycfn.com/gtnmqfurvo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.daxiang520.top/gtpvtynvwi.html

[U25] Py：CSV 按字典读
来源：http://hz.hfpthk.cn/gtyrcvebqn.html

csv.DictReader(f)
来源：http://hz.fengsongda.top/gtzuyhztkz.html

[U26] Py：并发下载
来源：http://hz.gotoacloud.top/gtqzcxebpo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.havefunace.top/gtukkdsaxd.html

[U27] Py：异步 HTTP
来源：http://hz.fengsongda.top/gtmorvddnn.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ppjwa.cn/gtnbhcreuy.html

[U28] Py：类型别名
来源：http://hz.guowangkeji.top/gtgmfnfdhr.html

UserId = int
来源：http://hz.chenjidiqi.icu/gtxtshhptm.html

[U29] Py：属性校验
来源：http://hz.jlsjyb.cn/gtbmdwrkfb.html

@property 与 @x.setter 配合
来源：http://hz.ywan-chungtsiang.top/gtlsnmnmcn.html

[U30] Py：数据类
来源：http://hz.9152youxi.cn/gtrvqksiwi.html

@dataclass(slots=True)
来源：http://hz.shanyushiyangtech.top/gtwiyhxvku.html

[U31] Py：单测
来源：http://hz.chenjidiqi.icu/gttbjnynxa.html

python -m pytest -q
来源：http://hz.pengpengdd.cyou/gtbgjrtbff.html

[U32] Py：代码格式化
来源：http://hz.guannengcc.top/gthttrhjuq.html

ruff format . && ruff check --fix .
来源：http://hz.bjfxy.top/gtujvafbpd.html

[U33] Py：打包发布
来源：http://hz.sxryk.cn/gtvhmrkatu.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hongshengwenyu.top/gtmlurjtzt.html

[U34] Py：判断编码
来源：http://hz.yvedp.cn/gtbccadbwm.html

chardet.detect(raw)
来源：http://hz.guannengcc.top/gtievuviiy.html

[U35] Py：发送邮件
来源：http://hz.yj202588.top/gtzoqzqoft.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.0kj1m.cn/gtyqdoswow.html

[U36] Py：定时任务
来源：http://hz.fzhhl.top/gtdhslcfkd.html

schedule.every(10).minutes.do(job)
来源：http://hz.jinqigfzy.top/gtnrbrwqyb.html

[U37] Py：读写 Excel
来源：http://hz.shangyingyoupin.top/gtynnkomgw.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.tianlin.xyz/gtpvurptvh.html

[U38] Py：获取脚本所在目录
来源：http://hz.fengsongda.top/gtrsvstmty.html

Path(__file__).resolve().parent
来源：http://hz.yonumen.top/gtncdqcowk.html

[U39] Py：判断是否在交互环境
来源：http://hz.sweek.top/gtahixrauh.html

sys.stdout.isatty()
来源：http://hz.quarkkingdee.top/gtbuerktjn.html

[U40] Py：打印到标准错误
来源：http://hz.nanxinkj.top/gtydpfbvwr.html

print("err", file=sys.stderr)
来源：http://hz.zhoulong.xyz/gtohhttuow.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yanxiufei.cn/gttnikoivt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ybcxt.top/gtkzwnsoxt.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sysykeji.top/gtwryyaibp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yj20258888.top/gtggdzkaaz.html

[U43] PHP：声明命名空间
来源：http://hz.tanke756.top/gtpykxmkrm.html

namespace App\Http;
来源：http://hz.sysykeji.top/gtafcgzjha.html

[U44] PHP：开启严格类型
来源：http://hz.yonumen.top/gtchdqovli.html

declare(strict_types=1);
来源：http://hz.guowangkeji.top/gtfdypezat.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jyoumei.cn/gtwcetxbhm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtptvmdark.html

[U46] PHP：可空类型
来源：http://hz.9152youxi.cn/gtzhwbznyc.html

?string $name = null
来源：http://hz.ywan-chungtsiang.top/gtbikrheeq.html

[U47] PHP：联合类型
来源：http://hz.jiagoushi.top/gtfpxaguzf.html

int|string $id
来源：http://hz.52xcode.cn/gtfbczqinj.html

[U48] PHP：纯枚举
来源：http://hz.wangdashe.top/gtsladhbby.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ivvv.top/gtswrokdvk.html

[U49] PHP：只读属性
来源：http://hz.dashuyun.cn/gteyvzbluc.html

public readonly string $name
来源：http://hz.sufxvd.cn/gtrnvgoqek.html

[U50] PHP：构造器属性提升
来源：http://hz.zhixingplan.top/gtzrztruce.html

public function __construct(private int $id) {}
来源：http://hz.gaohongyu789.top/gtfxsjduhs.html

[U51] PHP：数组解构
来源：http://hz.meibo888.top/gtvnfmelty.html

[$a, $b] = $arr;
来源：http://hz.cheryme.top/gtbpwkvasn.html

[U52] PHP：箭头函数
来源：http://hz.birdmap.top/gtmwbmtqbc.html

$double = fn($x) => $x * 2;
来源：http://hz.zhixingplan.top/gtmpvcssve.html

[U53] PHP：空合并运算符
来源：http://hz.cdnleiting.top/gtaocthbga.html

$v = $a ?? $b ?? "default";
来源：http://hz.guowangkeji.top/gtxohqlckk.html

[U54] PHP：空安全调用
来源：http://hz.chenzaomai.com/gtpcovfkvi.html

$obj?->method()
来源：http://hz.zycfv.cn/gtmjzkljzc.html

[U55] PHP：match 表达式
来源：http://hz.birdmap.top/gtpcvbokof.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ivvv.top/gtiabbkpqp.html

[U56] PHP：命名参数
来源：http://hz.shanyushiyangkeji.top/gtpexqwugm.html

f(a: 1, b: 2)
来源：http://hz.yonumen.top/gtlccsnwew.html

[U57] PHP：字符串插值
来源：http://hz.yongpay.top/gtnsenzoxm.html

"值: {$a}"
来源：http://hz.jqgufenzy.top/gtxpgdrzkf.html

[U58] PHP：数组三件套
来源：http://hz.fengsongda.top/gtmzefhycx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jlsjyb.cn/gtgbmsifpi.html

[U59] PHP：自定义排序
来源：http://hz.yj202588.top/gtjxtkjjrz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydjk.org.cn/gtcvwizleb.html

[U60] PHP：JSON 编解码
来源：http://hz.zhoulong.xyz/gtgyatxawv.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.pycfn.com/gtxotohlju.html

[U61] PHP：正则
来源：http://hz.hnqzz.top/gtupyimmgf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.0kj1m.cn/gtvyclznzu.html

[U62] PHP：日期对象
来源：http://hz.shanyushiyangtech.top/gtjzpyywfi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yonumen.top/gtfdevfcov.html

[U63] PHP：文件读写
来源：http://hz.sufxvd.cn/gtsouwtolh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.ppjwa.cn/gteawsvsef.html

[U64] PHP：目录遍历
来源：http://hz.vqdsnc.cn/gtlbdemfoe.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.daria6918.cn/gttiyredqs.html

[U65] PHP：会话
来源：http://hz.vqdsnc.cn/gtdafgayil.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ehwqpu.com/gtnqfbvbhr.html

[U66] PHP：设置 Cookie
来源：http://hz.9152youxi.cn/gtriyayngd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.mhx1999.top/gtwowvflwo.html


<!-- 参考信息 -->