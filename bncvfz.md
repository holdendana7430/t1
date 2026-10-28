代发 wailian999

[S37] C++：set
来源：http://hz.quarkkingdee.top/gthtdugqzv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yonumen.top/gtmtzguvhf.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gtaenpzlwd.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxinkj.top/gtmbnlylgz.html

[S39] C++：自定义比较器排序
来源：http://hz.haohaochexian.top/gtdpzzsqgi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jqgfzy.top/gtthaidlzd.html

[S40] C++：查找元素
来源：http://hz.hfpthk.cn/gtebfjsdng.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.redwolf501.top/gtqnhjuypj.html

[S41] C++：类与构造函数
来源：http://hz.dashuyun.cn/gtkebtueqq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.9152youxi.cn/gtmzykokzh.html

[S42] C++：继承与虚函数
来源：http://hz.shuidangran.top/gtxsifqrhd.html

class B : public Base { public: void f() override {} };
来源：http://hz.svipenyu.cn/gtsblxoyaw.html

[S43] C++：智能指针
来源：http://hz.aibaodan.cn/gtpcarrhwv.html

auto p = std::make_unique<int>(5);
来源：http://hz.shangyingyoupin.top/gtmwdbtehd.html

[S44] C++：引用传参
来源：http://hz.cheryme.top/gttyzpjmuf.html

void inc(int &x) { ++x; }
来源：http://hz.gaohongyu789.top/gtpidoizri.html

[S45] C++：lambda
来源：http://hz.yj202588.top/gtmthaacbs.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yueranfly.top/gthnrpxdbt.html

[S46] C++：函数模板
来源：http://hz.xziqi.cn/gtqordjmil.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xziqi.cn/gtcqkgsriq.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhengqikj.top/gtotcztvnb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sweek.top/gtlvhjwsyw.html

[S48] C++：逐行读文件
来源：http://hz.aibaodan.cn/gtaphfgqhl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydjk.org.cn/gtgkuntopn.html

while (std::getline(in, line)) { }
来源：http://hz.yangfankeji.com/gtwkkldwxp.html

[S49] C++：写文件
来源：http://hz.hysaishi.cn/gtxjzdssni.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.iojbl.cn/gtjnbffbgp.html

[S50] C++：格式化数字
来源：http://hz.nanxinkj.top/gtzewyyeoc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yj20258.top/gtpzdjvhmg.html

[S51] C++：显式类型转换
来源：http://hz.zhixingplan.top/gtylpjxnxc.html

static_cast<double>(a) / b
来源：http://hz.fzhhl.top/gtqakslmmt.html

[S52] C++：const 与 noexcept
来源：http://hz.guowangkeji.top/gtcnsrzwdv.html

int size() const noexcept { return n_; }
来源：http://hz.meibo888.top/gteavxypki.html

[S53] C++：移动语义
来源：http://hz.hammf.cn/gtvmtqscoo.html

std::vector<int> w = std::move(v);
来源：http://hz.yj202588.top/gtwbepefiw.html

[S54] C++：异常处理
来源：http://hz.pengpengdd.cyou/gtebolxhec.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cucudq.cn/gtyocvhlyo.html

[S55] C++：结构化绑定
来源：http://hz.birdmap.top/gtpsfpkxgy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.havefunace.top/gtnzshufhz.html

[S56] C++：optional
来源：http://hz.jiagoushi.top/gtkonnxqzg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yueranfly.top/gtvmbpnmbi.html

[S57] C++：编译期常量
来源：http://hz.chenzaomai.com/gtpulxlbhs.html

constexpr int N = 10;
来源：http://hz.meibo888.top/gtybwvwepd.html

[S58] C++：命名空间
来源：http://hz.shuidangran.top/gtzlxxgkqh.html

namespace ns { int f() { return 1; } }
来源：http://hz.hammf.cn/gtbbdfdutk.html

[S59] C++：静态断言
来源：http://hz.guowangkeji.top/gtdwqrqfdg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xylfe.cn/gtkatjtjlm.html

[S60] C++：遍历并删除元素
来源：http://hz.yj202588.top/gthpgrhqmi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinyuanbaomall.cn/gtpoigrumx.html

================================================================================
来源：http://hz.yongpay.top/gtvryrwvyg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yanxiufei.cn/gtkdflolhh.html

================================================================================
来源：http://hz.jianghu66.top/gtonpyvzvt.html

[T01] Kotlin：Hello World
来源：http://hz.cheryme.top/gtudgzexii.html

