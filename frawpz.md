代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://hz.kuanghao11.cn/gtxrzxdqzr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guowangkeji.top/gtycliuegk.html

[S48] C++：逐行读文件
来源：http://hz.daria6918.cn/gtrsxifxgb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cqqwz.cn/gtcxhbckyx.html

while (std::getline(in, line)) { }
来源：http://hz.nwbrower.top/gtwowfwocu.html

[S49] C++：写文件
来源：http://hz.hammf.cn/gtfhqezvqf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.meibo888.top/gtypoqyqtz.html

[S50] C++：格式化数字
来源：http://hz.redwolf501.top/gtyihnmqdo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.wangdashe.top/gtjykdvtpk.html

[S51] C++：显式类型转换
来源：http://hz.yongpay.top/gtlagnppbw.html

static_cast<double>(a) / b
来源：http://hz.zhoulong.xyz/gtrxkcwwfr.html

[S52] C++：const 与 noexcept
来源：http://hz.zycfv.cn/gtyurcfnxw.html

int size() const noexcept { return n_; }
来源：http://hz.hammf.cn/gtldqvpypf.html

[S53] C++：移动语义
来源：http://hz.svipenyu.cn/gtlgzauojy.html

std::vector<int> w = std::move(v);
来源：http://hz.zycfv.cn/gtgqowvqkz.html

[S54] C++：异常处理
来源：http://hz.fzhhl.top/gtdtbgjmsd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.smart0.xyz/gtouwdhqkd.html

[S55] C++：结构化绑定
来源：http://hz.ybcxt.top/gtbhdisjbz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.wangshuangyany.cn/gtvxrkanzk.html

[S56] C++：optional
来源：http://hz.jinqigufen.top/gtmkmvrytt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.0kj1m.cn/gtnkjvltnu.html

[S57] C++：编译期常量
来源：http://hz.chenjidiqi.icu/gttkdamiae.html

constexpr int N = 10;
来源：http://hz.zdqjudy.top/gtsjbwwbvl.html

[S58] C++：命名空间
来源：http://hz.hysaishi.cn/gtowfxnvso.html

namespace ns { int f() { return 1; } }
来源：http://hz.hnxiangtu.top/gtqanahfcj.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gtecnecsaz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.wangshuangyany.cn/gtmndmgrbt.html

[S60] C++：遍历并删除元素
来源：http://hz.chenzaomai.com/gtedyiwtfw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.svipenyu.cn/gtfflpleax.html

================================================================================
来源：http://hz.0kj1m.cn/gtudyfbswq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtnxhwlogx.html

================================================================================
来源：http://hz.gogol.net.cn/gtfxotxzqg.html

[T01] Kotlin：Hello World
来源：http://hz.wangdashe.top/gtpgxkaxph.html

println("Hello")
来源：http://hz.yuxming.cn/gtkesihdvx.html

[T02] Kotlin：变量
来源：http://hz.haohaochexian.top/gtbohnuvqy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xuanzx.com/gtafvkekcv.html

[T03] Kotlin：字符串模板
来源：http://hz.andypj.xyz/gttjgvcgmv.html

"值: $b"
来源：http://hz.daria6918.cn/gtprtmrsrr.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangtech.top/gtszowddnl.html

val n: String? = null;  n?.length
来源：http://hz.hysaishi.cn/gtpgldraol.html

[T05] Kotlin：when 表达式
来源：http://hz.fengsongda.top/gtfxbkpzer.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.iojbl.cn/gtsecbapae.html

[T06] Kotlin：集合映射
来源：http://hz.shangyingyoupin.top/gtxmtbcsyp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yuxming.cn/gtqxclhehr.html

[T07] Kotlin：集合过滤
来源：http://hz.9152youxi.cn/gtydgdbbem.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuxming.cn/gtahvsrjyv.html

[T08] Kotlin：数据类
来源：http://hz.yuxming.cn/gtkisdodpc.html

data class User(val name: String, val age: Int)
来源：http://hz.aibaodan.cn/gtfmrilsqb.html

[T09] Kotlin：扩展函数
来源：http://hz.ivvv.top/gtrqbhdxey.html

fun String.exclaim() = this + "!"
来源：http://hz.sweek.top/gtzcxylxuk.html

[T10] Kotlin：默认参数
来源：http://hz.iojbl.cn/gthqdnksjw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.nanxuanxn.top/gtaxyfwthm.html

