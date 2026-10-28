代发 wailian999

int size() const noexcept { return n_; }
来源：http://hz.sweek.top/gtkmowfqqg.html

[S53] C++：移动语义
来源：http://hz.iojbl.cn/gttdzkdttb.html

std::vector<int> w = std::move(v);
来源：http://hz.zhongyouzk.top/gtflsnyagc.html

[S54] C++：异常处理
来源：http://hz.havefunace.top/gtpldjabta.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinqigufen.top/gtjjfxztsb.html

[S55] C++：结构化绑定
来源：http://hz.zycfv.cn/gtongtcvne.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sysykeji.top/gteveucyre.html

[S56] C++：optional
来源：http://hz.jinqigfzy.top/gtfmjrjkji.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sweek.top/gtmiclmlzo.html

[S57] C++：编译期常量
来源：http://hz.316326.xyz/gtdifkcost.html

constexpr int N = 10;
来源：http://hz.sxryk.cn/gtatkyhsad.html

[S58] C++：命名空间
来源：http://hz.shanyushiyangkeji.top/gtlfipqngc.html

namespace ns { int f() { return 1; } }
来源：http://hz.xingfuxueyuan.xyz/gtpqyeggvn.html

[S59] C++：静态断言
来源：http://hz.pengpengdd.cyou/gtpttvuwcu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hfpthk.cn/gtuodqrcvr.html

[S60] C++：遍历并删除元素
来源：http://hz.hysaishi.cn/gttdjuxoco.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangtech.top/gtvftuikom.html

================================================================================
来源：http://hz.nanxuanxn.top/gtumfiabkn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.vqdsnc.cn/gtnwjkxfxi.html

================================================================================
来源：http://hz.ivvv.top/gtiytaiwvt.html

[T01] Kotlin：Hello World
来源：http://hz.havefunace.top/gtodakyrno.html

println("Hello")
来源：http://hz.52xcode.cn/gtydumajij.html

[T02] Kotlin：变量
来源：http://hz.feifeiyinyue.top/gtlkktfnhj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gotoacloud.top/gtwufcvlkr.html

[T03] Kotlin：字符串模板
来源：http://hz.meibo888.top/gtuwcmwvqt.html

"值: $b"
来源：http://hz.tanke756.top/gtacesvhpy.html

[T04] Kotlin：空安全
来源：http://hz.yonumen.top/gtbgpzcqin.html

val n: String? = null;  n?.length
来源：http://hz.yj20258888.top/gtxqhcuckr.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangkeji.top/gtctqhakft.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hnxiangtu.top/gtdlpjtwjk.html

[T06] Kotlin：集合映射
来源：http://hz.daxiang520.top/gtwttzlelw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jiagoushi.top/gtiszknnel.html

[T07] Kotlin：集合过滤
来源：http://hz.zhengqikj.top/gtgvmwefcm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuxming.cn/gtlarqksma.html

[T08] Kotlin：数据类
来源：http://hz.havefunace.top/gtfiazvssj.html

data class User(val name: String, val age: Int)
来源：http://hz.hongshengwenyu.top/gtslvokcmo.html

[T09] Kotlin：扩展函数
来源：http://hz.chenzaomai.com/gtkjaksqzp.html

fun String.exclaim() = this + "!"
来源：http://hz.xuetiantiany.cn/gtgooowtlh.html

[T10] Kotlin：默认参数
来源：http://hz.c1oappe.top/gtngzrewmt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daxiang520.top/gtsghnzpoh.html

[T11] Kotlin：协程
来源：http://hz.aizwys.cn/gtdpgzodve.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ppjwa.cn/gttxdtllcw.html

[T12] Kotlin：解构声明
来源：http://hz.guannengcc.top/gthepgivph.html

val (a, b) = Pair(1, 2)
来源：http://hz.ppjwa.cn/gtzlsgkhtt.html

