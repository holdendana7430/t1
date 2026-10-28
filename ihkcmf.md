代发 wailian999

[S39] C++：自定义比较器排序
来源：http://hz.snrcjt.cn/gtrbebnofa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jinqigfzy.top/gtxntezbpu.html

[S40] C++：查找元素
来源：http://hz.pycfn.com/gtbkcibxcp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gotoacloud.top/gtjmttjeno.html

[S41] C++：类与构造函数
来源：http://hz.ydzc1.top/gtzclmlrkb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cheryme.top/gttoidvhgb.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtwbwxvggo.html

class B : public Base { public: void f() override {} };
来源：http://hz.hywenlv.cn/gtpmovbrxz.html

[S43] C++：智能指针
来源：http://hz.hongshengwenyu.top/gthvhycude.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinghuilouyu.cn/gtooitbfds.html

[S44] C++：引用传参
来源：http://hz.nanxinkj.top/gtxupmvljp.html

void inc(int &x) { ++x; }
来源：http://hz.nwbrower.top/gtkbwzcivz.html

[S45] C++：lambda
来源：http://hz.aibaodan.cn/gtyvbknlpx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.c1oappe.top/gtjmrbegui.html

[S46] C++：函数模板
来源：http://hz.birdmap.top/gtsclwdsen.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.cashguo.top/gtxiosqedb.html

[S47] C++：结构化绑定遍历
来源：http://hz.ivvv.top/gtxjgpjsiy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tian-w.cn/gtiuncqemj.html

[S48] C++：逐行读文件
来源：http://hz.tanke756.top/gtepbkivph.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhengqikj.top/gtfhjdiuey.html

while (std::getline(in, line)) { }
来源：http://hz.daxiang520.top/gtkzctajic.html

[S49] C++：写文件
来源：http://hz.shuidangran.top/gtyeadqnax.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.52xcode.cn/gtlubdndqf.html

[S50] C++：格式化数字
来源：http://hz.zhoulong.xyz/gtjkhmbvva.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.meibo888.top/gtbjzzeqee.html

[S51] C++：显式类型转换
来源：http://hz.yj20258.top/gtdwlqbrwz.html

static_cast<double>(a) / b
来源：http://hz.ivvv.top/gthukguxbg.html

[S52] C++：const 与 noexcept
来源：http://hz.havefunace.top/gtwvnibpso.html

int size() const noexcept { return n_; }
来源：http://hz.snrcjt.cn/gtzgoovdcz.html

[S53] C++：移动语义
来源：http://hz.xingfuxueyuan.xyz/gtoesvlkrw.html

std::vector<int> w = std::move(v);
来源：http://hz.0kj1m.cn/gtksgdhamx.html

[S54] C++：异常处理
来源：http://hz.ybcxt.top/gtcmywpzca.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj202588.top/gtgiiwhoew.html

[S55] C++：结构化绑定
来源：http://hz.shanyushiyangtech.top/gtccvorjqg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.kuanghao11.cn/gtqfzqkhyn.html

[S56] C++：optional
来源：http://hz.xziqi.cn/gtqewgkwdf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.haohaochexian.top/gtzqaemifa.html

[S57] C++：编译期常量
来源：http://hz.jinqigufen.top/gtiecmkevf.html

constexpr int N = 10;
来源：http://hz.jinqigfzy.top/gtuunzmouy.html

[S58] C++：命名空间
来源：http://hz.shuidangran.top/gtjjizofcn.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangkeji.top/gtfbbmnhik.html

[S59] C++：静态断言
来源：http://hz.zhongyouzk.top/gtosvnnveg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xylfe.cn/gtskuyzjpn.html

[S60] C++：遍历并删除元素
来源：http://hz.mhx1999.top/gtxordmkvf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cheryme.top/gtqmxcthxt.html

================================================================================
来源：http://hz.ehwqpu.com/gtygszpiom.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhoulong.xyz/gtixgtobxs.html

================================================================================
来源：http://hz.shuidangran.top/gtqujfratl.html

[T01] Kotlin：Hello World
来源：http://hz.cdnleiting.top/gtxwwrwzwc.html

println("Hello")
来源：http://hz.jianghu66.top/gtqpshenum.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtkanagwel.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jianghu66.top/gtyhdbdzug.html

[T03] Kotlin：字符串模板
来源：http://hz.chenlongwang.top/gtffizfplv.html

"值: $b"
来源：http://hz.iojbl.cn/gtvyzcfvjt.html