[T11] Kotlin：协程
来源：http://hz.yuanzhike.top/gtiqvqqnxn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhijiandao.cn/gtnmuenmfx.html

[T12] Kotlin：解构声明
来源：http://hz.andypj.xyz/gtsdjulkqh.html

val (a, b) = Pair(1, 2)
来源：http://hz.sysykeji.top/gtrqmdgzfv.html

[T13] Kotlin：只读 Map
来源：http://hz.meibo888.top/gtjpnfzwll.html

val m = mapOf("a" to 1)
来源：http://hz.zhijiandao.cn/gtckjzyklz.html

[T14] Kotlin：循环
来源：http://hz.vqdsnc.cn/gtvgtcysym.html

for (i in 1..10) println(i)
来源：http://hz.tianlin.xyz/gtlkikovyd.html

[T15] Kotlin：接口
来源：http://hz.yueranfly.top/gtiunaiucm.html

interface Shape { fun area(): Double }
来源：http://hz.yanxiufei.cn/gtyrmvnddv.html

[T16] Swift：Hello World
来源：http://hz.xylfe.cn/gtutqsohob.html

print("Hello")
来源：http://hz.bjfxy.top/gtonbhmnfj.html

[T17] Swift：变量与常量
来源：http://hz.jyoumei.cn/gtjzhltohu.html

var a = 1;  let b = 2
来源：http://hz.gotoacloud.top/gtmrkjjzfo.html

[T18] Swift：字符串插值
来源：http://hz.316326.xyz/gtyquohkbp.html

"值: \(b)"
来源：http://hz.iojbl.cn/gthheqymft.html

[T19] Swift：可选绑定
来源：http://hz.ydjk.org.cn/gtspdjigsd.html

if let n = opt { print(n) }
来源：http://hz.nanxuanxn.top/gtomzjqhgf.html

[T20] Swift：数组操作
来源：http://hz.meibo888.top/gttrktzaww.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jianghu66.top/gtipojulft.html

[T21] Swift：遍历
来源：http://hz.iojbl.cn/gtzkkmvkpw.html

for x in a { print(x) }
来源：http://hz.hfpthk.cn/gtwhytcijq.html

[T22] Swift：字典
来源：http://hz.cucudq.cn/gtwudivpow.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jqgfzy.top/gtrsasgffd.html

[T23] Swift：函数
来源：http://hz.daria6918.cn/gtmlypupxj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhongyouzk.top/gthtpjojwp.html

[T24] Swift：闭包
来源：http://hz.cheryme.top/gteanbszrm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhongyouzk.top/gtflqvwsdh.html

[T25] Swift：结构体
来源：http://hz.hnqzz.top/gtsjqofxej.html

struct P { var x: Int }
来源：http://hz.daxiang520.top/gtbwkaypkv.html

[T26] Swift：类与重写
来源：http://hz.snrcjt.cn/gtvfzligzd.html

class A: Base { override func f() {} }
来源：http://hz.52xcode.cn/gtaeyxgocx.html

[T27] Swift：错误处理
来源：http://hz.bjfxy.top/gtwedeelcj.html

do { try f() } catch { print(error) }
来源：http://hz.jinghuilouyu.cn/gtjzkswmsm.html

[T28] Swift：枚举
来源：http://hz.shzxlz.cn/gtihmrdsec.html

enum Color { case red, green }
来源：http://hz.yangfankeji.com/gtufonogsk.html

[T29] Swift：guard 提前返回
来源：http://hz.haohaochexian.top/gtcatdgbiz.html

guard let x = opt else { return }
来源：http://hz.xylfe.cn/gtcelczyke.html

[T30] Swift：协议
来源：http://hz.aibaodan.cn/gtlortgmry.html

protocol Shape { func area() -> Double }
来源：http://hz.zhijiandao.cn/gtkoatmveo.html

[T31] Lua：Hello World
来源：http://hz.smart0.xyz/gtqzmzwuum.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtcjmbkjtd.html

[T32] Lua：局部变量
来源：http://hz.chenlongwang.top/gthulbgfzu.html

local a = 1
来源：http://hz.gotoacloud.top/gthghnwkwb.html

[T33] Lua：表（数组）
来源：http://hz.ybcxt.top/gtrdxcyboh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.tanke756.top/gtaydopjtl.html

[T34] Lua：遍历表
来源：http://hz.ywan-chungtsiang.top/gtgonkapjx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cheryme.top/gtwxlnguou.html