println("Hello")
来源：http://hz.svipenyu.cn/gtphlhecjo.html

[T02] Kotlin：变量
来源：http://hz.hnqzz.top/gtytvvetjk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.guowangkeji.top/gtpvshshcu.html

[T03] Kotlin：字符串模板
来源：http://hz.gogol.net.cn/gtgftyhcwh.html

"值: $b"
来源：http://hz.dashuyun.cn/gtlnkzsxbh.html

[T04] Kotlin：空安全
来源：http://hz.316326.xyz/gtbbvflmva.html

val n: String? = null;  n?.length
来源：http://hz.fzhhl.top/gtqvnlqeer.html

[T05] Kotlin：when 表达式
来源：http://hz.sxryk.cn/gtfimagejd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ppjwa.cn/gtpopmsxvi.html

[T06] Kotlin：集合映射
来源：http://hz.shanyushiyangkeji.top/gtrdoyeomf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhengqikj.top/gtvjzzkdlw.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgufenzy.top/gtnaoqshsr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shuidangran.top/gtgbtuyzza.html

[T08] Kotlin：数据类
来源：http://hz.havefunace.top/gtvijdzlha.html

data class User(val name: String, val age: Int)
来源：http://hz.quarkkingdee.top/gtlcosgvbk.html

[T09] Kotlin：扩展函数
来源：http://hz.xuanzx.com/gtsnnxvbwq.html

fun String.exclaim() = this + "!"
来源：http://hz.yj20258888.top/gtzdufzrqt.html

[T10] Kotlin：默认参数
来源：http://hz.haohaochexian.top/gtqyrhgkry.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhixingplan.top/gtkgtjqbvm.html

[T11] Kotlin：协程
来源：http://hz.haohaochexian.top/gtuksgovfp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.guannengcc.top/gtupztfdxt.html

[T12] Kotlin：解构声明
来源：http://hz.hongshengwenyu.top/gtahjtqlsd.html

val (a, b) = Pair(1, 2)
来源：http://hz.dianchejie.cn/gtzouebnbb.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtzcqbsocw.html

val m = mapOf("a" to 1)
来源：http://hz.yuxming.cn/gtfpxhkvjn.html

[T14] Kotlin：循环
来源：http://hz.c1oappe.top/gtlbflxcww.html

for (i in 1..10) println(i)
来源：http://hz.smart0.xyz/gtqkdiftnk.html

[T15] Kotlin：接口
来源：http://hz.yj20258888.top/gtblnchkmz.html

interface Shape { fun area(): Double }
来源：http://hz.vqdsnc.cn/gtzbxpmxkt.html

[T16] Swift：Hello World
来源：http://hz.shuidangran.top/gtbytstads.html

print("Hello")
来源：http://hz.havefunace.top/gtexuggjdy.html

[T17] Swift：变量与常量
来源：http://hz.shanyushiyangkeji.top/gtlegtmlou.html

var a = 1;  let b = 2
来源：http://hz.cqqwz.cn/gtetjoohba.html

[T18] Swift：字符串插值
来源：http://hz.xziqi.cn/gtyucyfegm.html

"值: \(b)"
来源：http://hz.zhixingplan.top/gtqmoleimw.html

[T19] Swift：可选绑定
来源：http://hz.wangshuangyany.cn/gtiagszsdo.html

if let n = opt { print(n) }
来源：http://hz.ivvv.top/gtlaoqwpyt.html

[T20] Swift：数组操作
来源：http://hz.ydjk.org.cn/gtnfcvhsau.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gogol.net.cn/gttxhnkgju.html

[T21] Swift：遍历
来源：http://hz.gotoacloud.top/gtzhijidmn.html

for x in a { print(x) }
来源：http://hz.chenzaomai.com/gtxbbpcmni.html

[T22] Swift：字典
来源：http://hz.sufxvd.cn/gtfrchajcs.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.feifeiyinyue.top/gtetxktgvg.html

[T23] Swift：函数
来源：http://hz.jianghu66.top/gtbslkfomw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hongshengwenyu.top/gtckuvhvzp.html

[T24] Swift：闭包
来源：http://hz.guowangkeji.top/gtuggjznia.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.sxryk.cn/gtpqxdzzdx.html

[T25] Swift：结构体
来源：http://hz.wangshuangyany.cn/gtmcddtxtb.html

struct P { var x: Int }
来源：http://hz.chenlongwang.top/gtkklhyphh.html