[T13] Kotlin：只读 Map
来源：http://hz.gotoacloud.top/gtuljrmpur.html

val m = mapOf("a" to 1)
来源：http://hz.xylfe.cn/gtzocaoepf.html

[T14] Kotlin：循环
来源：http://hz.zhijiandao.cn/gthvjsfoxw.html

for (i in 1..10) println(i)
来源：http://hz.hnqzz.top/gttynbuasf.html

[T15] Kotlin：接口
来源：http://hz.shuidangran.top/gtqbzakwat.html

interface Shape { fun area(): Double }
来源：http://hz.tianlin.xyz/gtjgiwryoo.html

[T16] Swift：Hello World
来源：http://hz.jinghuilouyu.cn/gtmaczbwzw.html

print("Hello")
来源：http://hz.chenzaomai.com/gtlvinvjng.html

[T17] Swift：变量与常量
来源：http://hz.zhongyouzk.top/gtmqbtqidt.html

var a = 1;  let b = 2
来源：http://hz.daria6918.cn/gtagsijxuy.html

[T18] Swift：字符串插值
来源：http://hz.aibaodan.cn/gthqsvdmwb.html

"值: \(b)"
来源：http://hz.hnxiangtu.top/gthukxtsdc.html

[T19] Swift：可选绑定
来源：http://hz.zhijiandao.cn/gtfgsyzdsf.html

if let n = opt { print(n) }
来源：http://hz.hywenlv.cn/gtgqmqioyk.html

[T20] Swift：数组操作
来源：http://hz.daxiang520.top/gtiuagxvar.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.smart0.xyz/gtzujainkr.html

[T21] Swift：遍历
来源：http://hz.jinqigufen.top/gtqttggrfr.html

for x in a { print(x) }
来源：http://hz.yj20258.top/gtbkrsgicn.html

[T22] Swift：字典
来源：http://hz.sysykeji.top/gtcfpjmubn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gaohongyu789.top/gtcpxfflbc.html

[T23] Swift：函数
来源：http://hz.aizwys.cn/gthhiiencz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.vqdsnc.cn/gtwrysymbu.html

[T24] Swift：闭包
来源：http://hz.jinyuanbaomall.cn/gtkmpqvdot.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ydzc1.top/gtpgvjmgdt.html

[T25] Swift：结构体
来源：http://hz.9152youxi.cn/gtcwazmwqn.html

struct P { var x: Int }
来源：http://hz.nanxinkj.top/gtfhhdpimd.html

[T26] Swift：类与重写
来源：http://hz.jqgfzy.top/gtplztnfck.html

class A: Base { override func f() {} }
来源：http://hz.iojbl.cn/gtsjykunad.html

[T27] Swift：错误处理
来源：http://hz.nanxinkj.top/gtmkmufdhz.html

do { try f() } catch { print(error) }
来源：http://hz.quarkkingdee.top/gtpbpqyqza.html

[T28] Swift：枚举
来源：http://hz.xuanzx.com/gthyooexhf.html

enum Color { case red, green }
来源：http://hz.chenzaomai.com/gtuqdhphrt.html

[T29] Swift：guard 提前返回
来源：http://hz.smart0.xyz/gtlfhizsgu.html

guard let x = opt else { return }
来源：http://hz.snrcjt.cn/gtsxpuabvu.html

[T30] Swift：协议
来源：http://hz.jinqigufen.top/gtpjymtahv.html

protocol Shape { func area() -> Double }
来源：http://hz.cqqwz.cn/gtkpeckiyt.html

[T31] Lua：Hello World
来源：http://hz.yj20258888.top/gtsdbrlzlx.html

print("Hello")
来源：http://hz.bjfxy.top/gtacfragja.html

[T32] Lua：局部变量
来源：http://hz.quarkkingdee.top/gtyvhmawsu.html

local a = 1
来源：http://hz.gaohongyu789.top/gtefcywcoc.html

