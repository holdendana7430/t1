代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://hz.tianlin.xyz/gtqrgbplrw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenzaomai.com/gtbyvhztwg.html

[S48] C++：逐行读文件
来源：http://hz.daria6918.cn/gtwuppvlwa.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.nanxuanxn.top/gtvhedyfqp.html

while (std::getline(in, line)) { }
来源：http://hz.c1oappe.top/gtvphswltg.html

[S49] C++：写文件
来源：http://hz.gzhubu.top/gtbmkbapbb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnqzz.top/gtysusrapf.html

[S50] C++：格式化数字
来源：http://hz.nanxinkj.top/gtmsvpbmlz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sufxvd.cn/gtxhrmjnmr.html

[S51] C++：显式类型转换
来源：http://hz.guannengcc.top/gtwjgsynnt.html

static_cast<double>(a) / b
来源：http://hz.cucudq.cn/gttzcwfnwr.html

[S52] C++：const 与 noexcept
来源：http://hz.bjfxy.top/gtwnnsdgik.html

int size() const noexcept { return n_; }
来源：http://hz.gogol.net.cn/gthkdfmcpu.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gthuevlxcm.html

std::vector<int> w = std::move(v);
来源：http://hz.ydjk.org.cn/gtyxxrsdur.html

[S54] C++：异常处理
来源：http://hz.nanxinkj.top/gtxuuiytto.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangdashe.top/gtrzahgqee.html

[S55] C++：结构化绑定
来源：http://hz.haohaochexian.top/gtrrjgctwg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhaomingkeji.xyz/gtouqhtysq.html

[S56] C++：optional
来源：http://hz.yj20258.top/gthpuzxjvs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.52xcode.cn/gtnmhiknxy.html

[S57] C++：编译期常量
来源：http://hz.cucudq.cn/gtnbtqlwqc.html

constexpr int N = 10;
来源：http://hz.52xcode.cn/gtwticllio.html

[S58] C++：命名空间
来源：http://hz.jyoumei.cn/gtspdfvlnl.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinyuanbaomall.cn/gtiwgheopi.html

[S59] C++：静态断言
来源：http://hz.jinqigfzy.top/gtncpkmpvn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hnxiangtu.top/gtwrolxzox.html

[S60] C++：遍历并删除元素
来源：http://hz.daxiang520.top/gtdzbofmfn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hammf.cn/gtkbiojpeu.html

================================================================================
来源：http://hz.redwolf501.top/gtweijsnnv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenzaomai.com/gtgaorwiyf.html

================================================================================
来源：http://hz.nanxinkj.top/gtxbhnibbu.html

[T01] Kotlin：Hello World
来源：http://hz.sysykeji.top/gtpiindsjm.html

println("Hello")
来源：http://hz.nanxuanxn.top/gttnledcaz.html

[T02] Kotlin：变量
来源：http://hz.sufxvd.cn/gtklxiasyz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinyuanbaomall.cn/gtfryzdfkq.html

[T03] Kotlin：字符串模板
来源：http://hz.hysaishi.cn/gtixgtpldw.html

"值: $b"
来源：http://hz.zhixingplan.top/gtdosdrddv.html

[T04] Kotlin：空安全
来源：http://hz.dianchejie.cn/gtvaozhaup.html

val n: String? = null;  n?.length
来源：http://hz.tanke756.top/gtbeymvlfa.html

[T05] Kotlin：when 表达式
来源：http://hz.ybcxt.top/gtkkyyrqvv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhoulong.xyz/gtwoszdivo.html

[T06] Kotlin：集合映射
来源：http://hz.zhoulong.xyz/gtjtgkzrwt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jianghu66.top/gtfpzfjogr.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgfzy.top/gtixflhruh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.sysykeji.top/gtknytwyjv.html

[T08] Kotlin：数据类
来源：http://hz.mhx1999.top/gtkjarcnju.html

data class User(val name: String, val age: Int)
来源：http://hz.316326.xyz/gtccezvkto.html

[T09] Kotlin：扩展函数
来源：http://hz.jinghuilouyu.cn/gtqujvgnda.html

fun String.exclaim() = this + "!"
来源：http://hz.jinqigfzy.top/gtemakvgas.html

[T10] Kotlin：默认参数
来源：http://hz.haohaochexian.top/gtkvnrwlvc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.kuanghao11.cn/gtytsnsrwa.html

[T11] Kotlin：协程
来源：http://hz.hongshengwenyu.top/gttrgfvvzo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jyoumei.cn/gtbcclruse.html

