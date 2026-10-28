代发 wailian999

int size() const noexcept { return n_; }
来源：http://hz.yuxming.cn/gtdoujyhlr.html

[S53] C++：移动语义
来源：http://hz.hongshengwenyu.top/gtbqgbdham.html

std::vector<int> w = std::move(v);
来源：http://hz.snrcjt.cn/gtqaiglvea.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gttslrtgea.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sweek.top/gtnbsxckai.html

[S55] C++：结构化绑定
来源：http://hz.cashguo.top/gtnvpmuhwe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhaomingkeji.xyz/gtuddizwjk.html

[S56] C++：optional
来源：http://hz.svipenyu.cn/gtnbbdscbi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nwbrower.top/gtspfzikgb.html

[S57] C++：编译期常量
来源：http://hz.zycfv.cn/gtaxxyyerh.html

constexpr int N = 10;
来源：http://hz.tian-w.cn/gtbkqanawe.html

[S58] C++：命名空间
来源：http://hz.iojbl.cn/gtxdbmrxcw.html

namespace ns { int f() { return 1; } }
来源：http://hz.yanxiufei.cn/gtdfnqwkys.html

[S59] C++：静态断言
来源：http://hz.xziqi.cn/gtkjahdbom.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgufenzy.top/gtzmwrgydg.html

[S60] C++：遍历并删除元素
来源：http://hz.kuanghao11.cn/gtgdtlfart.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gaohongyu789.top/gtcvzgdsrl.html

================================================================================
来源：http://hz.ppjwa.cn/gthvlnnfxd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ivvv.top/gtowryxyar.html

================================================================================
来源：http://hz.andypj.xyz/gtmpqcgrqp.html

[T01] Kotlin：Hello World
来源：http://hz.c1oappe.top/gtepfwjljf.html

println("Hello")
来源：http://hz.cdnleiting.top/gthqamchhe.html

[T02] Kotlin：变量
来源：http://hz.sysykeji.top/gtjtdaxezq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xingfuxueyuan.xyz/gtvpcnkklx.html

[T03] Kotlin：字符串模板
来源：http://hz.yvedp.cn/gtkblqeaot.html

"值: $b"
来源：http://hz.hysaishi.cn/gtrfshlbaz.html

[T04] Kotlin：空安全
来源：http://hz.aibaodan.cn/gttektfyzz.html

val n: String? = null;  n?.length
来源：http://hz.svipenyu.cn/gttcgdtbzg.html

[T05] Kotlin：when 表达式
来源：http://hz.smart0.xyz/gtfdlvsnpd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.snrcjt.cn/gtlwbthjfy.html

[T06] Kotlin：集合映射
来源：http://hz.jianghu66.top/gtaboecsgf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yanxiufei.cn/gtziwtzfks.html

[T07] Kotlin：集合过滤
来源：http://hz.mhx1999.top/gtwmxotvek.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xinyue.icu/gtapfhfwti.html

[T08] Kotlin：数据类
来源：http://hz.ydzc1.top/gtyfjwrdkq.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgfzy.top/gthidpytjj.html

[T09] Kotlin：扩展函数
来源：http://hz.zhaomingkeji.xyz/gtnmrnjgqc.html

fun String.exclaim() = this + "!"
来源：http://hz.316326.xyz/gtcwyvtaiq.html

[T10] Kotlin：默认参数
来源：http://hz.yvedp.cn/gttllwjoro.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ppjwa.cn/gtnvnawvlb.html

[T11] Kotlin：协程
来源：http://hz.chenzaomai.com/gtfduzkvwy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnxiangtu.top/gtgxhauiwg.html

[T12] Kotlin：解构声明
来源：http://hz.shanyushiyangkeji.top/gtlvfxfthx.html

val (a, b) = Pair(1, 2)
来源：http://hz.tian-w.cn/gtotjwhcqf.html

[T13] Kotlin：只读 Map
来源：http://hz.ydjk.org.cn/gtzxiodxvm.html

val m = mapOf("a" to 1)
来源：http://hz.iojbl.cn/gtnosdhfrb.html

[T14] Kotlin：循环
来源：http://hz.yonumen.top/gtpiiybcoo.html

for (i in 1..10) println(i)
来源：http://hz.cdnleiting.top/gtludracai.html

[T15] Kotlin：接口
来源：http://hz.gotoacloud.top/gtkczggcof.html

interface Shape { fun area(): Double }
来源：http://hz.quarkkingdee.top/gtlzrttule.html