[T33] Lua：表（数组）
来源：http://hz.aizwys.cn/gtlwtmeaqe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cqqwz.cn/gtcpjdocfv.html

[T34] Lua：遍历表
来源：http://hz.dashuyun.cn/gtkreimxsr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.guannengcc.top/gtfyecrpku.html

[T35] Lua：字典表
来源：http://hz.zhijiandao.cn/gtnlbxnelz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.hysaishi.cn/gtvlkhzkzh.html

[T36] Lua：函数
来源：http://hz.svipenyu.cn/gtyvcxxkwe.html

function add(a, b) return a + b end
来源：http://hz.mhx1999.top/gtdivjwukf.html

[T37] Lua：字符串拼接
来源：http://hz.xziqi.cn/gtofndefen.html

"a" .. "b"
来源：http://hz.yj20258888.top/gtlthkczks.html

[T38] Lua：条件
来源：http://hz.zhongyouzk.top/gtwjvmbqor.html

if x > 0 then print("正") end
来源：http://hz.jqgufenzy.top/gtjcaozhsk.html

[T39] Lua：模式匹配
来源：http://hz.sweek.top/gttjchuarg.html

string.find(s, "%d+")
来源：http://hz.snrcjt.cn/gtdiffpghw.html

[T40] Lua：元表
来源：http://hz.andypj.xyz/gtffnqjkid.html

setmetatable({}, { __index = base })
来源：http://hz.zhaomingkeji.xyz/gtybjcdlhc.html

[T41] Perl：Hello World
来源：http://hz.redwolf501.top/gtjywpkvnq.html

print "Hello\n";
来源：http://hz.shangyingyoupin.top/gtwcpuaedz.html

[T42] Perl：变量类型
来源：http://hz.jinqigfzy.top/gtbxvbtawr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jqgufenzy.top/gtwuhxbxih.html

[T43] Perl：字符串插值
来源：http://hz.zhongyouzk.top/gtenpssepb.html

"值: $a"
来源：http://hz.svipenyu.cn/gtinbjzmvr.html

[T44] Perl：条件
来源：http://hz.c1oappe.top/gtqmdmusov.html

if ($a > 0) { print "正"; }
来源：http://hz.ppjwa.cn/gtbfhybvvx.html

[T45] Perl：数组遍历
来源：http://hz.yanxiufei.cn/gtgomluqwn.html

for my $x (@arr) { print $x; }
来源：http://hz.xziqi.cn/gtdrwouiii.html

[T46] Perl：哈希操作
来源：http://hz.gzhubu.top/gtoudefqdd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj20258.top/gtqlllflhl.html

[T47] Perl：正则捕获
来源：http://hz.ehwqpu.com/gtibbvilcz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.jiagoushi.top/gtjxzdzuil.html

[T48] Perl：正则替换
来源：http://hz.c1oappe.top/gtslcrhlfv.html

$s =~ s/old/new/g;
来源：http://hz.sweek.top/gtnhpmgkzm.html

[T49] Perl：函数
来源：http://hz.hywenlv.cn/gtmsodbici.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gaohongyu789.top/gtuutsvknt.html

[T50] Perl：逐行读文件
来源：http://hz.zhijiandao.cn/gtwebqfjae.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.9152youxi.cn/gtmbhybmld.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gogol.net.cn/gtqffvtrrj.html

[T51] Scala：Hello World
来源：http://hz.andypj.xyz/gtqgebjabw.html

println("Hello")
来源：http://hz.ywan-chungtsiang.top/gtfgdkfedo.html

[T52] Scala：变量
来源：http://hz.guannengcc.top/gtdtogprkw.html

val a = 1;  var b = 2
来源：http://hz.mhx1999.top/gtcjopcjnz.html

[T53] Scala：字符串插值
来源：http://hz.hfpthk.cn/gtqesuzfge.html

s"值: $b"
来源：http://hz.hnqzz.top/gtflumrhbs.html

