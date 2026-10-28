代发 wailian999

[S33] C++：vector 增删
来源：http://hz.jinyuanbaomall.cn/gtjiidhmla.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj20258.top/gtytxfbwnn.html

[S34] C++：遍历 vector
来源：http://hz.jiagoushi.top/gtosjjaeoz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj20258888.top/gthpsdaavc.html

[S35] C++：map
来源：http://hz.feifeiyinyue.top/gtxsviccsi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.feifeiyinyue.top/gtlfubasdl.html

[S36] C++：unordered_map
来源：http://hz.vqdsnc.cn/gtpjxuehap.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtvsomwdls.html

[S37] C++：set
来源：http://hz.yongpay.top/gtbmbwvgfn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yuanzhike.top/gtxchprsay.html

[S38] C++：排序
来源：http://hz.nanxinkj.top/gtxkwgddee.html

std::sort(v.begin(), v.end());
来源：http://hz.hongshengwenyu.top/gttmfksiya.html

[S39] C++：自定义比较器排序
来源：http://hz.jinghuilouyu.cn/gthsjlpcrn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.havefunace.top/gtggchoibx.html

[S40] C++：查找元素
来源：http://hz.wangshuangyany.cn/gtlosoxhur.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.andypj.xyz/gtjdtxslts.html

[S41] C++：类与构造函数
来源：http://hz.sweek.top/gtwgdjuovt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yonumen.top/gtsozlwnow.html

[S42] C++：继承与虚函数
来源：http://hz.haohaochexian.top/gtwijgkgzx.html

class B : public Base { public: void f() override {} };
来源：http://hz.hnqzz.top/gtijgkwusf.html

[S43] C++：智能指针
来源：http://hz.yj20258.top/gtfourjyrd.html

auto p = std::make_unique<int>(5);
来源：http://hz.nwbrower.top/gtggnzmzfl.html

[S44] C++：引用传参
来源：http://hz.yvedp.cn/gtafmbsvse.html

void inc(int &x) { ++x; }
来源：http://hz.jinqigfzy.top/gttlgcpzdu.html

[S45] C++：lambda
来源：http://hz.yongpay.top/gtkystljpt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.0kj1m.cn/gtyiqtviej.html

[S46] C++：函数模板
来源：http://hz.zhixingplan.top/gtwiimpjir.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.feifeiyinyue.top/gtcnsaspsv.html

[S47] C++：结构化绑定遍历
来源：http://hz.wangdashe.top/gtxqpxydkr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.redwolf501.top/gtmwzjlfow.html

[S48] C++：逐行读文件
来源：http://hz.zhijiandao.cn/gtfxinkilm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zycfv.cn/gthzmoepgg.html

while (std::getline(in, line)) { }
来源：http://hz.wangdashe.top/gtmebroowp.html

[S49] C++：写文件
来源：http://hz.ybcxt.top/gtbfmifwmq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenlongwang.top/gtmemykqeb.html

[S50] C++：格式化数字
来源：http://hz.316326.xyz/gtkzwtrkkc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sxryk.cn/gtpcefzcpu.html

[S51] C++：显式类型转换
来源：http://hz.xziqi.cn/gtxtkidlio.html

static_cast<double>(a) / b
来源：http://hz.xylfe.cn/gtxxujgwyn.html

[S52] C++：const 与 noexcept
来源：http://hz.jinqigufen.top/gtclcjojjz.html

int size() const noexcept { return n_; }
来源：http://hz.jinghuilouyu.cn/gttznmsbjb.html

[S53] C++：移动语义
来源：http://hz.aibaodan.cn/gtayovfhfu.html

std::vector<int> w = std::move(v);
来源：http://hz.havefunace.top/gtaachnron.html

[S54] C++：异常处理
来源：http://hz.zhijiandao.cn/gtwdlxxtgw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hammf.cn/gtaabkemfd.html

[S55] C++：结构化绑定
来源：http://hz.jianghu66.top/gtnoqulgtc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.shanyushiyangtech.top/gtwvpriibv.html

[S56] C++：optional
来源：http://hz.9152youxi.cn/gttfcseuvw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gaohongyu789.top/gtsrwchpgz.html

[S57] C++：编译期常量
来源：http://hz.tian-w.cn/gtwljuuglm.html

constexpr int N = 10;
来源：http://hz.yanxiufei.cn/gthyairujz.html

[S58] C++：命名空间
来源：http://hz.yongpay.top/gtcoxuqksm.html