[T16] Swift：Hello World
来源：http://hz.vqdsnc.cn/gtqkmmwiwc.html

print("Hello")
来源：http://hz.redwolf501.top/gtrbyauyug.html

[T17] Swift：变量与常量
来源：http://hz.snrcjt.cn/gtlnsvimee.html

var a = 1;  let b = 2
来源：http://hz.dianchejie.cn/gtftcuabom.html

[T18] Swift：字符串插值
来源：http://hz.jinghuilouyu.cn/gturmlnzeu.html

"值: \(b)"
来源：http://hz.havefunace.top/gtjffjiwso.html

[T19] Swift：可选绑定
来源：http://hz.chenlongwang.top/gtcaybosbi.html

if let n = opt { print(n) }
来源：http://hz.jqgufenzy.top/gttepdxxdw.html

[T20] Swift：数组操作
来源：http://hz.jinqigufen.top/gtzeealthx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.chenlongwang.top/gtytxvueqy.html

[T21] Swift：遍历
来源：http://hz.ywan-chungtsiang.top/gtrktkjtmc.html

for x in a { print(x) }
来源：http://hz.sweek.top/gthactubhy.html

[T22] Swift：字典
来源：http://hz.svipenyu.cn/gttvtrrajy.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.fzhhl.top/gtbfdqawlc.html

[T23] Swift：函数
来源：http://hz.gogol.net.cn/gtlfudinil.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shuidangran.top/gtxkzhpwgb.html

[T24] Swift：闭包
来源：http://hz.ivvv.top/gtplcccryo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.pycfn.com/gtlqoqupcz.html

[T25] Swift：结构体
来源：http://hz.birdmap.top/gteyynwbkn.html

struct P { var x: Int }
来源：http://hz.meibo888.top/gtvtprudug.html

[T26] Swift：类与重写
来源：http://hz.yj202588.top/gtnwvswxlj.html

class A: Base { override func f() {} }
来源：http://hz.jinqigufen.top/gtzyhnozlu.html

[T27] Swift：错误处理
来源：http://hz.zhiwuduotai.top/gtzwoqcmfz.html

do { try f() } catch { print(error) }
来源：http://hz.yanxiufei.cn/gthhurwylg.html

[T28] Swift：枚举
来源：http://hz.gotoacloud.top/gtsstdfkok.html

enum Color { case red, green }
来源：http://hz.meibo888.top/gtwnscmnxm.html

[T29] Swift：guard 提前返回
来源：http://hz.jinqigfzy.top/gtfppnnpgb.html

guard let x = opt else { return }
来源：http://hz.jiagoushi.top/gtdtbflcei.html

[T30] Swift：协议
来源：http://hz.cucudq.cn/gthckrpbol.html

protocol Shape { func area() -> Double }
来源：http://hz.jqgfzy.top/gtfxrwyjvn.html

[T31] Lua：Hello World
来源：http://hz.xinyue.icu/gtvteesrkj.html

print("Hello")
来源：http://hz.ehwqpu.com/gtwhsllokr.html

[T32] Lua：局部变量
来源：http://hz.jqgfzy.top/gtvpqxhqwe.html

local a = 1
来源：http://hz.aibaodan.cn/gtbgrbfslk.html

[T33] Lua：表（数组）
来源：http://hz.dashuyun.cn/gtemfguwfe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.chenlongwang.top/gtwcgdecnt.html

[T34] Lua：遍历表
来源：http://hz.chenjidiqi.icu/gtxawkcfsl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ivvv.top/gtpbxwijgf.html

[T35] Lua：字典表
来源：http://hz.jqgfzy.top/gtmuyvthrs.html

local d = { a = 1 };  d.b = 2
来源：http://hz.tianlin.xyz/gtvxyvulaa.html

[T36] Lua：函数
来源：http://hz.yvedp.cn/gtbdyhxjfo.html

function add(a, b) return a + b end
来源：http://hz.bjfxy.top/gtsllfydxk.html

[T37] Lua：字符串拼接
来源：http://hz.0kj1m.cn/gtjfiqcmnd.html

"a" .. "b"
来源：http://hz.ydzc1.top/gtqjilxebb.html

[T38] Lua：条件
来源：http://hz.zhiwuduotai.top/gtqosjrypz.html

if x > 0 then print("正") end
来源：http://hz.gzhubu.top/gtixjghgfn.html

[T39] Lua：模式匹配
来源：http://hz.zycfv.cn/gtwuemckcx.html

string.find(s, "%d+")
来源：http://hz.chenzaomai.com/gtvsrqfteh.html

