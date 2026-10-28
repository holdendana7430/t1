代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.havefunace.top/gtsjpanoaf.html

[S57] C++：编译期常量
来源：http://hz.yangfankeji.com/gtnajfdjky.html

constexpr int N = 10;
来源：http://hz.xinyue.icu/gtslerprkl.html

[S58] C++：命名空间
来源：http://hz.wangdashe.top/gtthgnscge.html

namespace ns { int f() { return 1; } }
来源：http://hz.snrcjt.cn/gtuoixcfph.html

[S59] C++：静态断言
来源：http://hz.hongshengwenyu.top/gtnfyqyvhv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xziqi.cn/gtobsbkkwh.html

[S60] C++：遍历并删除元素
来源：http://hz.ivvv.top/gtlgednosq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhijiandao.cn/gtqqqliqef.html

================================================================================
来源：http://hz.ybcxt.top/gtmnqtsoau.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shuidangran.top/gtsqyfxvjw.html

================================================================================
来源：http://hz.shuidangran.top/gttebbdgwo.html

[T01] Kotlin：Hello World
来源：http://hz.xylfe.cn/gthgveecqj.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gtoepvdpjs.html

[T02] Kotlin：变量
来源：http://hz.yj20258888.top/gtaoemfeen.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sysykeji.top/gtoiknjlsq.html

[T03] Kotlin：字符串模板
来源：http://hz.yuanzhike.top/gtshgjeerz.html

"值: $b"
来源：http://hz.hnqzz.top/gtiiecbhch.html

[T04] Kotlin：空安全
来源：http://hz.pengpengdd.cyou/gtxkmfzqjq.html

val n: String? = null;  n?.length
来源：http://hz.quarkkingdee.top/gtwkvprcmb.html

[T05] Kotlin：when 表达式
来源：http://hz.cdnleiting.top/gtmowilric.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shzxlz.cn/gtzmvlshqh.html

[T06] Kotlin：集合映射
来源：http://hz.pycfn.com/gtnpqcyeal.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zdqjudy.top/gtslvnecgz.html

[T07] Kotlin：集合过滤
来源：http://hz.chenzaomai.com/gtsooacaqu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gogol.net.cn/gtzbflazqj.html

[T08] Kotlin：数据类
来源：http://hz.dianchejie.cn/gtpscdtidx.html

data class User(val name: String, val age: Int)
来源：http://hz.wangdashe.top/gtoluhczzk.html

[T09] Kotlin：扩展函数
来源：http://hz.gzhubu.top/gtvnkyiboh.html

fun String.exclaim() = this + "!"
来源：http://hz.guowangkeji.top/gtufnaceax.html

[T10] Kotlin：默认参数
来源：http://hz.yj202588.top/gtrnqyhvvf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj20258888.top/gtjddvpxxn.html

[T11] Kotlin：协程
来源：http://hz.52xcode.cn/gtatjmvjoy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydjk.org.cn/gtecfydnto.html

[T12] Kotlin：解构声明
来源：http://hz.gaohongyu789.top/gtmcmqoasf.html