[T04] Kotlin：空安全
来源：http://hz.gzhubu.top/gtpbyxszzm.html

val n: String? = null;  n?.length
来源：http://hz.dianchejie.cn/gtpkrzbzbi.html

[T05] Kotlin：when 表达式
来源：http://hz.tianlin.xyz/gtyecthvmp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.aibaodan.cn/gtdbsteuck.html

[T06] Kotlin：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtduqijtad.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangshuangyany.cn/gtubtdxzaq.html

[T07] Kotlin：集合过滤
来源：http://hz.andypj.xyz/gtxfmphqbf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinyuanbaomall.cn/gtzjoavloy.html

[T08] Kotlin：数据类
来源：http://hz.cheryme.top/gtjbxnfjqv.html

data class User(val name: String, val age: Int)
来源：http://hz.sxryk.cn/gtwcldudge.html

[T09] Kotlin：扩展函数
来源：http://hz.9152youxi.cn/gtsltqupam.html

fun String.exclaim() = this + "!"
来源：http://hz.zhengqikj.top/gttyutwaau.html

[T10] Kotlin：默认参数
来源：http://hz.gotoacloud.top/gtsclwvham.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hysaishi.cn/gtpywliben.html

[T11] Kotlin：协程
来源：http://hz.jinqigfzy.top/gtszggoimh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnxiangtu.top/gtzrzeedcz.html

[T12] Kotlin：解构声明
来源：http://hz.pycfn.com/gttlbgrydn.html

val (a, b) = Pair(1, 2)
来源：http://hz.0kj1m.cn/gtgoyhnwzp.html

[T13] Kotlin：只读 Map
来源：http://hz.jyoumei.cn/gtignttkde.html

val m = mapOf("a" to 1)
来源：http://hz.yanxiufei.cn/gtpajynqtx.html

[T14] Kotlin：循环
来源：http://hz.xingfuxueyuan.xyz/gttphpgnix.html

for (i in 1..10) println(i)
来源：http://hz.zhoulong.xyz/gtgskjymfe.html

[T15] Kotlin：接口
来源：http://hz.ydjk.org.cn/gtnherxskc.html

interface Shape { fun area(): Double }
来源：http://hz.mhx1999.top/gtzkycvdfj.html

[T16] Swift：Hello World
来源：http://hz.jinqigfzy.top/gtszilfysi.html

print("Hello")
来源：http://hz.meibo888.top/gtqitemldj.html

[T17] Swift：变量与常量
来源：http://hz.52xcode.cn/gtgdbpqopw.html

var a = 1;  let b = 2
来源：http://hz.tian-w.cn/gtqdlpcaas.html

[T18] Swift：字符串插值
来源：http://hz.haohaochexian.top/gtxunzzqeb.html

"值: \(b)"
来源：http://hz.dianchejie.cn/gtqhkloluo.html

[T19] Swift：可选绑定
来源：http://hz.jinyuanbaomall.cn/gtbwhoskbw.html

if let n = opt { print(n) }
来源：http://hz.gotoacloud.top/gtkoidrome.html

[T20] Swift：数组操作
来源：http://hz.bjfxy.top/gtigkaegbj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aizwys.cn/gtbnuqvlht.html

[T21] Swift：遍历
来源：http://hz.smart0.xyz/gtdrlxqubj.html

for x in a { print(x) }
来源：http://hz.zdqjudy.top/gtqgmvrnze.html

[T22] Swift：字典
来源：http://hz.ppjwa.cn/gtjqiezslh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydzc1.top/gtqzyiepcn.html

[T23] Swift：函数
来源：http://hz.yvedp.cn/gtqyllvsdu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.fengsongda.top/gtnbospnbq.html

[T24] Swift：闭包
来源：http://hz.shanyushiyangtech.top/gtjxnxaapu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinyuanbaomall.cn/gtrirhqhkm.html

[T25] Swift：结构体
来源：http://hz.hammf.cn/gtztcvurqi.html

struct P { var x: Int }
来源：http://hz.daxiang520.top/gtrmtkkqok.html

[T26] Swift：类与重写
来源：http://hz.yongpay.top/gtkdbfskaw.html

class A: Base { override func f() {} }
来源：http://hz.0kj1m.cn/gtwfmkwurv.html

[T27] Swift：错误处理
来源：http://hz.nanxinkj.top/gtixaaqfwr.html

do { try f() } catch { print(error) }
来源：http://hz.andypj.xyz/gtavziiyel.html