[T40] Lua：元表
来源：http://hz.tanke756.top/gthvyeybdv.html

setmetatable({}, { __index = base })
来源：http://hz.yuanzhike.top/gtnsjvxehe.html

[T41] Perl：Hello World
来源：http://hz.vqdsnc.cn/gthcgqqwxe.html

print "Hello\n";
来源：http://hz.xuetiantiany.cn/gtawfnejlo.html

[T42] Perl：变量类型
来源：http://hz.hfpthk.cn/gtfowocvtd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sxryk.cn/gtzoieimbl.html

[T43] Perl：字符串插值
来源：http://hz.yuanzhike.top/gtngprtvkg.html

"值: $a"
来源：http://hz.jinqigfzy.top/gtxnbtcrpt.html

[T44] Perl：条件
来源：http://hz.nwbrower.top/gtmfjoicqx.html

if ($a > 0) { print "正"; }
来源：http://hz.yj20258.top/gthjwxptos.html

[T45] Perl：数组遍历
来源：http://hz.hammf.cn/gtlxmojqbh.html

for my $x (@arr) { print $x; }
来源：http://hz.yanxiufei.cn/gtubvlvzdn.html

[T46] Perl：哈希操作
来源：http://hz.gogol.net.cn/gtwascxeoo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hnqzz.top/gtprgsrgji.html

[T47] Perl：正则捕获
来源：http://hz.tian-w.cn/gtigybdxoi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gotoacloud.top/gtfwnsdfge.html

[T48] Perl：正则替换
来源：http://hz.ppjwa.cn/gtdpltpnpt.html

$s =~ s/old/new/g;
来源：http://hz.daria6918.cn/gtkxztmfwt.html

[T49] Perl：函数
来源：http://hz.mhx1999.top/gtmtzzhkip.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gzhubu.top/gtxenbfxxw.html

[T50] Perl：逐行读文件
来源：http://hz.fengsongda.top/gtsxgiolji.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.xylfe.cn/gtislpaopn.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jiagoushi.top/gtjuowlarb.html

[T51] Scala：Hello World
来源：http://hz.wangshuangyany.cn/gtutxtkkpa.html

println("Hello")
来源：http://hz.redwolf501.top/gtilltsxdn.html

[T52] Scala：变量
来源：http://hz.daria6918.cn/gtefvavrcg.html

val a = 1;  var b = 2
来源：http://hz.ywan-chungtsiang.top/gtvqhsyyod.html

[T53] Scala：字符串插值
来源：http://hz.svipenyu.cn/gtpnmtjpsv.html

s"值: $b"
来源：http://hz.jyoumei.cn/gtlxhncywm.html

[T54] Scala：集合映射
来源：http://hz.sysykeji.top/gttwbkapzw.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.meibo888.top/gttxydhmmc.html

[T55] Scala：集合过滤
来源：http://hz.zdqjudy.top/gtybynwwie.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.nwbrower.top/gttxoarumj.html

[T56] Scala：样例类
来源：http://hz.cdnleiting.top/gtvijxqrqs.html

case class User(name: String, age: Int)
来源：http://hz.c1oappe.top/gtyirbnsdz.html

[T57] Scala：模式匹配
来源：http://hz.fengsongda.top/gtlrcxrgdn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.aizwys.cn/gtttbrzxvf.html

[T58] Scala：函数定义
来源：http://hz.sufxvd.cn/gtlybwvqql.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.havefunace.top/gtsxmxeqen.html

[T59] Scala：循环
来源：http://hz.svipenyu.cn/gtaceppuhz.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhijiandao.cn/gtjreucwpf.html

[T60] Scala：折叠
来源：http://hz.ppjwa.cn/gtxlszwjfr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.xylfe.cn/gtqdqqemyy.html

================================================================================
来源：http://hz.tanke756.top/gtuiyqkaku.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigfzy.top/gtwvmgafed.html

================================================================================
来源：http://hz.redwolf501.top/gtopcjuxhc.html

[U01] Py：创建虚拟环境
来源：http://hz.yuanzhike.top/gtcnrcbukp.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.wangdashe.top/gtznuompxm.html

[U02] Py：导出 / 安装依赖
来源：http://hz.daxiang520.top/gthbadlmwy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.sweek.top/gtupzohlnk.html

[U03] Py：加载 .env 配置
来源：http://hz.52xcode.cn/gtnqrzhweg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.quarkkingdee.top/gtpluibymt.html