val (a, b) = Pair(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtlzmoyqok.html

[T13] Kotlin：只读 Map
来源：http://hz.jiagoushi.top/gtgiqohtpt.html

val m = mapOf("a" to 1)
来源：http://hz.0kj1m.cn/gtkzdoapew.html

[T14] Kotlin：循环
来源：http://hz.ppjwa.cn/gtdtyjpesy.html

for (i in 1..10) println(i)
来源：http://hz.jianghu66.top/gtrfdamylr.html

[T15] Kotlin：接口
来源：http://hz.cqqwz.cn/gturfidsax.html

interface Shape { fun area(): Double }
来源：http://hz.havefunace.top/gtspgmnejj.html

[T16] Swift：Hello World
来源：http://hz.ydzc1.top/gtjulaxvwo.html

print("Hello")
来源：http://hz.yvedp.cn/gtwmdelmtv.html

[T17] Swift：变量与常量
来源：http://hz.nwbrower.top/gtoulakugz.html

var a = 1;  let b = 2
来源：http://hz.zhiwuduotai.top/gtbgjrcwwa.html

[T18] Swift：字符串插值
来源：http://hz.pengpengdd.cyou/gtvxayfdtd.html

"值: \(b)"
来源：http://hz.zhengqikj.top/gthoarxpby.html

[T19] Swift：可选绑定
来源：http://hz.wangdashe.top/gtniwtvije.html

if let n = opt { print(n) }
来源：http://hz.yuxming.cn/gtsfvemypd.html

[T20] Swift：数组操作
来源：http://hz.yonumen.top/gttyqholng.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jiagoushi.top/gtpbiicwbx.html

[T21] Swift：遍历
来源：http://hz.wangdashe.top/gtxaitypmx.html

for x in a { print(x) }
来源：http://hz.shanyushiyangtech.top/gtacmyxuaw.html

[T22] Swift：字典
来源：http://hz.yanxiufei.cn/gthwseezpc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xylfe.cn/gtincfuvvs.html

[T23] Swift：函数
来源：http://hz.jinyuanbaomall.cn/gtzifdxhnv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigufen.top/gtiwmiutgq.html

[T24] Swift：闭包
来源：http://hz.zhiwuduotai.top/gtxxegelgf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ybcxt.top/gtckyhvkto.html

[T25] Swift：结构体
来源：http://hz.zhongyouzk.top/gtjtagjrwr.html

struct P { var x: Int }
来源：http://hz.zhiwuduotai.top/gthgkueogd.html

[T26] Swift：类与重写
来源：http://hz.birdmap.top/gtvxjvhoox.html

class A: Base { override func f() {} }
来源：http://hz.jinqigufen.top/gtptcftpfq.html

[T27] Swift：错误处理
来源：http://hz.jqgufenzy.top/gtsklncqhf.html

do { try f() } catch { print(error) }
来源：http://hz.svipenyu.cn/gtbbocrvyn.html

[T28] Swift：枚举
来源：http://hz.zhoulong.xyz/gtsrttsfcv.html

enum Color { case red, green }
来源：http://hz.hammf.cn/gtrptfuwdt.html

[T29] Swift：guard 提前返回
来源：http://hz.hongshengwenyu.top/gttztgxpqd.html

guard let x = opt else { return }
来源：http://hz.meibo888.top/gtpqdkwfqu.html

[T30] Swift：协议
来源：http://hz.zhijiandao.cn/gtlazldsdm.html

protocol Shape { func area() -> Double }
来源：http://hz.ydzc1.top/gttrezqruy.html

[T31] Lua：Hello World
来源：http://hz.zhoulong.xyz/gtmygwrgkn.html

print("Hello")
来源：http://hz.zycfv.cn/gthiwvjbbt.html

[T32] Lua：局部变量
来源：http://hz.daxiang520.top/gtazmeanyb.html

local a = 1
来源：http://hz.shangyingyoupin.top/gtwthdzzdy.html

[T33] Lua：表（数组）
来源：http://hz.redwolf501.top/gtjaqkwotl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cheryme.top/gtwpxpvgpe.html

[T34] Lua：遍历表
来源：http://hz.hnxiangtu.top/gtlqgwqiwt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cdnleiting.top/gtjxyznbry.html

[T35] Lua：字典表
来源：http://hz.fengsongda.top/gtvbvargrn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.316326.xyz/gttgwxzsmt.html

[T36] Lua：函数
来源：http://hz.ehwqpu.com/gtrlrkguct.html

function add(a, b) return a + b end
来源：http://hz.pycfn.com/gttqjrxedv.html

[T37] Lua：字符串拼接
来源：http://hz.shanyushiyangtech.top/gtmszaahzs.html

"a" .. "b"
来源：http://hz.jinghuilouyu.cn/gtqsanrnaa.html

[T38] Lua：条件
来源：http://hz.cheryme.top/gtjnzzfyhl.html

if x > 0 then print("正") end
来源：http://hz.kuanghao11.cn/gtooweirxf.html

[T39] Lua：模式匹配
来源：http://hz.xinyue.icu/gtcanuqipi.html

string.find(s, "%d+")
来源：http://hz.yuxming.cn/gtwxkxdpxi.html

[T40] Lua：元表
来源：http://hz.yangfankeji.com/gtxunlrkqh.html

setmetatable({}, { __index = base })
来源：http://hz.jinghuilouyu.cn/gtwjitmxcj.html

[T41] Perl：Hello World
来源：http://hz.wangshuangyany.cn/gtistrqnda.html

print "Hello\n";
来源：http://hz.52xcode.cn/gtkhwctahi.html

[T42] Perl：变量类型
来源：http://hz.hywenlv.cn/gtnxybtwhu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yj20258888.top/gtrayjuhpx.html

[T43] Perl：字符串插值
来源：http://hz.shanyushiyangtech.top/gtxdawtclf.html

"值: $a"
来源：http://hz.shangyingyoupin.top/gtwxrpyrnm.html

[T44] Perl：条件
来源：http://hz.yj202588.top/gtzwlcioss.html

if ($a > 0) { print "正"; }
来源：http://hz.xinyue.icu/gtqreriixm.html

[T45] Perl：数组遍历
来源：http://hz.cucudq.cn/gthgftjwfu.html

for my $x (@arr) { print $x; }
来源：http://hz.jqgufenzy.top/gtqneqyjsp.html

[T46] Perl：哈希操作
来源：http://hz.guowangkeji.top/gtazkqrsms.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.nanxinkj.top/gtfstugvnl.html

[T47] Perl：正则捕获
来源：http://hz.tianlin.xyz/gtuaqmrxob.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.cucudq.cn/gtowruqrzj.html

[T48] Perl：正则替换
来源：http://hz.hammf.cn/gtnqpzhhzz.html

$s =~ s/old/new/g;
来源：http://hz.zhixingplan.top/gtaeqnferu.html

[T49] Perl：函数
来源：http://hz.dashuyun.cn/gtttetvgrq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xuanzx.com/gtwihequdy.html

[T50] Perl：逐行读文件
来源：http://hz.chenzaomai.com/gtdtzigkzs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.aizwys.cn/gtpuzeeefv.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cheryme.top/gteekhoxvc.html

[T51] Scala：Hello World
来源：http://hz.redwolf501.top/gtdnvmqwqy.html

println("Hello")
来源：http://hz.mhx1999.top/gtpfegahsf.html

[T52] Scala：变量
来源：http://hz.wangdashe.top/gtdnuuanwh.html

val a = 1;  var b = 2
来源：http://hz.sxryk.cn/gtgmgtmlzo.html

[T53] Scala：字符串插值
来源：http://hz.jinqigufen.top/gtvqojjplk.html

s"值: $b"
来源：http://hz.yuxming.cn/gttidhuhwu.html

[T54] Scala：集合映射
来源：http://hz.zhijiandao.cn/gtmopgssyl.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.haohaochexian.top/gtuvyycdqd.html

[T55] Scala：集合过滤
来源：http://hz.zhongyouzk.top/gtrzcutees.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.jinyuanbaomall.cn/gtzkcghnec.html

[T56] Scala：样例类
来源：http://hz.fengsongda.top/gtzdiuhvik.html

case class User(name: String, age: Int)
来源：http://hz.cqqwz.cn/gtkdwecudj.html

[T57] Scala：模式匹配
来源：http://hz.ivvv.top/gtgnxwemxz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.ydjk.org.cn/gtasmuooce.html

[T58] Scala：函数定义
来源：http://hz.jinqigfzy.top/gtdczltunx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.c1oappe.top/gtclvhvyje.html

[T59] Scala：循环
来源：http://hz.mhx1999.top/gthhvlzziv.html

for (i <- 1 to 10) println(i)
来源：http://hz.meibo888.top/gtfcpnjzhd.html

[T60] Scala：折叠
来源：http://hz.316326.xyz/gtfksavnhm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.feifeiyinyue.top/gtbkaamohl.html

================================================================================
来源：http://hz.ehwqpu.com/gtubqvazce.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hongshengwenyu.top/gtwzdwreqt.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtpqlcncyp.html

[U01] Py：创建虚拟环境
来源：http://hz.tianlin.xyz/gtetfickrt.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.svipenyu.cn/gttanvspgl.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jqgfzy.top/gtenurqaee.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cdnleiting.top/gtebymqhdo.html

[U03] Py：加载 .env 配置
来源：http://hz.jinqigufen.top/gtkuvniqva.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.daxiang520.top/gtkzdkbqdj.html

[U04] Py：变量调试打印
来源：http://hz.mhx1999.top/gtrvrvvjce.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhoulong.xyz/gtbkszbjyj.html

[U05] Py：列表去重且保序
来源：http://hz.jqgfzy.top/gtlulxdyjn.html

list(dict.fromkeys(arr))
来源：http://hz.hysaishi.cn/gtnlstdzmu.html

[U06] Py：合并两个字典
来源：http://hz.aizwys.cn/gtahtuxkrc.html

{**a, **b}
来源：http://hz.ydzc1.top/gthckkcbwk.html

[U07] Py：反转字典键值
来源：http://hz.xingfuxueyuan.xyz/gtnbbrbcbt.html

{v: k for k, v in d.items()}
来源：http://hz.ehwqpu.com/gtujqbgzej.html

[U08] Py：展平二维列表
来源：http://hz.52xcode.cn/gtjzvhwzoy.html

[y for x in nested for y in x]
来源：http://hz.yonumen.top/gtnwxxoemm.html

[U09] Py：字典取最大值的键
来源：http://hz.yanxiufei.cn/gtpzpihctu.html

max(d, key=d.get)
来源：http://hz.ivvv.top/gtwklodpid.html

[U10] Py：按值排序字典
来源：http://hz.quarkkingdee.top/gtsscszykh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.feifeiyinyue.top/gtyohqqfge.html

[U11] Py：生成器表达式
来源：http://hz.jinqigfzy.top/gtzrjbznln.html

(x * 2 for x in arr)
来源：http://hz.jinghuilouyu.cn/gttpyrekul.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hongshengwenyu.top/gtgzuzfrpj.html

Counter(arr).most_common(3)
来源：http://hz.daria6918.cn/gtqfsdkxwa.html

[U13] Py：固定长度队列
来源：http://hz.nanxinkj.top/gtsvygysfh.html

deque(maxlen=10)
来源：http://hz.jinqigufen.top/gtncfbzeju.html

[U14] Py：分组收集到列表
来源：http://hz.gotoacloud.top/gtfputtjcg.html

defaultdict(list)
来源：http://hz.xinyue.icu/gtgyyroqla.html

[U15] Py：高精度计时
来源：http://hz.yj20258888.top/gtvippmdlf.html

t = time.perf_counter()
来源：http://hz.yueranfly.top/gtewfpohau.html

[U16] Py：命令行参数解析
来源：http://hz.yvedp.cn/gtgloxklra.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.xingfuxueyuan.xyz/gtzrmzjspb.html

[U17] Py：初始化日志
来源：http://hz.yj202588.top/gtjeharvht.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.meibo888.top/gtlqqybpdk.html

[U18] Py：预编译正则
来源：http://hz.ydzc1.top/gtouoohsae.html

pat = re.compile(r"\d+")
来源：http://hz.pengpengdd.cyou/gtggxrusti.html

[U19] Py：正则替换带回调
来源：http://hz.dashuyun.cn/gtvhyjzfnu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.svipenyu.cn/gthhbeugmm.html

[U20] Py：缓存函数结果
来源：http://hz.gaohongyu789.top/gtmmsgwjyh.html

@functools.lru_cache(maxsize=None)
来源：http://hz.zdqjudy.top/gtkjcccopv.html

[U21] Py：自定义上下文管理器
来源：http://hz.c1oappe.top/gtqxutszbs.html

@contextlib.contextmanager
来源：http://hz.gaohongyu789.top/gtrmmvvzsg.html

[U22] Py：矩阵转置
来源：http://hz.ppjwa.cn/gtexlmajfg.html

list(zip(*m))
来源：http://hz.jinqigfzy.top/gtfagxzocl.html

[U23] Py：分块读取大文件
来源：http://hz.gzhubu.top/gtxrdojbrl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yonumen.top/gtlvnwsrvz.html

[U24] Py：路径操作
来源：http://hz.guowangkeji.top/gtnyrnotfy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.zycfv.cn/gtxdqhkshn.html

[U25] Py：CSV 按字典读
来源：http://hz.jiagoushi.top/gtfomjorgy.html

csv.DictReader(f)
来源：http://hz.shuidangran.top/gtmyrrfeuz.html

[U26] Py：并发下载
来源：http://hz.zdqjudy.top/gtxqcczrzx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.zhengqikj.top/gtgidzxwea.html

[U27] Py：异步 HTTP
来源：http://hz.sufxvd.cn/gtxhsyfyml.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.52xcode.cn/gtgabhpjhj.html

[U28] Py：类型别名
来源：http://hz.aibaodan.cn/gtbcbcxvzm.html

UserId = int
来源：http://hz.yanxiufei.cn/gtrcdcvwqv.html

[U29] Py：属性校验
来源：http://hz.hammf.cn/gtqdqrfpor.html

@property 与 @x.setter 配合
来源：http://hz.nanxuanxn.top/gtgesjaozp.html

[U30] Py：数据类
来源：http://hz.bjfxy.top/gtqrhsgfom.html

@dataclass(slots=True)
来源：http://hz.tian-w.cn/gtwdkmtfca.html

[U31] Py：单测
来源：http://hz.xinyue.icu/gtibeqifhh.html

python -m pytest -q
来源：http://hz.xziqi.cn/gtpbtgxcwa.html

[U32] Py：代码格式化
来源：http://hz.zhiwuduotai.top/gtdubkeihs.html

ruff format . && ruff check --fix .
来源：http://hz.cucudq.cn/gtwbnioyqa.html

[U33] Py：打包发布
来源：http://hz.daxiang520.top/gtybuoptup.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.havefunace.top/gtwvnwlypq.html

[U34] Py：判断编码
来源：http://hz.mhx1999.top/gtejwwwsof.html

chardet.detect(raw)
来源：http://hz.chenzaomai.com/gtygqyxmuf.html

[U35] Py：发送邮件
来源：http://hz.ppjwa.cn/gtmmsdvjqa.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.hywenlv.cn/gthizcylrr.html

[U36] Py：定时任务
来源：http://hz.shuidangran.top/gtozygnjkl.html

schedule.every(10).minutes.do(job)
来源：http://hz.smart0.xyz/gtrsqchred.html

[U37] Py：读写 Excel
来源：http://hz.yvedp.cn/gtheszvihx.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.ywan-chungtsiang.top/gttnjkvwcf.html

[U38] Py：获取脚本所在目录
来源：http://hz.tianlin.xyz/gtvpklmeti.html

Path(__file__).resolve().parent
来源：http://hz.jinqigufen.top/gthocwsbiq.html

[U39] Py：判断是否在交互环境
来源：http://hz.snrcjt.cn/gtyjljrrwe.html

sys.stdout.isatty()
来源：http://hz.c1oappe.top/gtaejlwnkl.html

[U40] Py：打印到标准错误
来源：http://hz.9152youxi.cn/gtpiclpbbj.html

print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtjwkcfmeu.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.redwolf501.top/gtopldzeze.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.yuxming.cn/gtaarqclad.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jinyuanbaomall.cn/gtgexkmibr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.shanyushiyangkeji.top/gtlegmgyrk.html

[U43] PHP：声明命名空间
来源：http://hz.chenjidiqi.icu/gthavcvvva.html

namespace App\Http;
来源：http://hz.xinyue.icu/gtxvnljaml.html

[U44] PHP：开启严格类型
来源：http://hz.yj20258.top/gtxcmxcxzp.html

declare(strict_types=1);
来源：http://hz.chenzaomai.com/gtfthuebri.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hfpthk.cn/gtvmmprsap.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtqqtmdgfz.html

[U46] PHP：可空类型
来源：http://hz.hnxiangtu.top/gtmagxwjnp.html

?string $name = null
来源：http://hz.tanke756.top/gthlkmvjuy.html

[U47] PHP：联合类型
来源：http://hz.xylfe.cn/gtiowxzkph.html

int|string $id
来源：http://hz.yuanzhike.top/gtzzzoupzy.html

[U48] PHP：纯枚举
来源：http://hz.xuetiantiany.cn/gtfautowpl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hywenlv.cn/gthemuhfze.html

[U49] PHP：只读属性
来源：http://hz.yangfankeji.com/gtrfbbtgra.html

public readonly string $name
来源：http://hz.dianchejie.cn/gtjqvtjozo.html

[U50] PHP：构造器属性提升
来源：http://hz.hnqzz.top/gtgexoqsbt.html

public function __construct(private int $id) {}
来源：http://hz.ydzc1.top/gtzpautlgd.html

[U51] PHP：数组解构
来源：http://hz.quarkkingdee.top/gtodprajmd.html

[$a, $b] = $arr;
来源：http://hz.ywan-chungtsiang.top/gtfmkkvgwd.html

[U52] PHP：箭头函数
来源：http://hz.sxryk.cn/gtwrbpculv.html

$double = fn($x) => $x * 2;
来源：http://hz.shzxlz.cn/gtwheiwewg.html

[U53] PHP：空合并运算符
来源：http://hz.hongshengwenyu.top/gtmlbllcyf.html

$v = $a ?? $b ?? "default";
来源：http://hz.yonumen.top/gtxbjdbpue.html

[U54] PHP：空安全调用
来源：http://hz.gotoacloud.top/gtgnfbqwea.html

$obj?->method()
来源：http://hz.jinghuilouyu.cn/gtbtdgwpgi.html

[U55] PHP：match 表达式
来源：http://hz.yj202588.top/gtzxonjjkb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.wangshuangyany.cn/gtrakqcdxa.html

[U56] PHP：命名参数
来源：http://hz.tianlin.xyz/gthoevxupb.html

f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtlbmjzrnf.html

[U57] PHP：字符串插值
来源：http://hz.xuetiantiany.cn/gtsbmmmfng.html

"值: {$a}"
来源：http://hz.cheryme.top/gtexpggbhf.html

[U58] PHP：数组三件套
来源：http://hz.ydzc1.top/gtrvkqscgi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jyoumei.cn/gtulkfmbkk.html

[U59] PHP：自定义排序
来源：http://hz.guannengcc.top/gtdqnjpivh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tianlin.xyz/gtkduxqarw.html

[U60] PHP：JSON 编解码
来源：http://hz.iojbl.cn/gtefrhekmw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.shzxlz.cn/gtqegxmgfc.html

[U61] PHP：正则
来源：http://hz.nanxinkj.top/gtvflcjnso.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.tanke756.top/gtwxywvacm.html

[U62] PHP：日期对象
来源：http://hz.xuanzx.com/gtndqxrwuq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.wangshuangyany.cn/gtvcqzttvj.html

[U63] PHP：文件读写
来源：http://hz.sufxvd.cn/gtjhlxnvkn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.gogol.net.cn/gtxkllwnzz.html

[U64] PHP：目录遍历
来源：http://hz.yanxiufei.cn/gtooaxfanz.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.dashuyun.cn/gttarbvujx.html

[U65] PHP：会话
来源：http://hz.gaohongyu789.top/gteauhevcb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.birdmap.top/gtaybspgnh.html

[U66] PHP：设置 Cookie
来源：http://hz.316326.xyz/gtekrnntik.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yj20258888.top/gtzphczskl.html

[U67] PHP：处理文件上传
来源：http://hz.yangfankeji.com/gtrzzghass.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.snrcjt.cn/gtbmynxyil.html

[U68] PHP：PDO 连接
来源：http://hz.cucudq.cn/gtkqxsdosb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.nanxinkj.top/gtbrrjncvu.html

[U69] PHP：PDO 预处理
来源：http://hz.jinyuanbaomall.cn/gtwcrkenqt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.zhengqikj.top/gtvmdnumim.html

[U70] PHP：PDO 事务
来源：http://hz.gotoacloud.top/gtxmbhtduk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.316326.xyz/gtndsiedtj.html

[U71] PHP：抛出异常
来源：http://hz.yueranfly.top/gtawlhbrvw.html

throw new RuntimeException("失败", 500);
来源：http://hz.cheryme.top/gtwdsspowv.html

[U72] PHP：写错误日志
来源：http://hz.fengsongda.top/gtwpsqbcvt.html

error_log("失败: " . $e->getMessage());
来源：http://hz.smart0.xyz/gtzvbqijdx.html

[U73] PHP：读取 ini 配置
来源：http://hz.jianghu66.top/gtftfpsqmq.html

parse_ini_file("config.ini", true)
来源：http://hz.zhixingplan.top/gtyciczbuk.html

[U74] PHP：读取环境变量
来源：http://hz.hnxiangtu.top/gtbcdlcxyd.html

getenv("APP_ENV") ?: "production"
来源：http://hz.aizwys.cn/gtejqrrzqh.html

[U75] PHP：依赖注入
来源：http://hz.havefunace.top/gtmhjxuqxf.html

composer require psr/container
来源：http://hz.ivvv.top/gttnnbsptr.html

[U76] PHP：简单路由
来源：http://hz.aizwys.cn/gtiswdppzi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.hammf.cn/gtekspenhq.html

[U77] PHP：模板渲染
来源：http://hz.smart0.xyz/gtmhtuatft.html

composer require twig/twig
来源：http://hz.9152youxi.cn/gtdfkkwdzj.html

[U78] PHP：单元测试
来源：http://hz.pycfn.com/gtnxjxttnn.html

composer require --dev phpunit/phpunit
来源：http://hz.guowangkeji.top/gtalhtpzwr.html

[U79] PHP：静态分析
来源：http://hz.hysaishi.cn/gtvkvbcoiz.html

composer require --dev phpstan/phpstan
来源：http://hz.zhongyouzk.top/gtagntsheh.html

[U80] PHP：代码规范修复
来源：http://hz.ivvv.top/gtbwettncn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.dashuyun.cn/gtadfwoosa.html

[U81] JS：初始化项目
来源：http://hz.aibaodan.cn/gtpavuwsbp.html

npm init -y;  npm i express
来源：http://hz.ehwqpu.com/gtsrsztsux.html

[U82] JS：package.json 脚本
来源：http://hz.tianlin.xyz/gtiasrphbe.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zdqjudy.top/gtlvnegfnb.html


<!-- 参考信息 -->