[T28] Swift：枚举
来源：http://hz.xinyue.icu/gtjmejllmo.html

enum Color { case red, green }
来源：http://hz.tianlin.xyz/gtfgodujod.html

[T29] Swift：guard 提前返回
来源：http://hz.hongshengwenyu.top/gtzubswfme.html

guard let x = opt else { return }
来源：http://hz.ydzc1.top/gtizosaxdu.html

[T30] Swift：协议
来源：http://hz.cheryme.top/gtnwqjkauh.html

protocol Shape { func area() -> Double }
来源：http://hz.shanyushiyangtech.top/gtmrrlqwzc.html

[T31] Lua：Hello World
来源：http://hz.yvedp.cn/gtyqgqjitk.html

print("Hello")
来源：http://hz.ppjwa.cn/gtprerlsol.html

[T32] Lua：局部变量
来源：http://hz.hywenlv.cn/gtnizdtbqu.html

local a = 1
来源：http://hz.yangfankeji.com/gtlrdlpppb.html

[T33] Lua：表（数组）
来源：http://hz.xuetiantiany.cn/gtghmupznr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ydzc1.top/gtqvhpvkjp.html

[T34] Lua：遍历表
来源：http://hz.pycfn.com/gtswlnmwzj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.316326.xyz/gtrwavwwpl.html

[T35] Lua：字典表
来源：http://hz.aibaodan.cn/gteddlkpqi.html

local d = { a = 1 };  d.b = 2
来源：http://hz.cdnleiting.top/gtkedcwwhn.html

[T36] Lua：函数
来源：http://hz.jinghuilouyu.cn/gtdqfpsohh.html

function add(a, b) return a + b end
来源：http://hz.ybcxt.top/gtcdybdvgh.html

[T37] Lua：字符串拼接
来源：http://hz.dashuyun.cn/gtfrgnqkbq.html

"a" .. "b"
来源：http://hz.fzhhl.top/gtnzvepvnx.html

[T38] Lua：条件
来源：http://hz.0kj1m.cn/gtsyyjiern.html

if x > 0 then print("正") end
来源：http://hz.chenjidiqi.icu/gtikgejziu.html

[T39] Lua：模式匹配
来源：http://hz.chenjidiqi.icu/gtscqlfauz.html

string.find(s, "%d+")
来源：http://hz.shuidangran.top/gtbnfjuafc.html

[T40] Lua：元表
来源：http://hz.aizwys.cn/gtrmwzpgwl.html

setmetatable({}, { __index = base })
来源：http://hz.jinqigufen.top/gtzovkbvvv.html

[T41] Perl：Hello World
来源：http://hz.hfpthk.cn/gtsvvtfxhy.html

print "Hello\n";
来源：http://hz.jinghuilouyu.cn/gtzjqxvxhx.html

[T42] Perl：变量类型
来源：http://hz.hongshengwenyu.top/gtgpgjclql.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xingfuxueyuan.xyz/gtstbvogdb.html

[T43] Perl：字符串插值
来源：http://hz.ybcxt.top/gtzmntrarp.html

"值: $a"
来源：http://hz.gzhubu.top/gtmvjsrszl.html

[T44] Perl：条件
来源：http://hz.haohaochexian.top/gttihpmoyb.html

if ($a > 0) { print "正"; }
来源：http://hz.jqgfzy.top/gtghfwkutb.html

[T45] Perl：数组遍历
来源：http://hz.yj20258.top/gtldburnel.html

for my $x (@arr) { print $x; }
来源：http://hz.52xcode.cn/gtnemiaquu.html

[T46] Perl：哈希操作
来源：http://hz.cashguo.top/gtcwkpsefk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shzxlz.cn/gtjagyxeua.html

[T47] Perl：正则捕获
来源：http://hz.jinghuilouyu.cn/gtonzebsgm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.pycfn.com/gtpednocgi.html

[T48] Perl：正则替换
来源：http://hz.yueranfly.top/gtpstcjwaf.html

$s =~ s/old/new/g;
来源：http://hz.xuanzx.com/gtuvhestaj.html

[T49] Perl：函数
来源：http://hz.zhijiandao.cn/gtratghxge.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.sxryk.cn/gtrkrynotx.html

[T50] Perl：逐行读文件
来源：http://hz.gotoacloud.top/gtsrcaggdn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.pycfn.com/gtpnnjkuag.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xinyue.icu/gtsxwmlffl.html

[T51] Scala：Hello World
来源：http://hz.jinghuilouyu.cn/gtlviggoje.html