[T26] Swift：类与重写
来源：http://hz.gogol.net.cn/gtrywdacbt.html

class A: Base { override func f() {} }
来源：http://hz.gaohongyu789.top/gtiupzluef.html

[T27] Swift：错误处理
来源：http://hz.feifeiyinyue.top/gtcicrswsz.html

do { try f() } catch { print(error) }
来源：http://hz.yj202588.top/gttaxevfiu.html

[T28] Swift：枚举
来源：http://hz.guowangkeji.top/gtfskyvzbc.html

enum Color { case red, green }
来源：http://hz.tianlin.xyz/gttqunkrig.html

[T29] Swift：guard 提前返回
来源：http://hz.zycfv.cn/gthktbakvf.html

guard let x = opt else { return }
来源：http://hz.zhijiandao.cn/gtrchwuisb.html

[T30] Swift：协议
来源：http://hz.zhoulong.xyz/gtchvrgkgq.html

protocol Shape { func area() -> Double }
来源：http://hz.yj202588.top/gttbvqwvsl.html

[T31] Lua：Hello World
来源：http://hz.cashguo.top/gtcupvxohn.html

print("Hello")
来源：http://hz.wangshuangyany.cn/gtqskjyrch.html

[T32] Lua：局部变量
来源：http://hz.jianghu66.top/gtinfrncdh.html

local a = 1
来源：http://hz.zycfv.cn/gtntebxuos.html

[T33] Lua：表（数组）
来源：http://hz.aibaodan.cn/gtqvilaypq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.aibaodan.cn/gtzlqwadta.html

[T34] Lua：遍历表
来源：http://hz.cheryme.top/gtwldcqvbj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.9152youxi.cn/gtpbrmgewl.html

[T35] Lua：字典表
来源：http://hz.jqgufenzy.top/gtbuiolemt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.birdmap.top/gtuksumpjh.html

[T36] Lua：函数
来源：http://hz.jlsjyb.cn/gtailcqunl.html

function add(a, b) return a + b end
来源：http://hz.daxiang520.top/gtqaryhmrw.html

[T37] Lua：字符串拼接
来源：http://hz.daria6918.cn/gtbdeaiscs.html

"a" .. "b"
来源：http://hz.yanxiufei.cn/gtansherxq.html

[T38] Lua：条件
来源：http://hz.shanyushiyangtech.top/gtmeilicpr.html

if x > 0 then print("正") end
来源：http://hz.jianghu66.top/gtmdieftde.html

[T39] Lua：模式匹配
来源：http://hz.yongpay.top/gtpmegrtry.html

string.find(s, "%d+")
来源：http://hz.hnxiangtu.top/gtvqbckpgh.html

[T40] Lua：元表
来源：http://hz.iojbl.cn/gtqngeiswg.html

setmetatable({}, { __index = base })
来源：http://hz.chenlongwang.top/gtuwjjuukd.html

[T41] Perl：Hello World
来源：http://hz.zycfv.cn/gtsujbtpls.html

print "Hello\n";
来源：http://hz.jlsjyb.cn/gtvpnbmcbn.html

[T42] Perl：变量类型
来源：http://hz.jinyuanbaomall.cn/gtpubliiqj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.aizwys.cn/gtmmismdlo.html

[T43] Perl：字符串插值
来源：http://hz.xziqi.cn/gtgwctmmxt.html

"值: $a"
来源：http://hz.nanxuanxn.top/gtibqzcydc.html

[T44] Perl：条件
来源：http://hz.c1oappe.top/gtedsnphza.html

if ($a > 0) { print "正"; }
来源：http://hz.aizwys.cn/gtvbyuqzbc.html

[T45] Perl：数组遍历
来源：http://hz.yj20258888.top/gtsspvvkpt.html

for my $x (@arr) { print $x; }
来源：http://hz.cdnleiting.top/gtfocsgmlr.html

[T46] Perl：哈希操作
来源：http://hz.bjfxy.top/gtpxobgxjq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yangfankeji.com/gtjaecctyw.html

[T47] Perl：正则捕获
来源：http://hz.cucudq.cn/gtyliiwotg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jyoumei.cn/gtixdpbbqn.html

[T48] Perl：正则替换
来源：http://hz.dashuyun.cn/gtlnxqwsxs.html

$s =~ s/old/new/g;
来源：http://hz.nanxinkj.top/gtabrjbzmd.html