namespace ns { int f() { return 1; } }
来源：http://hz.cdnleiting.top/gtvletcoaa.html

[S59] C++：静态断言
来源：http://hz.hnqzz.top/gtkcjbjmpi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.meibo888.top/gtselakfdx.html

[S60] C++：遍历并删除元素
来源：http://hz.guannengcc.top/gtovobgrce.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangkeji.top/gtbbihazkk.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtsrgjjxct.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sxryk.cn/gtwaqicqii.html

================================================================================
来源：http://hz.pycfn.com/gtmtukxqgy.html

[T01] Kotlin：Hello World
来源：http://hz.jyoumei.cn/gtxcfwbxzf.html

println("Hello")
来源：http://hz.sweek.top/gtajbswbey.html

[T02] Kotlin：变量
来源：http://hz.yuxming.cn/gtjiehibdn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xziqi.cn/gtumxkxpgx.html

[T03] Kotlin：字符串模板
来源：http://hz.ydzc1.top/gtnwincvfa.html

"值: $b"
来源：http://hz.zhoulong.xyz/gtsebksyhx.html

[T04] Kotlin：空安全
来源：http://hz.zhiwuduotai.top/gtimmbospk.html

val n: String? = null;  n?.length
来源：http://hz.zdqjudy.top/gtorgcqdea.html

[T05] Kotlin：when 表达式
来源：http://hz.sweek.top/gtvjylpjfe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.dianchejie.cn/gtgsrqiouc.html

[T06] Kotlin：集合映射
来源：http://hz.zhoulong.xyz/gtsrxbwcfg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hfpthk.cn/gtygbnsliq.html

[T07] Kotlin：集合过滤
来源：http://hz.xuanzx.com/gtsfdjgire.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhoulong.xyz/gtgzzanlbc.html

[T08] Kotlin：数据类
来源：http://hz.wangshuangyany.cn/gtotlsenep.html

data class User(val name: String, val age: Int)
来源：http://hz.hfpthk.cn/gtmrrbsiad.html

[T09] Kotlin：扩展函数
来源：http://hz.zhongyouzk.top/gtilejmsxy.html

fun String.exclaim() = this + "!"
来源：http://hz.hywenlv.cn/gtlxebmtro.html

[T10] Kotlin：默认参数
来源：http://hz.316326.xyz/gtisqnkgzb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cucudq.cn/gtzyegcchm.html

[T11] Kotlin：协程
来源：http://hz.gzhubu.top/gtetmefjnd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.feifeiyinyue.top/gtjquunoja.html

[T12] Kotlin：解构声明
来源：http://hz.dianchejie.cn/gttlxsblql.html

val (a, b) = Pair(1, 2)
来源：http://hz.cdnleiting.top/gtonocfoxe.html

[T13] Kotlin：只读 Map
来源：http://hz.guannengcc.top/gtusjjoatz.html

val m = mapOf("a" to 1)
来源：http://hz.yvedp.cn/gtcjnshrkd.html

[T14] Kotlin：循环
来源：http://hz.shanyushiyangkeji.top/gttwfgniyr.html

for (i in 1..10) println(i)
来源：http://hz.xylfe.cn/gtvidhyfan.html

[T15] Kotlin：接口
来源：http://hz.mhx1999.top/gtkikhfkgi.html

interface Shape { fun area(): Double }
来源：http://hz.xziqi.cn/gtwoklglen.html

[T16] Swift：Hello World
来源：http://hz.cdnleiting.top/gthycpedgd.html

print("Hello")
来源：http://hz.jyoumei.cn/gtqlcmmwxj.html

[T17] Swift：变量与常量
来源：http://hz.yanxiufei.cn/gtdgosznwa.html

var a = 1;  let b = 2
来源：http://hz.chenzaomai.com/gtohuvilsq.html

[T18] Swift：字符串插值
来源：http://hz.iojbl.cn/gtggwwlshi.html

"值: \(b)"
来源：http://hz.yuanzhike.top/gtrilabpqk.html

[T19] Swift：可选绑定
来源：http://hz.zhoulong.xyz/gtbvsttiyy.html

if let n = opt { print(n) }
来源：http://hz.jinghuilouyu.cn/gtkjwakcjy.html

[T20] Swift：数组操作
来源：http://hz.daxiang520.top/gtnbwybpbm.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gogol.net.cn/gtjiepaage.html

[T21] Swift：遍历
来源：http://hz.smart0.xyz/gtbsigbzsf.html

for x in a { print(x) }
来源：http://hz.cashguo.top/gtwnvqsrlm.html