[T12] Kotlin：解构声明
来源：http://hz.jqgfzy.top/gthbzueajo.html

val (a, b) = Pair(1, 2)
来源：http://hz.smart0.xyz/gtwssihcdn.html

[T13] Kotlin：只读 Map
来源：http://hz.zhijiandao.cn/gtpdrslklv.html

val m = mapOf("a" to 1)
来源：http://hz.yongpay.top/gtjyhkauuh.html

[T14] Kotlin：循环
来源：http://hz.yuanzhike.top/gtgjdpuyku.html

for (i in 1..10) println(i)
来源：http://hz.c1oappe.top/gtkjkwxmmk.html

[T15] Kotlin：接口
来源：http://hz.sysykeji.top/gtlddqhqsw.html

interface Shape { fun area(): Double }
来源：http://hz.meibo888.top/gttfbhzvaj.html

[T16] Swift：Hello World
来源：http://hz.daria6918.cn/gtegsjvugi.html

print("Hello")
来源：http://hz.cqqwz.cn/gtrwysypbx.html

[T17] Swift：变量与常量
来源：http://hz.xylfe.cn/gtdeojhenv.html

var a = 1;  let b = 2
来源：http://hz.quarkkingdee.top/gtjxnyxyss.html

[T18] Swift：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtawltgmos.html

"值: \(b)"
来源：http://hz.wangdashe.top/gtacaoxmgf.html

[T19] Swift：可选绑定
来源：http://hz.wangdashe.top/gtqrippuzh.html

if let n = opt { print(n) }
来源：http://hz.bjfxy.top/gtfjdgogvp.html

[T20] Swift：数组操作
来源：http://hz.jinqigfzy.top/gthypyfykd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sufxvd.cn/gttclambaz.html

[T21] Swift：遍历
来源：http://hz.zhaomingkeji.xyz/gthlupbliq.html

for x in a { print(x) }
来源：http://hz.xuanzx.com/gtdogvslkn.html

[T22] Swift：字典
来源：http://hz.haohaochexian.top/gtxaoyxyng.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sysykeji.top/gtpyxfhkpr.html

[T23] Swift：函数
来源：http://hz.yueranfly.top/gttdtmgtbf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sufxvd.cn/gtquwsogjd.html

[T24] Swift：闭包
来源：http://hz.quarkkingdee.top/gtifrprllg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj20258.top/gtukoibftp.html

[T25] Swift：结构体
来源：http://hz.hnqzz.top/gtfeyydsyh.html

struct P { var x: Int }
来源：http://hz.yuanzhike.top/gtvuidygvr.html

[T26] Swift：类与重写
来源：http://hz.yonumen.top/gtjionedfm.html

class A: Base { override func f() {} }
来源：http://hz.zhiwuduotai.top/gtlxxjauab.html

[T27] Swift：错误处理
来源：http://hz.xuanzx.com/gtqjheizof.html

do { try f() } catch { print(error) }
来源：http://hz.daria6918.cn/gtqiecjfoa.html

[T28] Swift：枚举
来源：http://hz.jyoumei.cn/gtkwlswyca.html

enum Color { case red, green }
来源：http://hz.smart0.xyz/gtqyrnajpp.html

[T29] Swift：guard 提前返回
来源：http://hz.zhengqikj.top/gtzpbytzef.html

guard let x = opt else { return }
来源：http://hz.pengpengdd.cyou/gtwjjxhect.html

[T30] Swift：协议
来源：http://hz.jiagoushi.top/gtbcdwcgqn.html

protocol Shape { func area() -> Double }
来源：http://hz.yangfankeji.com/gtebmfuphp.html

[T31] Lua：Hello World
来源：http://hz.dianchejie.cn/gtumlwnwmc.html

print("Hello")
来源：http://hz.yj20258.top/gtgxsojnlh.html

[T32] Lua：局部变量
来源：http://hz.zhoulong.xyz/gtplrigcwt.html

local a = 1
来源：http://hz.chenzaomai.com/gtpczqaelb.html

[T33] Lua：表（数组）
来源：http://hz.yanxiufei.cn/gtbcmnuwkl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhixingplan.top/gtpdjrggfy.html

[T34] Lua：遍历表
来源：http://hz.haohaochexian.top/gtdxfvzffq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cucudq.cn/gtidmzjewi.html

[T35] Lua：字典表
来源：http://hz.shuidangran.top/gtdafjtnnr.html