[U04] Py：变量调试打印
来源：http://hz.ydjk.org.cn/gtddruaybm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.svipenyu.cn/gtvawgmkis.html

[U05] Py：列表去重且保序
来源：http://hz.zhaomingkeji.xyz/gtbrbinmjj.html

list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtnvlefyxe.html

[U06] Py：合并两个字典
来源：http://hz.snrcjt.cn/gttjmkiivm.html

{**a, **b}
来源：http://hz.birdmap.top/gtgircyhch.html

[U07] Py：反转字典键值
来源：http://hz.guannengcc.top/gtblyemqzr.html

{v: k for k, v in d.items()}
来源：http://hz.sysykeji.top/gtehlieren.html

[U08] Py：展平二维列表
来源：http://hz.316326.xyz/gtymwblpsw.html

[y for x in nested for y in x]
来源：http://hz.dashuyun.cn/gtkhyqqniv.html

[U09] Py：字典取最大值的键
来源：http://hz.shuidangran.top/gtmljaguep.html

max(d, key=d.get)
来源：http://hz.snrcjt.cn/gtfnjrhapk.html

[U10] Py：按值排序字典
来源：http://hz.xuanzx.com/gttxddqgek.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.0kj1m.cn/gtbibdfivy.html

[U11] Py：生成器表达式
来源：http://hz.zhijiandao.cn/gtpdlrosob.html

(x * 2 for x in arr)
来源：http://hz.zhiwuduotai.top/gtbeyvgodw.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.xingfuxueyuan.xyz/gtwpchppzo.html

Counter(arr).most_common(3)
来源：http://hz.zhaomingkeji.xyz/gtxcasifkn.html

[U13] Py：固定长度队列
来源：http://hz.xziqi.cn/gtquxegqxz.html

deque(maxlen=10)
来源：http://hz.zhiwuduotai.top/gtavspsaby.html

[U14] Py：分组收集到列表
来源：http://hz.xuetiantiany.cn/gtsxitiqoz.html

defaultdict(list)
来源：http://hz.daria6918.cn/gtpputphyb.html

[U15] Py：高精度计时
来源：http://hz.fzhhl.top/gtgjtfuada.html

t = time.perf_counter()
来源：http://hz.sxryk.cn/gtxaqrbfcu.html

[U16] Py：命令行参数解析
来源：http://hz.cqqwz.cn/gtxbvhrdut.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.mhx1999.top/gttpotguti.html

[U17] Py：初始化日志
来源：http://hz.vqdsnc.cn/gtjcqrxyhw.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.aizwys.cn/gtvjczmspu.html

[U18] Py：预编译正则
来源：http://hz.316326.xyz/gtezgsutht.html

pat = re.compile(r"\d+")
来源：http://hz.feifeiyinyue.top/gtwadzsnyi.html

[U19] Py：正则替换带回调
来源：http://hz.cucudq.cn/gtyayomjzn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yonumen.top/gteqazbnad.html

[U20] Py：缓存函数结果
来源：http://hz.yuanzhike.top/gthsmrkqkj.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zhijiandao.cn/gtknzfddng.html

[U21] Py：自定义上下文管理器
来源：http://hz.cucudq.cn/gthnkqhtyg.html

@contextlib.contextmanager
来源：http://hz.jyoumei.cn/gtupqvumxp.html

[U22] Py：矩阵转置
来源：http://hz.tanke756.top/gtztbmtvyk.html

list(zip(*m))
来源：http://hz.smart0.xyz/gtxnvigpfi.html

[U23] Py：分块读取大文件
来源：http://hz.xuanzx.com/gtdtqdfndy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.quarkkingdee.top/gtbigcybfc.html

[U24] Py：路径操作
来源：http://hz.shanyushiyangtech.top/gtpvsswfzx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.fzhhl.top/gtyizdfhno.html

[U25] Py：CSV 按字典读
来源：http://hz.yanxiufei.cn/gtmgoujick.html

csv.DictReader(f)
来源：http://hz.chenjidiqi.icu/gtjqkglsex.html

[U26] Py：并发下载
来源：http://hz.snrcjt.cn/gtbzkjcylg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.chenjidiqi.icu/gtjfkrxxsb.html

[U27] Py：异步 HTTP
来源：http://hz.zhoulong.xyz/gtkrteyebm.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.svipenyu.cn/gtsrvwqwbw.html

[U28] Py：类型别名
来源：http://hz.mhx1999.top/gtcjejpeev.html

UserId = int
来源：http://hz.nwbrower.top/gtogszsxcp.html