[T22] Swift：字典
来源：http://hz.jiagoushi.top/gtpgbrmlgg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jianghu66.top/gtdhwomlcr.html

[T23] Swift：函数
来源：http://hz.ydzc1.top/gtessgzemi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ywan-chungtsiang.top/gtfvgcqloz.html

[T24] Swift：闭包
来源：http://hz.mhx1999.top/gtahkoukiy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hnxiangtu.top/gtglqsxkqf.html

[T25] Swift：结构体
来源：http://hz.zhixingplan.top/gtldtwtxqq.html

struct P { var x: Int }
来源：http://hz.jiagoushi.top/gtcgecssbl.html

[T26] Swift：类与重写
来源：http://hz.zhiwuduotai.top/gtwtglxsqy.html

class A: Base { override func f() {} }
来源：http://hz.smart0.xyz/gthcosxbpr.html

[T27] Swift：错误处理
来源：http://hz.snrcjt.cn/gtsziyvqxe.html

do { try f() } catch { print(error) }
来源：http://hz.wangshuangyany.cn/gtkdkhsvaj.html

[T28] Swift：枚举
来源：http://hz.jyoumei.cn/gtfqquhtmb.html

enum Color { case red, green }
来源：http://hz.gotoacloud.top/gtpcqkooya.html

[T29] Swift：guard 提前返回
来源：http://hz.zhaomingkeji.xyz/gtabtkhdju.html

guard let x = opt else { return }
来源：http://hz.ivvv.top/gtdydkyvqi.html

[T30] Swift：协议
来源：http://hz.nanxuanxn.top/gtaomyurmk.html

protocol Shape { func area() -> Double }
来源：http://hz.jianghu66.top/gtznzldbxh.html

[T31] Lua：Hello World
来源：http://hz.jqgufenzy.top/gthamlvfnt.html

print("Hello")
来源：http://hz.yangfankeji.com/gtinjwoome.html

[T32] Lua：局部变量
来源：http://hz.yongpay.top/gtqzxkylef.html

local a = 1
来源：http://hz.jinghuilouyu.cn/gtpldbgmbt.html

[T33] Lua：表（数组）
来源：http://hz.fzhhl.top/gthesbvxvs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jinyuanbaomall.cn/gtjcnxzggk.html

[T34] Lua：遍历表
来源：http://hz.guowangkeji.top/gtwaikdfit.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yuanzhike.top/gtgsjcfzqs.html

[T35] Lua：字典表
来源：http://hz.meibo888.top/gtvwrimiji.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yj202588.top/gtvhqiuazb.html

[T36] Lua：函数
来源：http://hz.sxryk.cn/gtiddnppuc.html

function add(a, b) return a + b end
来源：http://hz.kuanghao11.cn/gtbvwfsplg.html

[T37] Lua：字符串拼接
来源：http://hz.52xcode.cn/gtsblprdyn.html

"a" .. "b"
来源：http://hz.jianghu66.top/gtgsdankmp.html

[T38] Lua：条件
来源：http://hz.xinyue.icu/gtxzynezaa.html

if x > 0 then print("正") end
来源：http://hz.0kj1m.cn/gtobiqypts.html

[T39] Lua：模式匹配
来源：http://hz.cucudq.cn/gtvegjdixc.html

string.find(s, "%d+")
来源：http://hz.mhx1999.top/gtiasgwmvd.html

[T40] Lua：元表
来源：http://hz.yj20258.top/gtizhhsqlx.html

setmetatable({}, { __index = base })
来源：http://hz.zhaomingkeji.xyz/gtiofakqik.html

[T41] Perl：Hello World
来源：http://hz.chenzaomai.com/gtftwwsbki.html

print "Hello\n";
来源：http://hz.zhixingplan.top/gtgtlsrwzp.html

[T42] Perl：变量类型
来源：http://hz.chenlongwang.top/gtfnaxzhbu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gzhubu.top/gtqidtcrhb.html

[T43] Perl：字符串插值
来源：http://hz.sweek.top/gteubvoaay.html

"值: $a"
来源：http://hz.tianlin.xyz/gtdiiethyz.html

[T44] Perl：条件
来源：http://hz.gogol.net.cn/gtbjaqmgmt.html

if ($a > 0) { print "正"; }
来源：http://hz.jianghu66.top/gtljryrzpz.html

[T45] Perl：数组遍历
来源：http://hz.sxryk.cn/gtcpolpqrj.html