[T49] Perl：函数
来源：http://hz.zhongyouzk.top/gtyrgjjihe.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gotoacloud.top/gtpnfsyyxd.html

[T50] Perl：逐行读文件
来源：http://hz.shuidangran.top/gtodikynfk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.feifeiyinyue.top/gthficwwlt.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.yueranfly.top/gtifajjagz.html

[T51] Scala：Hello World
来源：http://hz.mhx1999.top/gtuzukyhzv.html

println("Hello")
来源：http://hz.cdnleiting.top/gtvyhtxbks.html

[T52] Scala：变量
来源：http://hz.jyoumei.cn/gtbxqydipi.html

val a = 1;  var b = 2
来源：http://hz.hysaishi.cn/gttjdkkflm.html

[T53] Scala：字符串插值
来源：http://hz.gogol.net.cn/gtxniptrpa.html

s"值: $b"
来源：http://hz.wangshuangyany.cn/gtddpdpzno.html

[T54] Scala：集合映射
来源：http://hz.fengsongda.top/gtcmiquqgf.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhixingplan.top/gtnhmcbvzu.html

[T55] Scala：集合过滤
来源：http://hz.yuanzhike.top/gtmphtprqq.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tanke756.top/gtkywxxeyx.html

[T56] Scala：样例类
来源：http://hz.smart0.xyz/gtqbcrxuwy.html

case class User(name: String, age: Int)
来源：http://hz.zhijiandao.cn/gtmlwvqkiu.html

[T57] Scala：模式匹配
来源：http://hz.zhaomingkeji.xyz/gtsdqzyzyk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.yongpay.top/gtsejoecct.html

[T58] Scala：函数定义
来源：http://hz.ivvv.top/gtyaljwnag.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jyoumei.cn/gtlpnmgqct.html

[T59] Scala：循环
来源：http://hz.yueranfly.top/gtmhpweazu.html

for (i <- 1 to 10) println(i)
来源：http://hz.wangdashe.top/gtcsohwgcj.html

[T60] Scala：折叠
来源：http://hz.chenzaomai.com/gtpcvuxhyi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.yj20258888.top/gtvzyukwxy.html

================================================================================
来源：http://hz.cdnleiting.top/gtghongywf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.meibo888.top/gtlvgtecrn.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgwjlbbns.html

[U01] Py：创建虚拟环境
来源：http://hz.tian-w.cn/gtevdwrhpd.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jiagoushi.top/gtyjvkjyhm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.cdnleiting.top/gtirghwqbq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.haohaochexian.top/gtjibxkmag.html

[U03] Py：加载 .env 配置
来源：http://hz.zhijiandao.cn/gtbntegbue.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jlsjyb.cn/gtyyxremzn.html

[U04] Py：变量调试打印
来源：http://hz.jyoumei.cn/gtaofmznii.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.9152youxi.cn/gtqeysqxif.html

[U05] Py：列表去重且保序
来源：http://hz.hfpthk.cn/gtqerpudla.html

list(dict.fromkeys(arr))
来源：http://hz.hywenlv.cn/gtybdvhrgv.html

[U06] Py：合并两个字典
来源：http://hz.gogol.net.cn/gtquwkrmjv.html

{**a, **b}
来源：http://hz.xziqi.cn/gtnfvrvauy.html

[U07] Py：反转字典键值
来源：http://hz.havefunace.top/gtjxzazyyl.html

{v: k for k, v in d.items()}
来源：http://hz.bjfxy.top/gtznqcntwc.html

[U08] Py：展平二维列表
来源：http://hz.tanke756.top/gtyatmiggi.html

[y for x in nested for y in x]
来源：http://hz.birdmap.top/gtpzzsvivl.html

[U09] Py：字典取最大值的键
来源：http://hz.pengpengdd.cyou/gtsmkhhwif.html

max(d, key=d.get)
来源：http://hz.ydzc1.top/gtxpjrlnqq.html

[U10] Py：按值排序字典
来源：http://hz.zhaomingkeji.xyz/gtwvgahmxi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.dianchejie.cn/gtpxytbqbp.html

[U11] Py：生成器表达式
来源：http://hz.ybcxt.top/gtnaoqsyrn.html

(x * 2 for x in arr)
来源：http://hz.ywan-chungtsiang.top/gtniwvvnmw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.andypj.xyz/gtzbhzqwno.html

Counter(arr).most_common(3)
来源：http://hz.jyoumei.cn/gtxdrfhvlu.html