[T35] Lua：字典表
来源：http://hz.hysaishi.cn/gtloetvggn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.redwolf501.top/gtbwruigsl.html

[T36] Lua：函数
来源：http://hz.nanxinkj.top/gtoilbmeon.html

function add(a, b) return a + b end
来源：http://hz.jiagoushi.top/gttflqibke.html

[T37] Lua：字符串拼接
来源：http://hz.shanyushiyangkeji.top/gtkribzaty.html

"a" .. "b"
来源：http://hz.aizwys.cn/gtjjttyfnb.html

[T38] Lua：条件
来源：http://hz.zhaomingkeji.xyz/gtslgzmybv.html

if x > 0 then print("正") end
来源：http://hz.ivvv.top/gtunjubska.html

[T39] Lua：模式匹配
来源：http://hz.xuetiantiany.cn/gtfchoakdz.html

string.find(s, "%d+")
来源：http://hz.jlsjyb.cn/gtlfqdfwqc.html

[T40] Lua：元表
来源：http://hz.tianlin.xyz/gtngpclytp.html

setmetatable({}, { __index = base })
来源：http://hz.nanxuanxn.top/gtnqcrolum.html

[T41] Perl：Hello World
来源：http://hz.ehwqpu.com/gtjatyxztw.html

print "Hello\n";
来源：http://hz.jinqigfzy.top/gtubyniczh.html

[T42] Perl：变量类型
来源：http://hz.bjfxy.top/gttgoylzwl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jiagoushi.top/gtztkdvryh.html

[T43] Perl：字符串插值
来源：http://hz.shanyushiyangtech.top/gtbkasvpia.html

"值: $a"
来源：http://hz.jinqigfzy.top/gtbtfrphii.html

[T44] Perl：条件
来源：http://hz.haohaochexian.top/gtqvqaijqy.html

if ($a > 0) { print "正"; }
来源：http://hz.snrcjt.cn/gtdsnsdblm.html

[T45] Perl：数组遍历
来源：http://hz.hongshengwenyu.top/gtnsfmlcve.html

for my $x (@arr) { print $x; }
来源：http://hz.haohaochexian.top/gtlprranum.html

[T46] Perl：哈希操作
来源：http://hz.hnxiangtu.top/gtjiplfpwq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xinyue.icu/gteiemmmvn.html

[T47] Perl：正则捕获
来源：http://hz.gaohongyu789.top/gthreabxwt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.pycfn.com/gtzzotdzoa.html

[T48] Perl：正则替换
来源：http://hz.0kj1m.cn/gthpqtuhpn.html

$s =~ s/old/new/g;
来源：http://hz.shanyushiyangtech.top/gtgsbefwci.html

[T49] Perl：函数
来源：http://hz.sweek.top/gtfcoecfdk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ppjwa.cn/gtaztmkxdj.html

[T50] Perl：逐行读文件
来源：http://hz.shangyingyoupin.top/gtwbiyzmzm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ppjwa.cn/gthgytromv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.haohaochexian.top/gtiopjnmul.html

[T51] Scala：Hello World
来源：http://hz.wangdashe.top/gtrijknxnl.html

println("Hello")
来源：http://hz.52xcode.cn/gtnixfaysh.html

[T52] Scala：变量
来源：http://hz.meibo888.top/gtblfiqzta.html

val a = 1;  var b = 2
来源：http://hz.cdnleiting.top/gtiaxzjpcf.html

[T53] Scala：字符串插值
来源：http://hz.ivvv.top/gtwqqewkzp.html

s"值: $b"
来源：http://hz.dianchejie.cn/gtpgoujedb.html

[T54] Scala：集合映射
来源：http://hz.zhixingplan.top/gtxohtgqbl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yj20258888.top/gtzhmkysmg.html

[T55] Scala：集合过滤
来源：http://hz.jiagoushi.top/gtutiowwvr.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinqigfzy.top/gtmfwweidh.html

[T56] Scala：样例类
来源：http://hz.yj202588.top/gtzvuurbui.html

case class User(name: String, age: Int)
来源：http://hz.shuidangran.top/gtqvzgbmhu.html

[T57] Scala：模式匹配
来源：http://hz.ydzc1.top/gtrozunenm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xziqi.cn/gtjkkwsvmn.html

[T58] Scala：函数定义
来源：http://hz.gogol.net.cn/gtupcxmren.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ydjk.org.cn/gtwhqrctqb.html