for my $x (@arr) { print $x; }
来源：http://hz.yj202588.top/gtqusucanw.html

[T46] Perl：哈希操作
来源：http://hz.nanxuanxn.top/gtebkeyzca.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.cdnleiting.top/gthzvxprvf.html

[T47] Perl：正则捕获
来源：http://hz.vqdsnc.cn/gtrhpvomiv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.birdmap.top/gtmckdvtoz.html

[T48] Perl：正则替换
来源：http://hz.pycfn.com/gtlmeohdhj.html

$s =~ s/old/new/g;
来源：http://hz.hywenlv.cn/gtylxrpwyd.html

[T49] Perl：函数
来源：http://hz.zhijiandao.cn/gtmybtyjde.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xingfuxueyuan.xyz/gteidbcwwc.html

[T50] Perl：逐行读文件
来源：http://hz.nanxuanxn.top/gtmcqqdeif.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.cucudq.cn/gttshtudtl.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jlsjyb.cn/gttlkbofxw.html

[T51] Scala：Hello World
来源：http://hz.zhaomingkeji.xyz/gtemckmrrc.html

println("Hello")
来源：http://hz.snrcjt.cn/gtpifwvjnt.html

[T52] Scala：变量
来源：http://hz.guannengcc.top/gtbadzsqcy.html

val a = 1;  var b = 2
来源：http://hz.zhoulong.xyz/gtoyvcxmbz.html

[T53] Scala：字符串插值
来源：http://hz.nanxinkj.top/gtdrxegaah.html

s"值: $b"
来源：http://hz.zhijiandao.cn/gtfubndlii.html

[T54] Scala：集合映射
来源：http://hz.yvedp.cn/gtkqsetsns.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.feifeiyinyue.top/gtadqtcvxi.html

[T55] Scala：集合过滤
来源：http://hz.andypj.xyz/gtyvtzdixg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.mhx1999.top/gtvckggvjf.html

[T56] Scala：样例类
来源：http://hz.iojbl.cn/gtivbdpcya.html

case class User(name: String, age: Int)
来源：http://hz.shangyingyoupin.top/gtjczvntdd.html

[T57] Scala：模式匹配
来源：http://hz.yj202588.top/gtiaxhzeah.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cdnleiting.top/gtcwpnvcau.html

[T58] Scala：函数定义
来源：http://hz.yueranfly.top/gtfflqhjvl.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.meibo888.top/gtkwfpgnkj.html

[T59] Scala：循环
来源：http://hz.jinghuilouyu.cn/gtklsrsidk.html

for (i <- 1 to 10) println(i)
来源：http://hz.fzhhl.top/gtlkexvezp.html

[T60] Scala：折叠
来源：http://hz.shangyingyoupin.top/gtzcsdcegr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.daxiang520.top/gtsuqstoms.html

================================================================================
来源：http://hz.jqgfzy.top/gtqzzuuxdg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj20258888.top/gtobebhkwf.html

================================================================================
来源：http://hz.ppjwa.cn/gtouxtqbsj.html

[U01] Py：创建虚拟环境
来源：http://hz.daxiang520.top/gtvcghenay.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.xuetiantiany.cn/gthisqqvjs.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ppjwa.cn/gtecjauouw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.ybcxt.top/gtzxgbfgnk.html

[U03] Py：加载 .env 配置
来源：http://hz.yj20258888.top/gtftsorjhg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.cucudq.cn/gtgcqrrejw.html

[U04] Py：变量调试打印
来源：http://hz.guowangkeji.top/gtbgclzflj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.birdmap.top/gttqlpfowq.html

[U05] Py：列表去重且保序
来源：http://hz.aibaodan.cn/gtdxqvpofy.html

list(dict.fromkeys(arr))
来源：http://hz.pycfn.com/gtuipgbtyl.html

[U06] Py：合并两个字典
来源：http://hz.pycfn.com/gtzerfmxcf.html

{**a, **b}
来源：http://hz.fzhhl.top/gtvwyxkdwt.html

[U07] Py：反转字典键值
来源：http://hz.jqgufenzy.top/gtkokfnocp.html

{v: k for k, v in d.items()}
来源：http://hz.52xcode.cn/gteglornru.html

[U08] Py：展平二维列表
来源：http://hz.quarkkingdee.top/gtozdhpocb.html

[y for x in nested for y in x]
来源：http://hz.hysaishi.cn/gtlficigwr.html

[U09] Py：字典取最大值的键
来源：http://hz.zhijiandao.cn/gtxsmpdevv.html