[U13] Py：固定长度队列
来源：http://hz.hywenlv.cn/gtnzjxmukm.html

deque(maxlen=10)
来源：http://hz.chenjidiqi.icu/gtnflgqeci.html

[U14] Py：分组收集到列表
来源：http://hz.zhengqikj.top/gtrpxuzrde.html

defaultdict(list)
来源：http://hz.chenjidiqi.icu/gtbzeablvv.html

[U15] Py：高精度计时
来源：http://hz.hnqzz.top/gtdzdvkgqp.html

t = time.perf_counter()
来源：http://hz.xziqi.cn/gtextafuru.html

[U16] Py：命令行参数解析
来源：http://hz.fengsongda.top/gtyyorutox.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.feifeiyinyue.top/gtqmfakfdp.html

[U17] Py：初始化日志
来源：http://hz.yvedp.cn/gtkeqnfdgv.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.aibaodan.cn/gtojewkxtq.html

[U18] Py：预编译正则
来源：http://hz.xziqi.cn/gtruqlvvzt.html

pat = re.compile(r"\d+")
来源：http://hz.guowangkeji.top/gtsftywfhw.html

[U19] Py：正则替换带回调
来源：http://hz.jinqigufen.top/gtrfphantp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cdnleiting.top/gthexjyqkq.html

[U20] Py：缓存函数结果
来源：http://hz.yanxiufei.cn/gtkuwmjbwp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhiwuduotai.top/gtboshrdbh.html

[U21] Py：自定义上下文管理器
来源：http://hz.andypj.xyz/gtnxsawyre.html

@contextlib.contextmanager
来源：http://hz.zhongyouzk.top/gtivavfgxe.html

[U22] Py：矩阵转置
来源：http://hz.yj202588.top/gtodvpuvjg.html

list(zip(*m))
来源：http://hz.yvedp.cn/gtvdoficwe.html

[U23] Py：分块读取大文件
来源：http://hz.chenzaomai.com/gtisjpdgjb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jiagoushi.top/gteejrotyl.html

[U24] Py：路径操作
来源：http://hz.52xcode.cn/gtlqlgsjje.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.hfpthk.cn/gtbdxnnxme.html

[U25] Py：CSV 按字典读
来源：http://hz.fengsongda.top/gthklhhufi.html

csv.DictReader(f)
来源：http://hz.nanxuanxn.top/gtngryohee.html

[U26] Py：并发下载
来源：http://hz.yangfankeji.com/gtwfwsmbii.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.dianchejie.cn/gtdndzewdt.html

[U27] Py：异步 HTTP
来源：http://hz.hnxiangtu.top/gtmrpjezdw.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.zhengqikj.top/gteraphecz.html

[U28] Py：类型别名
来源：http://hz.ivvv.top/gtutarqtqc.html

UserId = int
来源：http://hz.yonumen.top/gtdipbbsam.html

[U29] Py：属性校验
来源：http://hz.zdqjudy.top/gtmhwlzcgs.html

@property 与 @x.setter 配合
来源：http://hz.hywenlv.cn/gtomemftka.html

[U30] Py：数据类
来源：http://hz.zhiwuduotai.top/gtdasiuqvj.html

@dataclass(slots=True)
来源：http://hz.cqqwz.cn/gtlihkhwkl.html

[U31] Py：单测
来源：http://hz.redwolf501.top/gtjlwvgagn.html

python -m pytest -q
来源：http://hz.hywenlv.cn/gtcmviszjb.html

[U32] Py：代码格式化
来源：http://hz.haohaochexian.top/gtwliorobm.html

ruff format . && ruff check --fix .
来源：http://hz.pycfn.com/gtxhgoiekk.html

[U33] Py：打包发布
来源：http://hz.svipenyu.cn/gtlwagsbiv.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.9152youxi.cn/gtuzpwyesd.html

[U34] Py：判断编码
来源：http://hz.ywan-chungtsiang.top/gtvaetdnyv.html

chardet.detect(raw)
来源：http://hz.jlsjyb.cn/gtykfpsqqx.html

[U35] Py：发送邮件
来源：http://hz.cucudq.cn/gtziyzphlw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.zhoulong.xyz/gteicjaauo.html

[U36] Py：定时任务
来源：http://hz.tanke756.top/gtratwxgnk.html

schedule.every(10).minutes.do(job)
来源：http://hz.nanxinkj.top/gtxzswrlwt.html

[U37] Py：读写 Excel
来源：http://hz.tanke756.top/gtstsbsrzd.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.andypj.xyz/gtypjclsse.html