[T59] Scala：循环
来源：http://hz.cashguo.top/gtpxmohtvw.html

for (i <- 1 to 10) println(i)
来源：http://hz.bjfxy.top/gtfsumqosg.html

[T60] Scala：折叠
来源：http://hz.hnqzz.top/gtmlcvwzdh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.9152youxi.cn/gtnbemyupo.html

================================================================================
来源：http://hz.bjfxy.top/gtrrrxjyxf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.quarkkingdee.top/gtmuelgxnl.html

================================================================================
来源：http://hz.shuidangran.top/gtlfqxukqc.html

[U01] Py：创建虚拟环境
来源：http://hz.jqgufenzy.top/gtiwjmkxou.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hammf.cn/gtouyaknai.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xuanzx.com/gtlfgpstlq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sweek.top/gtzfeadrel.html

[U03] Py：加载 .env 配置
来源：http://hz.yangfankeji.com/gtsmenjqmt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.dashuyun.cn/gthpaplekc.html

[U04] Py：变量调试打印
来源：http://hz.fengsongda.top/gtcwkxzkrb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.haohaochexian.top/gtqeyyddwl.html

[U05] Py：列表去重且保序
来源：http://hz.yangfankeji.com/gtadytpdxv.html

list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtnieuamtu.html

[U06] Py：合并两个字典
来源：http://hz.zhijiandao.cn/gtegpbpcbh.html

{**a, **b}
来源：http://hz.nanxuanxn.top/gtxerltzxm.html

[U07] Py：反转字典键值
来源：http://hz.haohaochexian.top/gtgwicemss.html

{v: k for k, v in d.items()}
来源：http://hz.yj20258.top/gtrftytjyn.html

[U08] Py：展平二维列表
来源：http://hz.yuxming.cn/gtofzozekp.html

[y for x in nested for y in x]
来源：http://hz.yueranfly.top/gtfjrigaum.html

[U09] Py：字典取最大值的键
来源：http://hz.ehwqpu.com/gtmjkdciax.html

max(d, key=d.get)
来源：http://hz.dashuyun.cn/gteqkmolpe.html

[U10] Py：按值排序字典
来源：http://hz.andypj.xyz/gttdzefjzl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.nwbrower.top/gtrwbhibxu.html

[U11] Py：生成器表达式
来源：http://hz.xuetiantiany.cn/gtntomfeaj.html

(x * 2 for x in arr)
来源：http://hz.yuanzhike.top/gtyokeqrsd.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ivvv.top/gtkltuyapa.html

Counter(arr).most_common(3)
来源：http://hz.9152youxi.cn/gtnknwmvaj.html

[U13] Py：固定长度队列
来源：http://hz.fzhhl.top/gtmkhvvanu.html

deque(maxlen=10)
来源：http://hz.xziqi.cn/gtovpjbavq.html

[U14] Py：分组收集到列表
来源：http://hz.cqqwz.cn/gtvvqhvoqx.html

defaultdict(list)
来源：http://hz.gogol.net.cn/gtknkeejci.html

[U15] Py：高精度计时
来源：http://hz.xinyue.icu/gtpuventsc.html

t = time.perf_counter()
来源：http://hz.hywenlv.cn/gtrtgweaha.html

[U16] Py：命令行参数解析
来源：http://hz.0kj1m.cn/gtupbbpvgt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhoulong.xyz/gtprzysldm.html

[U17] Py：初始化日志
来源：http://hz.kuanghao11.cn/gtdfdeswjw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.dianchejie.cn/gtsvowsges.html

[U18] Py：预编译正则
来源：http://hz.shzxlz.cn/gtgjeztily.html

pat = re.compile(r"\d+")
来源：http://hz.gogol.net.cn/gtzhefnafg.html

[U19] Py：正则替换带回调
来源：http://hz.ydzc1.top/gtnzfkahvx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xinyue.icu/gtblbwciym.html

[U20] Py：缓存函数结果
来源：http://hz.cqqwz.cn/gtprpfmhzt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhaomingkeji.xyz/gtwhudokjt.html

[U21] Py：自定义上下文管理器
来源：http://hz.yvedp.cn/gtvgxqacne.html

@contextlib.contextmanager
来源：http://hz.hysaishi.cn/gtiexijqmb.html

[U22] Py：矩阵转置
来源：http://hz.sysykeji.top/gtjniygmso.html