local d = { a = 1 };  d.b = 2
来源：http://hz.tanke756.top/gtejjufrmn.html

[T36] Lua：函数
来源：http://hz.snrcjt.cn/gtwsgnwqpm.html

function add(a, b) return a + b end
来源：http://hz.xingfuxueyuan.xyz/gtfytwwqkw.html

[T37] Lua：字符串拼接
来源：http://hz.gogol.net.cn/gtwnfiakhz.html

"a" .. "b"
来源：http://hz.sxryk.cn/gtxdhihujy.html

[T38] Lua：条件
来源：http://hz.ydzc1.top/gticwfkzsf.html

if x > 0 then print("正") end
来源：http://hz.cheryme.top/gtertpfold.html

[T39] Lua：模式匹配
来源：http://hz.aibaodan.cn/gtxekqkptf.html

string.find(s, "%d+")
来源：http://hz.yj202588.top/gtlernwugf.html

[T40] Lua：元表
来源：http://hz.havefunace.top/gtdjrggbrj.html

setmetatable({}, { __index = base })
来源：http://hz.yueranfly.top/gthjvibipx.html

[T41] Perl：Hello World
来源：http://hz.ydjk.org.cn/gtgoqntcdk.html

print "Hello\n";
来源：http://hz.guowangkeji.top/gtgiscnnwi.html

[T42] Perl：变量类型
来源：http://hz.zhijiandao.cn/gtacaqejkd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xuanzx.com/gtpbfdlsui.html

[T43] Perl：字符串插值
来源：http://hz.yj20258.top/gtrvubnssf.html

"值: $a"
来源：http://hz.shuidangran.top/gtnkqjgugi.html

[T44] Perl：条件
来源：http://hz.ywan-chungtsiang.top/gtdihdxzkg.html

if ($a > 0) { print "正"; }
来源：http://hz.zhengqikj.top/gtqthuugls.html

[T45] Perl：数组遍历
来源：http://hz.feifeiyinyue.top/gtfkgxngbq.html

for my $x (@arr) { print $x; }
来源：http://hz.shuidangran.top/gtnopyrkta.html

[T46] Perl：哈希操作
来源：http://hz.chenlongwang.top/gtehyyqiua.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.chenjidiqi.icu/gtgenesgrm.html

[T47] Perl：正则捕获
来源：http://hz.jiagoushi.top/gtueomwrcn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangtech.top/gtxxxqmfao.html

[T48] Perl：正则替换
来源：http://hz.jlsjyb.cn/gtstqkkhjn.html

$s =~ s/old/new/g;
来源：http://hz.shanyushiyangkeji.top/gtnoqbcxks.html

[T49] Perl：函数
来源：http://hz.shuidangran.top/gtizwltvgz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hfpthk.cn/gttiiqzwun.html

[T50] Perl：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtwwifttrz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.fengsongda.top/gttiscdszo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cdnleiting.top/gtblkjuxty.html

[T51] Scala：Hello World
来源：http://hz.dashuyun.cn/gtkmilgdye.html

println("Hello")
来源：http://hz.pengpengdd.cyou/gtffctehba.html

[T52] Scala：变量
来源：http://hz.snrcjt.cn/gtixmrdtph.html

val a = 1;  var b = 2
来源：http://hz.jqgufenzy.top/gtuntsutcu.html

[T53] Scala：字符串插值
来源：http://hz.gaohongyu789.top/gtksrtksxi.html

s"值: $b"
来源：http://hz.sxryk.cn/gtlnamvtky.html

[T54] Scala：集合映射
来源：http://hz.jlsjyb.cn/gtilxsntll.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.9152youxi.cn/gtcjimsjtn.html

[T55] Scala：集合过滤
来源：http://hz.smart0.xyz/gtgtxgmfid.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinqigfzy.top/gtqvofsapn.html

[T56] Scala：样例类
来源：http://hz.sysykeji.top/gtqxyubbkt.html

case class User(name: String, age: Int)
来源：http://hz.shangyingyoupin.top/gtzpkaeepi.html

[T57] Scala：模式匹配
来源：http://hz.dashuyun.cn/gtiwgpzdkr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhixingplan.top/gttadwynzj.html

[T58] Scala：函数定义
来源：http://hz.tian-w.cn/gtejsdkgqg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.sysykeji.top/gtnylizwov.html

[T59] Scala：循环
来源：http://hz.cucudq.cn/gtrktspobt.html