[U38] Py：获取脚本所在目录
来源：http://hz.yueranfly.top/gtouypmpzx.html

Path(__file__).resolve().parent
来源：http://hz.zhaomingkeji.xyz/gtlurkudkl.html

[U39] Py：判断是否在交互环境
来源：http://hz.nwbrower.top/gtiwpwmvib.html

sys.stdout.isatty()
来源：http://hz.sweek.top/gtzsuoqehc.html

[U40] Py：打印到标准错误
来源：http://hz.feifeiyinyue.top/gtghbcnaji.html

print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gthbudgirl.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ivvv.top/gtqczbejyf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.sweek.top/gtbaxitiue.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.sweek.top/gtlnwcykei.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.xuetiantiany.cn/gtxfwvnhky.html

[U43] PHP：声明命名空间
来源：http://hz.iojbl.cn/gtuciaoudm.html

namespace App\Http;
来源：http://hz.dashuyun.cn/gtxugpznjw.html

[U44] PHP：开启严格类型
来源：http://hz.c1oappe.top/gtnmvddsin.html

declare(strict_types=1);
来源：http://hz.cqqwz.cn/gtuupqdvud.html

[U45] PHP：类型声明与返回类型
来源：http://hz.shanyushiyangkeji.top/gtmkjjiyzl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ppjwa.cn/gtbajmgdnz.html

[U46] PHP：可空类型
来源：http://hz.pengpengdd.cyou/gtgwwyjofl.html

?string $name = null
来源：http://hz.haohaochexian.top/gtbmtzggrk.html

[U47] PHP：联合类型
来源：http://hz.mhx1999.top/gtbwwhpxra.html

int|string $id
来源：http://hz.gzhubu.top/gtorsvydxx.html

[U48] PHP：纯枚举
来源：http://hz.smart0.xyz/gtajrfqlqe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yj20258.top/gtfwcyjqzp.html

[U49] PHP：只读属性
来源：http://hz.wangdashe.top/gtrnihzjer.html

public readonly string $name
来源：http://hz.havefunace.top/gtdfpmaexk.html

[U50] PHP：构造器属性提升
来源：http://hz.tianlin.xyz/gtpjwfljzg.html

public function __construct(private int $id) {}
来源：http://hz.gotoacloud.top/gtxzamdehw.html

[U51] PHP：数组解构
来源：http://hz.c1oappe.top/gtcoywbojl.html

[$a, $b] = $arr;
来源：http://hz.fengsongda.top/gtzzerlvjo.html

[U52] PHP：箭头函数
来源：http://hz.yj202588.top/gtjpvvcfov.html

$double = fn($x) => $x * 2;
来源：http://hz.andypj.xyz/gtwskahtbe.html

[U53] PHP：空合并运算符
来源：http://hz.tianlin.xyz/gtnmzfucwu.html

$v = $a ?? $b ?? "default";
来源：http://hz.jinqigufen.top/gtqaokzila.html

[U54] PHP：空安全调用
来源：http://hz.yuanzhike.top/gtzfqkwwuw.html

$obj?->method()
来源：http://hz.yonumen.top/gtnrrphamv.html

[U55] PHP：match 表达式
来源：http://hz.haohaochexian.top/gtkiyijabb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.zhaomingkeji.xyz/gtriosymle.html

[U56] PHP：命名参数
来源：http://hz.cashguo.top/gteecwuvdk.html

f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtluznitew.html

[U57] PHP：字符串插值
来源：http://hz.kuanghao11.cn/gtbxpetnvl.html

"值: {$a}"
来源：http://hz.nanxinkj.top/gtzsrtuejn.html

[U58] PHP：数组三件套
来源：http://hz.dashuyun.cn/gtblruzrhg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.fengsongda.top/gtshwixpfi.html

[U59] PHP：自定义排序
来源：http://hz.zdqjudy.top/gtqawxcfhk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuanzx.com/gtohayqigo.html

[U60] PHP：JSON 编解码
来源：http://hz.ydzc1.top/gtdoifapsk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.sweek.top/gtfrbxhlyc.html

[U61] PHP：正则
来源：http://hz.kuanghao11.cn/gtqkjqfhlg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnqzz.top/gtvcjpowoq.html

[U62] PHP：日期对象
来源：http://hz.zhongyouzk.top/gthjehwajl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.iojbl.cn/gtwflksehq.html


<!-- 参考信息 -->