list(zip(*m))
来源：http://hz.jinghuilouyu.cn/gthtqabuwc.html

[U23] Py：分块读取大文件
来源：http://hz.jqgufenzy.top/gtpxiakoky.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.chenzaomai.com/gtxhhilvov.html

[U24] Py：路径操作
来源：http://hz.meibo888.top/gtlutimewu.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yuanzhike.top/gtxoxsohod.html

[U25] Py：CSV 按字典读
来源：http://hz.jyoumei.cn/gtgomxkslu.html

csv.DictReader(f)
来源：http://hz.hysaishi.cn/gtjiemcguk.html

[U26] Py：并发下载
来源：http://hz.jinghuilouyu.cn/gtwcirdhns.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhengqikj.top/gtiopvzltc.html

[U27] Py：异步 HTTP
来源：http://hz.tian-w.cn/gtrujtnjnu.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ivvv.top/gtzxumfinh.html

[U28] Py：类型别名
来源：http://hz.tianlin.xyz/gtyfjglqvq.html

UserId = int
来源：http://hz.chenjidiqi.icu/gtogssqvch.html

[U29] Py：属性校验
来源：http://hz.chenjidiqi.icu/gtqjgggovq.html

@property 与 @x.setter 配合
来源：http://hz.xinyue.icu/gtzrlyktnn.html

[U30] Py：数据类
来源：http://hz.jinyuanbaomall.cn/gtkkftpnbg.html

@dataclass(slots=True)
来源：http://hz.chenjidiqi.icu/gtytxgnksr.html

[U31] Py：单测
来源：http://hz.yanxiufei.cn/gtfnuhugus.html

python -m pytest -q
来源：http://hz.yonumen.top/gtlermtafh.html

[U32] Py：代码格式化
来源：http://hz.ydjk.org.cn/gtpkndqtlr.html

ruff format . && ruff check --fix .
来源：http://hz.svipenyu.cn/gtolaipdft.html

[U33] Py：打包发布
来源：http://hz.yuanzhike.top/gtcmyzhvup.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.jqgufenzy.top/gtqbenzwrp.html

[U34] Py：判断编码
来源：http://hz.nanxuanxn.top/gtfbdinhrt.html

chardet.detect(raw)
来源：http://hz.chenlongwang.top/gttgvablwn.html

[U35] Py：发送邮件
来源：http://hz.hywenlv.cn/gtqsqbkhlf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.kuanghao11.cn/gtrjgdfhqj.html

[U36] Py：定时任务
来源：http://hz.yanxiufei.cn/gtpnviiefo.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhongyouzk.top/gttbibbcao.html

[U37] Py：读写 Excel
来源：http://hz.kuanghao11.cn/gtvkodeujk.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yj20258.top/gtrocmmoqk.html

[U38] Py：获取脚本所在目录
来源：http://hz.shanyushiyangtech.top/gtidwsumnn.html

Path(__file__).resolve().parent
来源：http://hz.jyoumei.cn/gtrmbqenzj.html

[U39] Py：判断是否在交互环境
来源：http://hz.fengsongda.top/gtyqvscwqz.html

sys.stdout.isatty()
来源：http://hz.svipenyu.cn/gtkpnckdsm.html

[U40] Py：打印到标准错误
来源：http://hz.redwolf501.top/gtjqjwfqqq.html

print("err", file=sys.stderr)
来源：http://hz.fengsongda.top/gtkdbfbibh.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cqqwz.cn/gtjxbyhshb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.chenlongwang.top/gtexcslzph.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.guowangkeji.top/gtmgqobmzg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.cashguo.top/gtdicurjla.html

[U43] PHP：声明命名空间
来源：http://hz.sxryk.cn/gtocbjfcob.html

namespace App\Http;
来源：http://hz.sufxvd.cn/gtrafldexg.html

[U44] PHP：开启严格类型
来源：http://hz.pycfn.com/gtermnzagv.html

declare(strict_types=1);
来源：http://hz.cdnleiting.top/gtudbusllv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.wangdashe.top/gtchxgeqxs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtqmmbgjhp.html

[U46] PHP：可空类型
来源：http://hz.zhongyouzk.top/gtyqnbxxfg.html

?string $name = null
来源：http://hz.jinyuanbaomall.cn/gtsikehloj.html

[U47] PHP：联合类型
来源：http://hz.52xcode.cn/gtrdoyzart.html

int|string $id
来源：http://hz.c1oappe.top/gtyhbsaygg.html