max(d, key=d.get)
来源：http://hz.yanxiufei.cn/gtdasrwpcw.html

[U10] Py：按值排序字典
来源：http://hz.shanyushiyangkeji.top/gtshmuehjg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.ydjk.org.cn/gthfxpnrid.html

[U11] Py：生成器表达式
来源：http://hz.wangdashe.top/gtqtlklwig.html

(x * 2 for x in arr)
来源：http://hz.jyoumei.cn/gtjtvyiafa.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.gotoacloud.top/gtttuvzixn.html

Counter(arr).most_common(3)
来源：http://hz.aibaodan.cn/gtaiisepui.html

[U13] Py：固定长度队列
来源：http://hz.svipenyu.cn/gtixxckhzc.html

deque(maxlen=10)
来源：http://hz.cucudq.cn/gtfqrztnrt.html

[U14] Py：分组收集到列表
来源：http://hz.gogol.net.cn/gtpnieuhso.html

defaultdict(list)
来源：http://hz.sysykeji.top/gthzjerjez.html

[U15] Py：高精度计时
来源：http://hz.meibo888.top/gtarskmuxn.html

t = time.perf_counter()
来源：http://hz.ywan-chungtsiang.top/gtdrgjrnvq.html

[U16] Py：命令行参数解析
来源：http://hz.zhijiandao.cn/gtizrleagf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.quarkkingdee.top/gtxmpkchuu.html

[U17] Py：初始化日志
来源：http://hz.xinyue.icu/gtqaxiitum.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhixingplan.top/gtzwjkrnrb.html

[U18] Py：预编译正则
来源：http://hz.jqgfzy.top/gtpbnianuj.html

pat = re.compile(r"\d+")
来源：http://hz.c1oappe.top/gtdrrbprkm.html

[U19] Py：正则替换带回调
来源：http://hz.cucudq.cn/gtqlwjpeau.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jqgfzy.top/gtzcpqjhgi.html

[U20] Py：缓存函数结果
来源：http://hz.aizwys.cn/gtxasuuuhi.html

@functools.lru_cache(maxsize=None)
来源：http://hz.dashuyun.cn/gtmjtctomp.html

[U21] Py：自定义上下文管理器
来源：http://hz.sufxvd.cn/gtochwrdkl.html

@contextlib.contextmanager
来源：http://hz.fzhhl.top/gtayifwfrc.html

[U22] Py：矩阵转置
来源：http://hz.quarkkingdee.top/gtyeiczcol.html

list(zip(*m))
来源：http://hz.chenzaomai.com/gtsivlifch.html

[U23] Py：分块读取大文件
来源：http://hz.hnqzz.top/gtscvbjyzl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xinyue.icu/gtbeucsmas.html

[U24] Py：路径操作
来源：http://hz.andypj.xyz/gtzdenfksz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.shzxlz.cn/gtlyzbjtry.html

[U25] Py：CSV 按字典读
来源：http://hz.kuanghao11.cn/gtqvezcpjm.html

csv.DictReader(f)
来源：http://hz.xylfe.cn/gtogdyewlg.html

[U26] Py：并发下载
来源：http://hz.meibo888.top/gtwuncsaww.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jqgufenzy.top/gtbtwiklvx.html

[U27] Py：异步 HTTP
来源：http://hz.jqgfzy.top/gteqfkgwpe.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.haohaochexian.top/gtombfaknf.html

[U28] Py：类型别名
来源：http://hz.dashuyun.cn/gtxtvyuylz.html

UserId = int
来源：http://hz.andypj.xyz/gtveiguayu.html

[U29] Py：属性校验
来源：http://hz.yj20258.top/gtadyihijf.html

@property 与 @x.setter 配合
来源：http://hz.zhoulong.xyz/gtgpwvjrwb.html

[U30] Py：数据类
来源：http://hz.zhaomingkeji.xyz/gtsjtcykle.html

@dataclass(slots=True)
来源：http://hz.smart0.xyz/gtyatepvaq.html

[U31] Py：单测
来源：http://hz.gogol.net.cn/gtamxbkzqq.html

python -m pytest -q
来源：http://hz.xuanzx.com/gtswjyctfo.html

[U32] Py：代码格式化
来源：http://hz.sysykeji.top/gtohjsgncy.html

ruff format . && ruff check --fix .
来源：http://hz.cqqwz.cn/gtcjzowbdw.html

[U33] Py：打包发布
来源：http://hz.fengsongda.top/gtpbfzzvjr.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hammf.cn/gtetfkkzct.html