for (i <- 1 to 10) println(i)
来源：http://hz.xingfuxueyuan.xyz/gtompjecij.html

[T60] Scala：折叠
来源：http://hz.zhoulong.xyz/gtdgwqwhoq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.nwbrower.top/gtfrmxvvjj.html

================================================================================
来源：http://hz.cashguo.top/gtnhjvkvto.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gaohongyu789.top/gtufnsvjhb.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtnadvncse.html

[U01] Py：创建虚拟环境
来源：http://hz.gotoacloud.top/gtwwdjsqfn.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhixingplan.top/gtpstwbjze.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ehwqpu.com/gtnpwndhbd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.52xcode.cn/gtccptmgjk.html

[U03] Py：加载 .env 配置
来源：http://hz.mhx1999.top/gtdtjyrsmm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jqgfzy.top/gtwnouclgp.html

[U04] Py：变量调试打印
来源：http://hz.jinqigufen.top/gtvjzzeltv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.cheryme.top/gtqzmewyol.html

[U05] Py：列表去重且保序
来源：http://hz.zhiwuduotai.top/gtomvhbnjp.html

list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gthdaqtreq.html

[U06] Py：合并两个字典
来源：http://hz.gogol.net.cn/gtpisjzqjj.html

{**a, **b}
来源：http://hz.zhongyouzk.top/gteynxnnhy.html

[U07] Py：反转字典键值
来源：http://hz.sufxvd.cn/gtijmgcmjt.html

{v: k for k, v in d.items()}
来源：http://hz.yvedp.cn/gtvvpkzusp.html

[U08] Py：展平二维列表
来源：http://hz.redwolf501.top/gtubfsetbj.html

[y for x in nested for y in x]
来源：http://hz.havefunace.top/gtvjephwkb.html

[U09] Py：字典取最大值的键
来源：http://hz.redwolf501.top/gtbpiswwdb.html

max(d, key=d.get)
来源：http://hz.wangshuangyany.cn/gtqssxqciy.html

[U10] Py：按值排序字典
来源：http://hz.xuetiantiany.cn/gtczzrmqrq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.cashguo.top/gtntdofcgw.html

[U11] Py：生成器表达式
来源：http://hz.chenlongwang.top/gtrkakusfq.html

(x * 2 for x in arr)
来源：http://hz.xuetiantiany.cn/gtuienrqxa.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.mhx1999.top/gtpvaqfrdm.html

Counter(arr).most_common(3)
来源：http://hz.jlsjyb.cn/gtuwfngemf.html

[U13] Py：固定长度队列
来源：http://hz.feifeiyinyue.top/gtwugazcxu.html

deque(maxlen=10)
来源：http://hz.zhaomingkeji.xyz/gtpialfulq.html

[U14] Py：分组收集到列表
来源：http://hz.zhiwuduotai.top/gtrwzdubkw.html

defaultdict(list)
来源：http://hz.mhx1999.top/gtbphcesaq.html

[U15] Py：高精度计时
来源：http://hz.shangyingyoupin.top/gtephcdbos.html

t = time.perf_counter()
来源：http://hz.0kj1m.cn/gtwfpprvpx.html

[U16] Py：命令行参数解析
来源：http://hz.zhongyouzk.top/gtcljewgjt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zhijiandao.cn/gtcecsygai.html

[U17] Py：初始化日志
来源：http://hz.kuanghao11.cn/gtoefzmeja.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.jlsjyb.cn/gtveczcqpy.html

[U18] Py：预编译正则
来源：http://hz.zhixingplan.top/gtxypgtjul.html

pat = re.compile(r"\d+")
来源：http://hz.iojbl.cn/gtwvbxbppq.html

[U19] Py：正则替换带回调
来源：http://hz.cheryme.top/gteyojjkce.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yangfankeji.com/gttnofsjjh.html

[U20] Py：缓存函数结果
来源：http://hz.cashguo.top/gtfgcjsazh.html

@functools.lru_cache(maxsize=None)
来源：http://hz.yvedp.cn/gtdcaxugvn.html

[U21] Py：自定义上下文管理器
来源：http://hz.cheryme.top/gtfjnnsdgn.html

@contextlib.contextmanager
来源：http://hz.sxryk.cn/gtffsixurb.html

[U22] Py：矩阵转置
来源：http://hz.yuxming.cn/gtarxytgpl.html

list(zip(*m))
来源：http://hz.zhiwuduotai.top/gteumquexs.html