[U48] PHP：纯枚举
来源：http://hz.yuanzhike.top/gtoeyeqlsj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.chenzaomai.com/gtfingvaoh.html

[U49] PHP：只读属性
来源：http://hz.aizwys.cn/gtboaqxfjl.html

public readonly string $name
来源：http://hz.sysykeji.top/gtarkhmyhy.html

[U50] PHP：构造器属性提升
来源：http://hz.pengpengdd.cyou/gtydtxcpjf.html

public function __construct(private int $id) {}
来源：http://hz.svipenyu.cn/gtsnzkbnhh.html

[U51] PHP：数组解构
来源：http://hz.fengsongda.top/gtliqporrq.html

[$a, $b] = $arr;
来源：http://hz.fengsongda.top/gtckgefiln.html

[U52] PHP：箭头函数
来源：http://hz.yonumen.top/gtfpxbczdc.html

$double = fn($x) => $x * 2;
来源：http://hz.9152youxi.cn/gtlcukoilx.html

[U53] PHP：空合并运算符
来源：http://hz.9152youxi.cn/gtmpgjfqes.html

$v = $a ?? $b ?? "default";
来源：http://hz.ppjwa.cn/gtyiwlsznl.html

[U54] PHP：空安全调用
来源：http://hz.52xcode.cn/gtvyazujao.html

$obj?->method()
来源：http://hz.bjfxy.top/gtzanachvm.html

[U55] PHP：match 表达式
来源：http://hz.zhixingplan.top/gtynhevxqw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.chenjidiqi.icu/gteabfyaur.html

[U56] PHP：命名参数
来源：http://hz.sxryk.cn/gtydjldkvw.html

f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gtyzeyngtk.html

[U57] PHP：字符串插值
来源：http://hz.zhijiandao.cn/gtlrifpkfb.html

"值: {$a}"
来源：http://hz.xingfuxueyuan.xyz/gtnyzlxfll.html

[U58] PHP：数组三件套
来源：http://hz.guowangkeji.top/gtmndkmbjf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinghuilouyu.cn/gtmszrplpq.html

[U59] PHP：自定义排序
来源：http://hz.yonumen.top/gtnodypfpz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj202588.top/gtpzjvoxiq.html

[U60] PHP：JSON 编解码
来源：http://hz.daxiang520.top/gtbpemvvtc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.hysaishi.cn/gtmyxknoay.html

[U61] PHP：正则
来源：http://hz.aibaodan.cn/gtnggurvzk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtsdnkejpt.html

[U62] PHP：日期对象
来源：http://hz.chenzaomai.com/gtskhwpybu.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.0kj1m.cn/gttztauetl.html

[U63] PHP：文件读写
来源：http://hz.dashuyun.cn/gtffjvpfkh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.quarkkingdee.top/gtolaabvrz.html

[U64] PHP：目录遍历
来源：http://hz.zdqjudy.top/gtajdvmiah.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.snrcjt.cn/gthktfzaqg.html

[U65] PHP：会话
来源：http://hz.pengpengdd.cyou/gtpyxqkoyv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.dianchejie.cn/gtpzdiouhe.html

[U66] PHP：设置 Cookie
来源：http://hz.yj202588.top/gtgpchzejn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.fzhhl.top/gtjfdpcwoq.html

[U67] PHP：处理文件上传
来源：http://hz.zhengqikj.top/gtcgoobote.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.sysykeji.top/gttxnarejy.html

[U68] PHP：PDO 连接
来源：http://hz.yangfankeji.com/gtphsbhlcy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.sufxvd.cn/gtuiqbigai.html

[U69] PHP：PDO 预处理
来源：http://hz.wangdashe.top/gtgkzcvaqd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhoulong.xyz/gtfyuevrej.html

[U70] PHP：PDO 事务
来源：http://hz.yj20258.top/gtxqqjamte.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.zhixingplan.top/gttxnpuqkt.html

[U71] PHP：抛出异常
来源：http://hz.cqqwz.cn/gtufaqhvwn.html

throw new RuntimeException("失败", 500);
来源：http://hz.cdnleiting.top/gtospaxgvg.html

[U72] PHP：写错误日志
来源：http://hz.ydjk.org.cn/gtznnguirv.html

error_log("失败: " . $e->getMessage());
来源：http://hz.cucudq.cn/gtugbtvrzj.html


<!-- 参考信息 -->