[U34] Py：判断编码
来源：http://hz.xylfe.cn/gtrbwjfcta.html

chardet.detect(raw)
来源：http://hz.aizwys.cn/gtsyjpkwja.html

[U35] Py：发送邮件
来源：http://hz.zhijiandao.cn/gtfrjslcqb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.jiagoushi.top/gtuttysaas.html

[U36] Py：定时任务
来源：http://hz.dianchejie.cn/gtkxxxdkzp.html

schedule.every(10).minutes.do(job)
来源：http://hz.aibaodan.cn/gtdibbwnmt.html

[U37] Py：读写 Excel
来源：http://hz.yuanzhike.top/gtjjejcvtn.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.svipenyu.cn/gtqqwughrp.html

[U38] Py：获取脚本所在目录
来源：http://hz.jinqigufen.top/gtmgxcrtji.html

Path(__file__).resolve().parent
来源：http://hz.zhixingplan.top/gtwzglcmkg.html

[U39] Py：判断是否在交互环境
来源：http://hz.gogol.net.cn/gtdfdtrjgw.html

sys.stdout.isatty()
来源：http://hz.guannengcc.top/gtrsulueix.html

[U40] Py：打印到标准错误
来源：http://hz.yanxiufei.cn/gtscgisfdi.html

print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtznmmbuuz.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jyoumei.cn/gtwdjfimvc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.haohaochexian.top/gtylilzhok.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xuetiantiany.cn/gtmpavsjxt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jinghuilouyu.cn/gtyjfvkfht.html

[U43] PHP：声明命名空间
来源：http://hz.jlsjyb.cn/gtcoaovehl.html

namespace App\Http;
来源：http://hz.zhijiandao.cn/gtyzuajopd.html

[U44] PHP：开启严格类型
来源：http://hz.yangfankeji.com/gtauvyqmqm.html

declare(strict_types=1);
来源：http://hz.daria6918.cn/gtwkmrrxrl.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shangyingyoupin.top/gtaurlqiqg.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtgbchwppb.html

[U46] PHP：可空类型
来源：http://hz.meibo888.top/gtulzcdmva.html

?string $name = null
来源：http://hz.jianghu66.top/gtofdcqpwu.html

[U47] PHP：联合类型
来源：http://hz.gzhubu.top/gtyeftcpnc.html

int|string $id
来源：http://hz.zhijiandao.cn/gtnxdehaex.html

[U48] PHP：纯枚举
来源：http://hz.kuanghao11.cn/gteawlxumk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.aibaodan.cn/gtlrqnmfsm.html

[U49] PHP：只读属性
来源：http://hz.chenzaomai.com/gtjcvpuxss.html

public readonly string $name
来源：http://hz.wangdashe.top/gtihaqzoyf.html

[U50] PHP：构造器属性提升
来源：http://hz.cdnleiting.top/gtesmtgorf.html

public function __construct(private int $id) {}
来源：http://hz.zycfv.cn/gtwswwgovs.html

[U51] PHP：数组解构
来源：http://hz.daria6918.cn/gtvcvrfsdd.html

[$a, $b] = $arr;
来源：http://hz.chenzaomai.com/gtoqqucnhn.html

[U52] PHP：箭头函数
来源：http://hz.hammf.cn/gttavlibzx.html

$double = fn($x) => $x * 2;
来源：http://hz.aibaodan.cn/gtfozrbvzz.html

[U53] PHP：空合并运算符
来源：http://hz.zhaomingkeji.xyz/gttxsfwuvy.html

$v = $a ?? $b ?? "default";
来源：http://hz.wangshuangyany.cn/gtukwfgooj.html

[U54] PHP：空安全调用
来源：http://hz.hnqzz.top/gttsxccczu.html

$obj?->method()
来源：http://hz.yangfankeji.com/gtlhhytljz.html

[U55] PHP：match 表达式
来源：http://hz.jyoumei.cn/gtinvjludl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ppjwa.cn/gtlvewxzoa.html

[U56] PHP：命名参数
来源：http://hz.xinyue.icu/gtpciylpjr.html

f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gthwnfkfgn.html

[U57] PHP：字符串插值
来源：http://hz.jiagoushi.top/gtaehwgeoh.html

"值: {$a}"
来源：http://hz.shuidangran.top/gtuefuicpd.html

[U58] PHP：数组三件套
来源：http://hz.nwbrower.top/gtyzfrlmha.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.pycfn.com/gtkjfyqagj.html


<!-- 参考信息 -->