[T54] Scala：集合映射
来源：http://hz.mhx1999.top/gtghudxrus.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.zhijiandao.cn/gtqjpzfyee.html

[T55] Scala：集合过滤
来源：http://hz.aizwys.cn/gtiytefbwt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shanyushiyangtech.top/gthtsllgvm.html

[T56] Scala：样例类
来源：http://hz.zdqjudy.top/gthmichoev.html

case class User(name: String, age: Int)
来源：http://hz.zhoulong.xyz/gtcmfogahy.html

[T57] Scala：模式匹配
来源：http://hz.meibo888.top/gtptwudpug.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinqigufen.top/gtunsilhsi.html

[T58] Scala：函数定义
来源：http://hz.snrcjt.cn/gtqpqymdgq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jinqigfzy.top/gtjmetbjpz.html

[T59] Scala：循环
来源：http://hz.jinyuanbaomall.cn/gtksjaurmr.html

for (i <- 1 to 10) println(i)
来源：http://hz.yvedp.cn/gtpgmsagbb.html

[T60] Scala：折叠
来源：http://hz.wangshuangyany.cn/gtwmqhdqhc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jyoumei.cn/gtjxhdguiu.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gthfjrilsc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.gogol.net.cn/gtldkfapms.html

================================================================================
来源：http://hz.svipenyu.cn/gtaealklei.html

[U01] Py：创建虚拟环境
来源：http://hz.vqdsnc.cn/gtifafbnvz.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.aibaodan.cn/gttljbyryz.html

[U02] Py：导出 / 安装依赖
来源：http://hz.dianchejie.cn/gtqjvqkpfp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xylfe.cn/gtpiyqmbth.html

[U03] Py：加载 .env 配置
来源：http://hz.gotoacloud.top/gtivgazcfc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shanyushiyangtech.top/gtasanfhzn.html

[U04] Py：变量调试打印
来源：http://hz.9152youxi.cn/gtsnffauyh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.hysaishi.cn/gtsjxbcwku.html

[U05] Py：列表去重且保序
来源：http://hz.jinqigufen.top/gtezrxmvji.html

list(dict.fromkeys(arr))
来源：http://hz.vqdsnc.cn/gtdgtlzlhm.html

[U06] Py：合并两个字典
来源：http://hz.zdqjudy.top/gtpqlwgayq.html

{**a, **b}
来源：http://hz.chenzaomai.com/gtsoeaqqoo.html

[U07] Py：反转字典键值
来源：http://hz.svipenyu.cn/gtvayptfku.html

{v: k for k, v in d.items()}
来源：http://hz.wangshuangyany.cn/gthftpkskk.html

[U08] Py：展平二维列表
来源：http://hz.9152youxi.cn/gtnvnbdldo.html

[y for x in nested for y in x]
来源：http://hz.sweek.top/gtkynnfwhc.html

[U09] Py：字典取最大值的键
来源：http://hz.hywenlv.cn/gtpaxeodse.html

max(d, key=d.get)
来源：http://hz.cucudq.cn/gtikudqwiy.html

[U10] Py：按值排序字典
来源：http://hz.zhijiandao.cn/gtyfqtmdme.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.chenzaomai.com/gtybxvpwyn.html

[U11] Py：生成器表达式
来源：http://hz.shzxlz.cn/gtpjnihbgp.html

(x * 2 for x in arr)
来源：http://hz.zhengqikj.top/gtfnwqjxzc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.bjfxy.top/gtocfbxjpt.html

Counter(arr).most_common(3)
来源：http://hz.jinyuanbaomall.cn/gtlacysvxz.html

[U13] Py：固定长度队列
来源：http://hz.sufxvd.cn/gtvyimzhsy.html

deque(maxlen=10)
来源：http://hz.zhoulong.xyz/gtpabhvosb.html