[U29] Py：属性校验
来源：http://hz.smart0.xyz/gteiezkbxz.html

@property 与 @x.setter 配合
来源：http://hz.snrcjt.cn/gttgblpckg.html

[U30] Py：数据类
来源：http://hz.nwbrower.top/gtznmltpva.html

@dataclass(slots=True)
来源：http://hz.jinqigufen.top/gtrpkadznp.html

[U31] Py：单测
来源：http://hz.andypj.xyz/gtkwftivpk.html

python -m pytest -q
来源：http://hz.gogol.net.cn/gtyqvtfckg.html

[U32] Py：代码格式化
来源：http://hz.9152youxi.cn/gtiomspoyn.html

ruff format . && ruff check --fix .
来源：http://hz.zdqjudy.top/gtgbtczawj.html

[U33] Py：打包发布
来源：http://hz.hfpthk.cn/gtdmozmmon.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.pengpengdd.cyou/gtnjgaejuu.html

[U34] Py：判断编码
来源：http://hz.wangdashe.top/gtoohegory.html

chardet.detect(raw)
来源：http://hz.hywenlv.cn/gtalbigdha.html

[U35] Py：发送邮件
来源：http://hz.pengpengdd.cyou/gtpbdvjjmm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.guannengcc.top/gtptcbbqwp.html

[U36] Py：定时任务
来源：http://hz.zhongyouzk.top/gtyxizhfca.html

schedule.every(10).minutes.do(job)
来源：http://hz.gotoacloud.top/gtornzfqyy.html

[U37] Py：读写 Excel
来源：http://hz.yuxming.cn/gtjivuajil.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ivvv.top/gtirczvmjy.html

[U38] Py：获取脚本所在目录
来源：http://hz.ydzc1.top/gtuzjrbnsu.html

Path(__file__).resolve().parent
来源：http://hz.kuanghao11.cn/gtftjblkra.html

[U39] Py：判断是否在交互环境
来源：http://hz.guowangkeji.top/gtrlbshkjt.html

sys.stdout.isatty()
来源：http://hz.52xcode.cn/gtdgrqpnre.html

[U40] Py：打印到标准错误
来源：http://hz.havefunace.top/gtxxlvzhok.html

print("err", file=sys.stderr)
来源：http://hz.jinqigufen.top/gtskiaxeax.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.fengsongda.top/gtubebyhjg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.wangshuangyany.cn/gtxlrefbau.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jinyuanbaomall.cn/gtexpgqbvy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.vqdsnc.cn/gtbcaqghma.html

[U43] PHP：声明命名空间
来源：http://hz.hongshengwenyu.top/gtlsfxmgkt.html

namespace App\Http;
来源：http://hz.quarkkingdee.top/gtbdoopbzv.html

[U44] PHP：开启严格类型
来源：http://hz.yuanzhike.top/gtplwzdcad.html

declare(strict_types=1);
来源：http://hz.gogol.net.cn/gtdjqluijy.html

[U45] PHP：类型声明与返回类型
来源：http://hz.nanxuanxn.top/gtklbapfyv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtwvbkuqkv.html

[U46] PHP：可空类型
来源：http://hz.kuanghao11.cn/gtffpfzkbm.html

?string $name = null
来源：http://hz.shuidangran.top/gtidczabri.html

[U47] PHP：联合类型
来源：http://hz.jinyuanbaomall.cn/gtwbifnqsx.html

int|string $id
来源：http://hz.ppjwa.cn/gthgaffjcg.html

[U48] PHP：纯枚举
来源：http://hz.c1oappe.top/gthcdvbplu.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.wangshuangyany.cn/gtuoxyzuqg.html

[U49] PHP：只读属性
来源：http://hz.zhoulong.xyz/gtupoibdpf.html

public readonly string $name
来源：http://hz.jlsjyb.cn/gtclyotdyh.html

[U50] PHP：构造器属性提升
来源：http://hz.kuanghao11.cn/gtdcafihaj.html

public function __construct(private int $id) {}
来源：http://hz.hysaishi.cn/gtwkftnpqv.html

[U51] PHP：数组解构
来源：http://hz.jianghu66.top/gtlnjovonh.html

[$a, $b] = $arr;
来源：http://hz.cucudq.cn/gtrnbksohk.html

[U52] PHP：箭头函数
来源：http://hz.sxryk.cn/gtvttddajj.html

$double = fn($x) => $x * 2;
来源：http://hz.zhoulong.xyz/gtdjdbmoja.html