[U23] Py：分块读取大文件
来源：http://hz.xingfuxueyuan.xyz/gtelfmhcth.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.xinyue.icu/gtvxualknb.html

[U24] Py：路径操作
来源：http://hz.ybcxt.top/gtcbzlejsr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yonumen.top/gtyzlglwcs.html

[U25] Py：CSV 按字典读
来源：http://hz.havefunace.top/gtvpawrcjb.html

csv.DictReader(f)
来源：http://hz.yuanzhike.top/gtqbllehjn.html

[U26] Py：并发下载
来源：http://hz.yonumen.top/gtlsjbywkh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.316326.xyz/gtbqtcbckt.html

[U27] Py：异步 HTTP
来源：http://hz.zhongyouzk.top/gtowxhyyfg.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.smart0.xyz/gttwnxtdjl.html

[U28] Py：类型别名
来源：http://hz.sufxvd.cn/gtwayglcho.html

UserId = int
来源：http://hz.pycfn.com/gtnpjodlzb.html

[U29] Py：属性校验
来源：http://hz.sufxvd.cn/gtvopsuxtk.html

@property 与 @x.setter 配合
来源：http://hz.jinqigufen.top/gtmdpxpmcj.html

[U30] Py：数据类
来源：http://hz.wangshuangyany.cn/gtuxduydqg.html

@dataclass(slots=True)
来源：http://hz.cheryme.top/gtesmirhyb.html

[U31] Py：单测
来源：http://hz.fzhhl.top/gtgqrvnkhj.html

python -m pytest -q
来源：http://hz.birdmap.top/gttcgauhzl.html

[U32] Py：代码格式化
来源：http://hz.sysykeji.top/gtexbpdzee.html

ruff format . && ruff check --fix .
来源：http://hz.jianghu66.top/gtacevljoq.html

[U33] Py：打包发布
来源：http://hz.cheryme.top/gtingycnge.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.zhoulong.xyz/gtnqucgdac.html

[U34] Py：判断编码
来源：http://hz.sxryk.cn/gtkcolqbcp.html

chardet.detect(raw)
来源：http://hz.ppjwa.cn/gtfrnovogz.html

[U35] Py：发送邮件
来源：http://hz.guannengcc.top/gthrezbpni.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.shanyushiyangkeji.top/gtfaloetwo.html

[U36] Py：定时任务
来源：http://hz.dianchejie.cn/gthdchafkr.html

schedule.every(10).minutes.do(job)
来源：http://hz.gaohongyu789.top/gtdkfmwbmi.html

[U37] Py：读写 Excel
来源：http://hz.c1oappe.top/gtkrpnrzko.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhixingplan.top/gtuoaazxhd.html

[U38] Py：获取脚本所在目录
来源：http://hz.xuetiantiany.cn/gtfurdxyxy.html

Path(__file__).resolve().parent
来源：http://hz.haohaochexian.top/gtkhwllpuj.html

[U39] Py：判断是否在交互环境
来源：http://hz.redwolf501.top/gtlhrdiemh.html

sys.stdout.isatty()
来源：http://hz.vqdsnc.cn/gtolkgymjf.html

[U40] Py：打印到标准错误
来源：http://hz.zdqjudy.top/gtlowhghcc.html

print("err", file=sys.stderr)
来源：http://hz.nanxuanxn.top/gtifndawwf.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.fzhhl.top/gtrwlxthwv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jiagoushi.top/gtmghpisdo.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.yongpay.top/gtkdhtkbhg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.gogol.net.cn/gtfaduukaa.html

[U43] PHP：声明命名空间
来源：http://hz.zhongyouzk.top/gtyvysytxc.html

namespace App\Http;
来源：http://hz.yj202588.top/gtsqfabmrv.html

[U44] PHP：开启严格类型
来源：http://hz.dianchejie.cn/gtgyhvmkuc.html

declare(strict_types=1);
来源：http://hz.pycfn.com/gtfjzrvhba.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nanxuanxn.top/gtfgrdeiaf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhixingplan.top/gtghwlpyim.html

[U46] PHP：可空类型
来源：http://hz.zycfv.cn/gtepjzrlaw.html

?string $name = null
来源：http://hz.yueranfly.top/gtrcngbilo.html

[U47] PHP：联合类型
来源：http://hz.meibo888.top/gtifuzwpku.html

int|string $id
来源：http://hz.kuanghao11.cn/gtnpbccrko.html