[U14] Py：分组收集到列表
来源：http://hz.zdqjudy.top/gtrpjbwghx.html

defaultdict(list)
来源：http://hz.zhoulong.xyz/gtntpgpvjn.html

[U15] Py：高精度计时
来源：http://hz.redwolf501.top/gtzqmvmlpu.html

t = time.perf_counter()
来源：http://hz.nanxinkj.top/gtzuregwng.html

[U16] Py：命令行参数解析
来源：http://hz.hammf.cn/gtsmsffxrl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.guowangkeji.top/gtpywvzsgg.html

[U17] Py：初始化日志
来源：http://hz.birdmap.top/gttbpujtbc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.meibo888.top/gtivnicpkt.html

[U18] Py：预编译正则
来源：http://hz.0kj1m.cn/gtqajedouz.html

pat = re.compile(r"\d+")
来源：http://hz.yonumen.top/gtasrcbjpe.html

[U19] Py：正则替换带回调
来源：http://hz.jinyuanbaomall.cn/gtcxjlcnsy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.xylfe.cn/gtbchgniuf.html

[U20] Py：缓存函数结果
来源：http://hz.jinghuilouyu.cn/gttntgoagk.html

@functools.lru_cache(maxsize=None)
来源：http://hz.gzhubu.top/gtjczzsaxu.html

[U21] Py：自定义上下文管理器
来源：http://hz.zdqjudy.top/gttoubiomf.html

@contextlib.contextmanager
来源：http://hz.jlsjyb.cn/gtiggbuzse.html

[U22] Py：矩阵转置
来源：http://hz.hfpthk.cn/gtclcjeedm.html

list(zip(*m))
来源：http://hz.havefunace.top/gtwpkzwyon.html

[U23] Py：分块读取大文件
来源：http://hz.wangshuangyany.cn/gtjrkeysim.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.hammf.cn/gtypnkbijl.html

[U24] Py：路径操作
来源：http://hz.sufxvd.cn/gtughuefcd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.gogol.net.cn/gthpdnpedy.html

[U25] Py：CSV 按字典读
来源：http://hz.dianchejie.cn/gtjuiyvtwy.html

csv.DictReader(f)
来源：http://hz.zhongyouzk.top/gtbgcwygwb.html

[U26] Py：并发下载
来源：http://hz.nwbrower.top/gtfupnfdzc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.ydzc1.top/gtssethory.html

[U27] Py：异步 HTTP
来源：http://hz.shuidangran.top/gtbbyjybct.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.xylfe.cn/gtgznsytsv.html

[U28] Py：类型别名
来源：http://hz.shzxlz.cn/gtqppndfrm.html

UserId = int
来源：http://hz.jyoumei.cn/gtlbfphdlb.html

[U29] Py：属性校验
来源：http://hz.sysykeji.top/gtfxzpcpyj.html

@property 与 @x.setter 配合
来源：http://hz.gotoacloud.top/gtfxirhfum.html

[U30] Py：数据类
来源：http://hz.haohaochexian.top/gtdwrcwiup.html

@dataclass(slots=True)
来源：http://hz.zhixingplan.top/gtxepbfebo.html

[U31] Py：单测
来源：http://hz.cdnleiting.top/gtuosnnqqk.html

python -m pytest -q
来源：http://hz.yj20258.top/gtdtpadqbk.html

[U32] Py：代码格式化
来源：http://hz.guowangkeji.top/gtxwyozinq.html

ruff format . && ruff check --fix .
来源：http://hz.hfpthk.cn/gtelsdazhw.html

[U33] Py：打包发布
来源：http://hz.jqgufenzy.top/gtjraybikt.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.bjfxy.top/gtuclufxax.html

[U34] Py：判断编码
来源：http://hz.daria6918.cn/gtckmovxio.html

chardet.detect(raw)
来源：http://hz.aibaodan.cn/gtockupykl.html