println("Hello")
来源：http://hz.nwbrower.top/gtcirkssmn.html

[T52] Scala：变量
来源：http://hz.iojbl.cn/gtpomvzdcc.html

val a = 1;  var b = 2
来源：http://hz.nanxuanxn.top/gtnclolhdz.html

[T53] Scala：字符串插值
来源：http://hz.feifeiyinyue.top/gtysohdlrj.html

s"值: $b"
来源：http://hz.ydzc1.top/gtgwayvyqc.html

[T54] Scala：集合映射
来源：http://hz.pengpengdd.cyou/gtrloabaud.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhengqikj.top/gtyxzntlwf.html

[T55] Scala：集合过滤
来源：http://hz.zhoulong.xyz/gtoymbjndn.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ybcxt.top/gtfvzokjqq.html

[T56] Scala：样例类
来源：http://hz.wangdashe.top/gtuuttnhzk.html

case class User(name: String, age: Int)
来源：http://hz.sweek.top/gtjpvcmuuj.html

[T57] Scala：模式匹配
来源：http://hz.jinqigufen.top/gtpuuzamfp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ydjk.org.cn/gtyqpwymgc.html

[T58] Scala：函数定义
来源：http://hz.daxiang520.top/gtniwirhyz.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.guannengcc.top/gtdjkjrxtb.html

[T59] Scala：循环
来源：http://hz.chenzaomai.com/gteurepuow.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnxiangtu.top/gtnjluxywn.html

[T60] Scala：折叠
来源：http://hz.tanke756.top/gtjsexdvie.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ydzc1.top/gtdtuopgsy.html

================================================================================
来源：http://hz.jinqigufen.top/gtpqppjmvy.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.birdmap.top/gtxywpdevw.html

================================================================================
来源：http://hz.fengsongda.top/gtngevqtcv.html

[U01] Py：创建虚拟环境
来源：http://hz.smart0.xyz/gtnvfguqjg.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.daria6918.cn/gtkzbqutxz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.iojbl.cn/gtbdifdvwa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.bjfxy.top/gtivjznfvg.html

[U03] Py：加载 .env 配置
来源：http://hz.yuxming.cn/gtqgaobcox.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.52xcode.cn/gtyzpmzobr.html

[U04] Py：变量调试打印
来源：http://hz.jyoumei.cn/gtcgfqevwv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.52xcode.cn/gtngdyqlms.html

[U05] Py：列表去重且保序
来源：http://hz.shanyushiyangkeji.top/gtnaecjkhn.html

list(dict.fromkeys(arr))
来源：http://hz.chenjidiqi.icu/gtcwbucmni.html

[U06] Py：合并两个字典
来源：http://hz.jinyuanbaomall.cn/gttvhrdsbo.html

{**a, **b}
来源：http://hz.aibaodan.cn/gtwbfdudqs.html

[U07] Py：反转字典键值
来源：http://hz.kuanghao11.cn/gtsaomugyy.html

{v: k for k, v in d.items()}
来源：http://hz.cheryme.top/gtlztibvmn.html

[U08] Py：展平二维列表
来源：http://hz.c1oappe.top/gtjqdmiucm.html

[y for x in nested for y in x]
来源：http://hz.aizwys.cn/gtzvudfzyy.html

[U09] Py：字典取最大值的键
来源：http://hz.nanxinkj.top/gtjfzgjtud.html

max(d, key=d.get)
来源：http://hz.jlsjyb.cn/gthzroowxc.html

[U10] Py：按值排序字典
来源：http://hz.yj20258.top/gtfoobaeok.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.c1oappe.top/gtipavuwls.html

[U11] Py：生成器表达式
来源：http://hz.yj20258.top/gtmhxwszqp.html

(x * 2 for x in arr)
来源：http://hz.jqgufenzy.top/gturgacsjm.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yueranfly.top/gtcnofuvxf.html

Counter(arr).most_common(3)
来源：http://hz.jinqigufen.top/gtwohrmxxj.html

[U13] Py：固定长度队列
来源：http://hz.gotoacloud.top/gthgunfbop.html

deque(maxlen=10)
来源：http://hz.xylfe.cn/gtqajxbxyr.html

[U14] Py：分组收集到列表
来源：http://hz.hysaishi.cn/gtbdtfryrl.html

defaultdict(list)
来源：http://hz.hongshengwenyu.top/gtpklcmhmj.html

[U15] Py：高精度计时
来源：http://hz.jianghu66.top/gtishbmybd.html