[U48] PHP：纯枚举
来源：http://hz.kuanghao11.cn/gtxcdvavln.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ehwqpu.com/gtyxoogtbt.html

[U49] PHP：只读属性
来源：http://hz.tianlin.xyz/gtenhggdqo.html

public readonly string $name
来源：http://hz.xuanzx.com/gthyvoqalb.html

[U50] PHP：构造器属性提升
来源：http://hz.9152youxi.cn/gtosttwudg.html

public function __construct(private int $id) {}
来源：http://hz.zhaomingkeji.xyz/gtkaighvcs.html

[U51] PHP：数组解构
来源：http://hz.redwolf501.top/gtizgyxjdk.html

[$a, $b] = $arr;
来源：http://hz.yj20258888.top/gtbojhaape.html

[U52] PHP：箭头函数
来源：http://hz.fengsongda.top/gtibctgbhq.html

$double = fn($x) => $x * 2;
来源：http://hz.sweek.top/gteemzpcdm.html

[U53] PHP：空合并运算符
来源：http://hz.hongshengwenyu.top/gtmtdkhlhy.html

$v = $a ?? $b ?? "default";
来源：http://hz.ydzc1.top/gtwkejlgxl.html

[U54] PHP：空安全调用
来源：http://hz.0kj1m.cn/gtzvylanuz.html

$obj?->method()
来源：http://hz.zhongyouzk.top/gtpseyoyfl.html

[U55] PHP：match 表达式
来源：http://hz.daxiang520.top/gttgagfcmr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ydzc1.top/gtmmlvvqvc.html

[U56] PHP：命名参数
来源：http://hz.jianghu66.top/gtsfqqowrc.html

f(a: 1, b: 2)
来源：http://hz.xingfuxueyuan.xyz/gtrxxpnkbw.html

[U57] PHP：字符串插值
来源：http://hz.ybcxt.top/gtrlusirfw.html

"值: {$a}"
来源：http://hz.shanyushiyangkeji.top/gtwmotxsgh.html

[U58] PHP：数组三件套
来源：http://hz.jinqigfzy.top/gttxpunqug.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yueranfly.top/gtpcwjxmkc.html

[U59] PHP：自定义排序
来源：http://hz.hywenlv.cn/gttuxvqnhw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xingfuxueyuan.xyz/gtmvcdlfxj.html

[U60] PHP：JSON 编解码
来源：http://hz.wangshuangyany.cn/gtlqahvtee.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.pycfn.com/gtkjhywlmq.html

[U61] PHP：正则
来源：http://hz.yanxiufei.cn/gtqlhbbisv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuetiantiany.cn/gtprhmveyh.html

[U62] PHP：日期对象
来源：http://hz.nanxinkj.top/gtuktmrnzb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jianghu66.top/gtbrjhrzcy.html

[U63] PHP：文件读写
来源：http://hz.shanyushiyangtech.top/gthxjotqrv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.xuanzx.com/gtnxzqlkdx.html

[U64] PHP：目录遍历
来源：http://hz.daxiang520.top/gtzeurylvk.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.havefunace.top/gtqghkwoso.html

[U65] PHP：会话
来源：http://hz.kuanghao11.cn/gtmpuryqfm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yvedp.cn/gtdazmgvji.html

[U66] PHP：设置 Cookie
来源：http://hz.hnqzz.top/gtustvefnm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.daria6918.cn/gtopsyxwdj.html

[U67] PHP：处理文件上传
来源：http://hz.nanxinkj.top/gtrkgizmae.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.shanyushiyangtech.top/gtpwnpugwt.html

[U68] PHP：PDO 连接
来源：http://hz.aibaodan.cn/gtgiyhejxe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.bjfxy.top/gtrqvbgbrb.html

[U69] PHP：PDO 预处理
来源：http://hz.chenlongwang.top/gtkksdwjlw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.mhx1999.top/gtffmavevk.html

[U70] PHP：PDO 事务
来源：http://hz.ywan-chungtsiang.top/gtvuqzzbbq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.nwbrower.top/gtdlichrpt.html

[U71] PHP：抛出异常
来源：http://hz.yj202588.top/gtyxgvsfil.html

throw new RuntimeException("失败", 500);
来源：http://hz.guannengcc.top/gtecfgyhqj.html

[U72] PHP：写错误日志
来源：http://hz.zhixingplan.top/gtryamkgvx.html

error_log("失败: " . $e->getMessage());
来源：http://hz.feifeiyinyue.top/gtbuaajhdm.html


<!-- 参考信息 -->