[U35] Py：发送邮件
来源：http://hz.redwolf501.top/gtqarntxuf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.cqqwz.cn/gthbfibslz.html

[U36] Py：定时任务
来源：http://hz.9152youxi.cn/gtjwnauwic.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhongyouzk.top/gtaayygkbd.html

[U37] Py：读写 Excel
来源：http://hz.xylfe.cn/gtldjxbxyh.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.xylfe.cn/gtyjayzipk.html

[U38] Py：获取脚本所在目录
来源：http://hz.gaohongyu789.top/gtqhzmljks.html

Path(__file__).resolve().parent
来源：http://hz.xuanzx.com/gtujbwxhkm.html

[U39] Py：判断是否在交互环境
来源：http://hz.zhaomingkeji.xyz/gtadknyrlu.html

sys.stdout.isatty()
来源：http://hz.yuanzhike.top/gtgdfiqbmu.html

[U40] Py：打印到标准错误
来源：http://hz.ydzc1.top/gtxibffttt.html

print("err", file=sys.stderr)
来源：http://hz.sweek.top/gtdaxlttrx.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cucudq.cn/gtfemevwkm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.aizwys.cn/gtuwtzqutb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shzxlz.cn/gtzqjeqvlm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.sysykeji.top/gtonuvrbbr.html

[U43] PHP：声明命名空间
来源：http://hz.chenlongwang.top/gtwyxtuzgu.html

namespace App\Http;
来源：http://hz.nanxuanxn.top/gtoexrosjf.html

[U44] PHP：开启严格类型
来源：http://hz.guowangkeji.top/gtgryvgrbn.html

declare(strict_types=1);
来源：http://hz.c1oappe.top/gtwjurlvqv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.yuanzhike.top/gthjfkfqvw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtbcumuzjt.html

[U46] PHP：可空类型
来源：http://hz.guannengcc.top/gtyosqomzn.html

?string $name = null
来源：http://hz.gaohongyu789.top/gtvefsjwic.html

[U47] PHP：联合类型
来源：http://hz.chenjidiqi.icu/gtvdejgnzm.html

int|string $id
来源：http://hz.shanyushiyangkeji.top/gtdifbehxo.html

[U48] PHP：纯枚举
来源：http://hz.sufxvd.cn/gtflrzskao.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ydjk.org.cn/gthwqenomg.html

[U49] PHP：只读属性
来源：http://hz.jinghuilouyu.cn/gtedipppbo.html

public readonly string $name
来源：http://hz.aizwys.cn/gtttyeuluo.html

[U50] PHP：构造器属性提升
来源：http://hz.yj20258888.top/gtjhchhrwl.html

public function __construct(private int $id) {}
来源：http://hz.zycfv.cn/gtinqpvtna.html

[U51] PHP：数组解构
来源：http://hz.cqqwz.cn/gtnzyfpnxb.html

[$a, $b] = $arr;
来源：http://hz.andypj.xyz/gtwtvvbped.html

[U52] PHP：箭头函数
来源：http://hz.gotoacloud.top/gtgiqstixk.html

$double = fn($x) => $x * 2;
来源：http://hz.hfpthk.cn/gtydpmbmlf.html

[U53] PHP：空合并运算符
来源：http://hz.tianlin.xyz/gtgjdsnhwy.html

$v = $a ?? $b ?? "default";
来源：http://hz.havefunace.top/gtpmtswoeb.html

[U54] PHP：空安全调用
来源：http://hz.nanxinkj.top/gtsbuspemx.html

$obj?->method()
来源：http://hz.yonumen.top/gteskexzrt.html

[U55] PHP：match 表达式
来源：http://hz.hongshengwenyu.top/gtdxhcmzab.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.hysaishi.cn/gtnpzcpokc.html

[U56] PHP：命名参数
来源：http://hz.snrcjt.cn/gtkowesmav.html

f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtfivoocna.html

[U57] PHP：字符串插值
来源：http://hz.gzhubu.top/gtheujdwbo.html