t = time.perf_counter()
来源：http://hz.ydzc1.top/gtxkiqcukh.html

[U16] Py：命令行参数解析
来源：http://hz.jlsjyb.cn/gtglpbqigw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.cqqwz.cn/gtpnukjvjo.html

[U17] Py：初始化日志
来源：http://hz.jinqigufen.top/gtmrscyydz.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.feifeiyinyue.top/gtzlzcadxy.html

[U18] Py：预编译正则
来源：http://hz.hysaishi.cn/gtsrvtgofk.html

pat = re.compile(r"\d+")
来源：http://hz.52xcode.cn/gtblbrfryb.html

[U19] Py：正则替换带回调
来源：http://hz.xziqi.cn/gtudksfdvr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.nwbrower.top/gtwkzmnkpt.html

[U20] Py：缓存函数结果
来源：http://hz.zhijiandao.cn/gtniebngef.html

@functools.lru_cache(maxsize=None)
来源：http://hz.andypj.xyz/gtgfeebkmy.html

[U21] Py：自定义上下文管理器
来源：http://hz.aibaodan.cn/gtwdfuzeyp.html

@contextlib.contextmanager
来源：http://hz.c1oappe.top/gtncyyjvpt.html

[U22] Py：矩阵转置
来源：http://hz.snrcjt.cn/gtfdnccpsd.html

list(zip(*m))
来源：http://hz.chenzaomai.com/gtlpzzkqis.html

[U23] Py：分块读取大文件
来源：http://hz.jiagoushi.top/gtxdikmkty.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.pengpengdd.cyou/gtvmgnxsgm.html

[U24] Py：路径操作
来源：http://hz.shzxlz.cn/gtzdugavfa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj202588.top/gtboutpgqo.html

[U25] Py：CSV 按字典读
来源：http://hz.fzhhl.top/gtqljuseto.html

csv.DictReader(f)
来源：http://hz.fzhhl.top/gtnnpikmgd.html

[U26] Py：并发下载
来源：http://hz.316326.xyz/gtphujjmcp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ppjwa.cn/gtynualdaj.html

[U27] Py：异步 HTTP
来源：http://hz.shangyingyoupin.top/gtyonssnyo.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.svipenyu.cn/gtdpmzjtum.html

[U28] Py：类型别名
来源：http://hz.guannengcc.top/gtaklpjdud.html

UserId = int
来源：http://hz.hammf.cn/gtqtywvkmd.html

[U29] Py：属性校验
来源：http://hz.yuanzhike.top/gtugtfpfkm.html

@property 与 @x.setter 配合
来源：http://hz.fzhhl.top/gtytneccul.html

[U30] Py：数据类
来源：http://hz.jianghu66.top/gtaaolshtl.html

@dataclass(slots=True)
来源：http://hz.pengpengdd.cyou/gtwpmjosbx.html

[U31] Py：单测
来源：http://hz.aibaodan.cn/gtxvycauqi.html

python -m pytest -q
来源：http://hz.hongshengwenyu.top/gtjozfbdap.html

[U32] Py：代码格式化
来源：http://hz.zhaomingkeji.xyz/gtxfdoofri.html

ruff format . && ruff check --fix .
来源：http://hz.xuanzx.com/gtqlmmjmwy.html

[U33] Py：打包发布
来源：http://hz.jinghuilouyu.cn/gtbxftrccg.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.tanke756.top/gtvmgvuiem.html

[U34] Py：判断编码
来源：http://hz.zhengqikj.top/gthdgeumrw.html

chardet.detect(raw)
来源：http://hz.iojbl.cn/gtxvnayisn.html

[U35] Py：发送邮件
来源：http://hz.ydzc1.top/gtgzenbine.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jlsjyb.cn/gteemskhvi.html

[U36] Py：定时任务
来源：http://hz.pycfn.com/gtetcntiyi.html

schedule.every(10).minutes.do(job)
来源：http://hz.yvedp.cn/gtdlfiuehg.html

[U37] Py：读写 Excel
来源：http://hz.xylfe.cn/gtgmtllxsf.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.feifeiyinyue.top/gtvojiuluq.html

[U38] Py：获取脚本所在目录
来源：http://hz.pengpengdd.cyou/gtvedxjjys.html

Path(__file__).resolve().parent
来源：http://hz.hywenlv.cn/gtikmzevjn.html

[U39] Py：判断是否在交互环境
来源：http://hz.xuanzx.com/gtjlyhqjkr.html