[U53] PHP：空合并运算符
来源：http://hz.yvedp.cn/gtzglgzsjb.html

$v = $a ?? $b ?? "default";
来源：http://hz.316326.xyz/gtzfjbdgpn.html

[U54] PHP：空安全调用
来源：http://hz.guannengcc.top/gtqxfqaayf.html

$obj?->method()
来源：http://hz.wangdashe.top/gtzhderslx.html

[U55] PHP：match 表达式
来源：http://hz.zhijiandao.cn/gtqwinngix.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.chenlongwang.top/gtljwsqhge.html

[U56] PHP：命名参数
来源：http://hz.daxiang520.top/gtjqherhsx.html

f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtqgiwmjsc.html

[U57] PHP：字符串插值
来源：http://hz.jqgufenzy.top/gtlwjtkouo.html

"值: {$a}"
来源：http://hz.jiagoushi.top/gtbvjrevjs.html

[U58] PHP：数组三件套
来源：http://hz.iojbl.cn/gtjapkserb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.redwolf501.top/gtwpyzyomk.html

[U59] PHP：自定义排序
来源：http://hz.ppjwa.cn/gtisonfbov.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yj20258.top/gtkjxbdqdi.html

[U60] PHP：JSON 编解码
来源：http://hz.shuidangran.top/gtmugeybef.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ehwqpu.com/gtuequfyfl.html

[U61] PHP：正则
来源：http://hz.zdqjudy.top/gtcochrapy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinyuanbaomall.cn/gtrbgwghkg.html

[U62] PHP：日期对象
来源：http://hz.zhaomingkeji.xyz/gtdzydunbz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yongpay.top/gtakwwkckj.html

[U63] PHP：文件读写
来源：http://hz.hnqzz.top/gtiqhbosjf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jianghu66.top/gtlkcvcsew.html

[U64] PHP：目录遍历
来源：http://hz.dianchejie.cn/gtpvdqldui.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hnxiangtu.top/gtwklkndrc.html

[U65] PHP：会话
来源：http://hz.sxryk.cn/gtrllisoly.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.sufxvd.cn/gtnhkhnygl.html

[U66] PHP：设置 Cookie
来源：http://hz.zhoulong.xyz/gtlrfbacou.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.jianghu66.top/gtmtwcggys.html

[U67] PHP：处理文件上传
来源：http://hz.jlsjyb.cn/gtxaqoyspp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.9152youxi.cn/gtgnmuiywb.html

[U68] PHP：PDO 连接
来源：http://hz.hnqzz.top/gtbsacuciy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.svipenyu.cn/gtuebyxexw.html

[U69] PHP：PDO 预处理
来源：http://hz.xuanzx.com/gtwzwwvkae.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.aizwys.cn/gtykfkiflx.html

[U70] PHP：PDO 事务
来源：http://hz.hongshengwenyu.top/gtfgnwtyuk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jinqigufen.top/gtgplyzxuf.html

[U71] PHP：抛出异常
来源：http://hz.gzhubu.top/gtczawauut.html

throw new RuntimeException("失败", 500);
来源：http://hz.hnqzz.top/gtmppemmwy.html

[U72] PHP：写错误日志
来源：http://hz.hnqzz.top/gtuukemsgc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.52xcode.cn/gtefmhcuzl.html

[U73] PHP：读取 ini 配置
来源：http://hz.meibo888.top/gtwybgwikn.html

parse_ini_file("config.ini", true)
来源：http://hz.jinqigufen.top/gtjiloqfpp.html

[U74] PHP：读取环境变量
来源：http://hz.redwolf501.top/gtgsejqjmy.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jqgfzy.top/gtihrrzjfz.html

[U75] PHP：依赖注入
来源：http://hz.52xcode.cn/gtvbxkqwdn.html

composer require psr/container
来源：http://hz.ppjwa.cn/gtbjnhiavg.html

[U76] PHP：简单路由
来源：http://hz.shuidangran.top/gtdghhtxal.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.kuanghao11.cn/gtzugqvzkt.html

[U77] PHP：模板渲染
来源：http://hz.dashuyun.cn/gtibtjktkp.html

composer require twig/twig
来源：http://hz.jinqigfzy.top/gtdlxlcpfj.html

[U78] PHP：单元测试
来源：http://hz.smart0.xyz/gtjiwbotdb.html

composer require --dev phpunit/phpunit
来源：http://hz.xinyue.icu/gtokxahaqz.html


<!-- 参考信息 -->