"值: {$a}"
来源：http://hz.yueranfly.top/gtxgqlthnq.html

[U58] PHP：数组三件套
来源：http://hz.tianlin.xyz/gtmmlnwubr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jiagoushi.top/gtpizlzpwz.html

[U59] PHP：自定义排序
来源：http://hz.ehwqpu.com/gtsbfcetcz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hongshengwenyu.top/gtykjhhxaf.html

[U60] PHP：JSON 编解码
来源：http://hz.zhixingplan.top/gtxdobpxvb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.pycfn.com/gtvyhvnnsg.html

[U61] PHP：正则
来源：http://hz.havefunace.top/gtypdyndha.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hysaishi.cn/gttwlfhbhs.html

[U62] PHP：日期对象
来源：http://hz.yj20258.top/gtqyetwbuz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.c1oappe.top/gtrrynfdyo.html

[U63] PHP：文件读写
来源：http://hz.hnxiangtu.top/gtlzacdqzp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.shangyingyoupin.top/gteudxspmj.html

[U64] PHP：目录遍历
来源：http://hz.ywan-chungtsiang.top/gtzqkofyoa.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.tian-w.cn/gtlhlvfnyb.html

[U65] PHP：会话
来源：http://hz.ehwqpu.com/gtlxsoakxx.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.guowangkeji.top/gtexwjxyss.html

[U66] PHP：设置 Cookie
来源：http://hz.birdmap.top/gtfaxwqqxp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.ydzc1.top/gtqlhqitvw.html

[U67] PHP：处理文件上传
来源：http://hz.sxryk.cn/gtsergbwap.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.sysykeji.top/gtsixbiggm.html

[U68] PHP：PDO 连接
来源：http://hz.xuanzx.com/gtdrxkxbfx.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xingfuxueyuan.xyz/gtikymkmsa.html

[U69] PHP：PDO 预处理
来源：http://hz.redwolf501.top/gtzxzzslfh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gotoacloud.top/gtbdkxkipx.html

[U70] PHP：PDO 事务
来源：http://hz.zhongyouzk.top/gteuxqmazb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.daria6918.cn/gttcgvuhph.html

[U71] PHP：抛出异常
来源：http://hz.jqgufenzy.top/gtmyorqhiu.html

throw new RuntimeException("失败", 500);
来源：http://hz.hammf.cn/gtupvxwdlw.html

[U72] PHP：写错误日志
来源：http://hz.ydzc1.top/gtkpwbbtbl.html

error_log("失败: " . $e->getMessage());
来源：http://hz.snrcjt.cn/gtxxfordyk.html

[U73] PHP：读取 ini 配置
来源：http://hz.hysaishi.cn/gtmhdfeqyt.html

parse_ini_file("config.ini", true)
来源：http://hz.jinqigufen.top/gtzdyyorjp.html

[U74] PHP：读取环境变量
来源：http://hz.zhiwuduotai.top/gtxmzlrxyi.html

getenv("APP_ENV") ?: "production"
来源：http://hz.shanyushiyangtech.top/gtvccegtcq.html

[U75] PHP：依赖注入
来源：http://hz.zhengqikj.top/gtfkysluri.html

composer require psr/container
来源：http://hz.zhengqikj.top/gtaeibigll.html

[U76] PHP：简单路由
来源：http://hz.ppjwa.cn/gtghppbxvj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.tianlin.xyz/gthgwxsptq.html

[U77] PHP：模板渲染
来源：http://hz.yvedp.cn/gtpljcinhq.html

composer require twig/twig
来源：http://hz.c1oappe.top/gtepkshvzs.html

[U78] PHP：单元测试
来源：http://hz.xuanzx.com/gtykdrxktk.html

composer require --dev phpunit/phpunit
来源：http://hz.wangshuangyany.cn/gtswutwmhj.html


<!-- 参考信息 -->