sys.stdout.isatty()
来源：http://hz.jinqigfzy.top/gtaaukwahd.html

[U40] Py：打印到标准错误
来源：http://hz.jinyuanbaomall.cn/gtymtetmku.html

print("err", file=sys.stderr)
来源：http://hz.redwolf501.top/gtnfpmxnjb.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.zhoulong.xyz/gtdzemxyii.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.zhaomingkeji.xyz/gtoqnotubh.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.svipenyu.cn/gtnuabcrms.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.smart0.xyz/gtmczoasru.html

[U43] PHP：声明命名空间
来源：http://hz.hywenlv.cn/gtbyinhody.html

namespace App\Http;
来源：http://hz.yuxming.cn/gtbnpuhvuz.html

[U44] PHP：开启严格类型
来源：http://hz.zhiwuduotai.top/gtpaegqufx.html

declare(strict_types=1);
来源：http://hz.jinqigufen.top/gtcnzkoyyt.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jlsjyb.cn/gtecspsosg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.c1oappe.top/gtrrdmungz.html

[U46] PHP：可空类型
来源：http://hz.ydzc1.top/gtmtcbuajg.html

?string $name = null
来源：http://hz.yongpay.top/gthucmiuuc.html

[U47] PHP：联合类型
来源：http://hz.52xcode.cn/gtgaezaldi.html

int|string $id
来源：http://hz.ydzc1.top/gtjzgjfegp.html

[U48] PHP：纯枚举
来源：http://hz.chenzaomai.com/gteeqrntoj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.mhx1999.top/gtyoudczuh.html

[U49] PHP：只读属性
来源：http://hz.cdnleiting.top/gtqcptykfu.html

public readonly string $name
来源：http://hz.quarkkingdee.top/gtnunawzrx.html

[U50] PHP：构造器属性提升
来源：http://hz.hammf.cn/gtogeefjjc.html

public function __construct(private int $id) {}
来源：http://hz.9152youxi.cn/gtfvfofjtf.html

[U51] PHP：数组解构
来源：http://hz.ppjwa.cn/gtiwaxxoeo.html

[$a, $b] = $arr;
来源：http://hz.yongpay.top/gttvvfqezm.html

[U52] PHP：箭头函数
来源：http://hz.ppjwa.cn/gtxesqrqea.html

$double = fn($x) => $x * 2;
来源：http://hz.daxiang520.top/gtbtuzdvpf.html

[U53] PHP：空合并运算符
来源：http://hz.zhongyouzk.top/gtufxjxofz.html

$v = $a ?? $b ?? "default";
来源：http://hz.hnxiangtu.top/gtwgtzeakx.html

[U54] PHP：空安全调用
来源：http://hz.dianchejie.cn/gtlmapsgzy.html

$obj?->method()
来源：http://hz.jinghuilouyu.cn/gtocuxtgtu.html

[U55] PHP：match 表达式
来源：http://hz.chenjidiqi.icu/gtcudmdics.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.sysykeji.top/gtelvxpppb.html

[U56] PHP：命名参数
来源：http://hz.snrcjt.cn/gtsbhaowos.html

f(a: 1, b: 2)
来源：http://hz.hammf.cn/gtokzoizac.html

[U57] PHP：字符串插值
来源：http://hz.52xcode.cn/gtaptrkarm.html

"值: {$a}"
来源：http://hz.zhiwuduotai.top/gtfvplbpeu.html

[U58] PHP：数组三件套
来源：http://hz.kuanghao11.cn/gteoudcdie.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.andypj.xyz/gtoyuqkgdn.html

[U59] PHP：自定义排序
来源：http://hz.cashguo.top/gtsftptxpw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ppjwa.cn/gttqlngzdq.html

[U60] PHP：JSON 编解码
来源：http://hz.yangfankeji.com/gtzofnaiks.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shzxlz.cn/gttxhussut.html

[U61] PHP：正则
来源：http://hz.zhongyouzk.top/gtbajjofmt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zdqjudy.top/gtmzjwbihu.html

[U62] PHP：日期对象
来源：http://hz.zhongyouzk.top/gtjgriljwk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.9152youxi.cn/gtfmirebtf.html

[U63] PHP：文件读写
来源：http://hz.nwbrower.top/gtuoafpuhf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.haohaochexian.top/gtlstgdahy.html

[U64] PHP：目录遍历
来源：http://hz.dashuyun.cn/gtxzefpxsf.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.cqqwz.cn/gtzbmhgjbe.html


<!-- 参考信息 -->