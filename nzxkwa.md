代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zdqjudy.top/gtqoajkpgv.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gtsbennpwv.html

constexpr int N = 10;
来源：http://hz.shanyushiyangkeji.top/gtqlpgnsyp.html

[S58] C++：命名空间
来源：http://hz.zhongyouzk.top/gtmcjvwmdf.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinghuilouyu.cn/gtemjosdwb.html

[S59] C++：静态断言
来源：http://hz.vqdsnc.cn/gtsshvqglv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hongshengwenyu.top/gtupvdiniw.html

[S60] C++：遍历并删除元素
来源：http://hz.zhoulong.xyz/gtriowrany.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.havefunace.top/gtftjanbti.html

================================================================================
来源：http://hz.jiagoushi.top/gtxvlvvdvm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.quarkkingdee.top/gtpaakgimu.html

================================================================================
来源：http://hz.chenlongwang.top/gtlhqgdupx.html

[T01] Kotlin：Hello World
来源：http://hz.chenlongwang.top/gtvfvwjqhq.html

println("Hello")
来源：http://hz.jinghuilouyu.cn/gtercndwfl.html

[T02] Kotlin：变量
来源：http://hz.yangfankeji.com/gtzpaefroq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinghuilouyu.cn/gtvkuitepz.html

[T03] Kotlin：字符串模板
来源：http://hz.shanyushiyangtech.top/gtfnvuiwzy.html

"值: $b"
来源：http://hz.wangdashe.top/gtfstdlnvs.html

[T04] Kotlin：空安全
来源：http://hz.ppjwa.cn/gtycqiajmz.html

val n: String? = null;  n?.length
来源：http://hz.jyoumei.cn/gtyigefinn.html

[T05] Kotlin：when 表达式
来源：http://hz.vqdsnc.cn/gtnfjzdzuk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenlongwang.top/gtmcwstmok.html

[T06] Kotlin：集合映射
来源：http://hz.cucudq.cn/gtrdyszzdo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.316326.xyz/gtevgiummr.html

[T07] Kotlin：集合过滤
来源：http://hz.ppjwa.cn/gtlwbzaaoh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gotoacloud.top/gtxvsnwqex.html

[T08] Kotlin：数据类
来源：http://hz.guowangkeji.top/gthfedtcar.html

data class User(val name: String, val age: Int)
来源：http://hz.zhengqikj.top/gtqtxeminh.html

[T09] Kotlin：扩展函数
来源：http://hz.redwolf501.top/gtkluopbnq.html

fun String.exclaim() = this + "!"
来源：http://hz.c1oappe.top/gtzpparpny.html

[T10] Kotlin：默认参数
来源：http://hz.jqgfzy.top/gttrthefyn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.nanxuanxn.top/gtuukrncau.html

[T11] Kotlin：协程
来源：http://hz.jqgufenzy.top/gtwarzzgxf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sysykeji.top/gtyqeaqxgb.html

[T12] Kotlin：解构声明
来源：http://hz.zhaomingkeji.xyz/gtifirkftt.html

val (a, b) = Pair(1, 2)
来源：http://hz.nanxinkj.top/gtqdkouuwd.html

[T13] Kotlin：只读 Map
来源：http://hz.iojbl.cn/gtubfeolux.html

val m = mapOf("a" to 1)
来源：http://hz.hongshengwenyu.top/gtaxtutczc.html

[T14] Kotlin：循环
来源：http://hz.wangdashe.top/gtrpjzsopv.html

for (i in 1..10) println(i)
来源：http://hz.gotoacloud.top/gtipbxwbyp.html

[T15] Kotlin：接口
来源：http://hz.zhongyouzk.top/gtsjxjjakv.html

interface Shape { fun area(): Double }
来源：http://hz.kuanghao11.cn/gtawmhgyqx.html

[T16] Swift：Hello World
来源：http://hz.ybcxt.top/gtcvmpxwzf.html

print("Hello")
来源：http://hz.jinghuilouyu.cn/gtgxgharzv.html

[T17] Swift：变量与常量
来源：http://hz.jinyuanbaomall.cn/gtqnspzkcl.html

var a = 1;  let b = 2
来源：http://hz.cqqwz.cn/gtdjxvhsjx.html

[T18] Swift：字符串插值
来源：http://hz.jinqigfzy.top/gtlvtuhbuz.html

"值: \(b)"
来源：http://hz.sxryk.cn/gtvnlmvcgk.html

[T19] Swift：可选绑定
来源：http://hz.redwolf501.top/gtdacsanaa.html

if let n = opt { print(n) }
来源：http://hz.fengsongda.top/gtxqfbecgi.html

[T20] Swift：数组操作
来源：http://hz.zhiwuduotai.top/gtpnlyitrk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ydjk.org.cn/gtyrfcumqa.html

[T21] Swift：遍历
来源：http://hz.hnqzz.top/gtmddxiqyk.html

for x in a { print(x) }
来源：http://hz.feifeiyinyue.top/gtyuklphxg.html

[T22] Swift：字典
来源：http://hz.feifeiyinyue.top/gtbgqrndrl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hywenlv.cn/gtsxfgojva.html

[T23] Swift：函数
来源：http://hz.smart0.xyz/gtxnfhqyol.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jyoumei.cn/gtqgzwflmk.html

[T24] Swift：闭包
来源：http://hz.andypj.xyz/gtaajudkwx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.mhx1999.top/gtnpyvmuhu.html

[T25] Swift：结构体
来源：http://hz.jinghuilouyu.cn/gtdgguzyux.html

struct P { var x: Int }
来源：http://hz.sxryk.cn/gtaaqvdfux.html

[T26] Swift：类与重写
来源：http://hz.zhixingplan.top/gtukvwstfq.html

class A: Base { override func f() {} }
来源：http://hz.tian-w.cn/gtlsdkqzlv.html

[T27] Swift：错误处理
来源：http://hz.wangdashe.top/gtikmpcvwl.html

do { try f() } catch { print(error) }
来源：http://hz.yuanzhike.top/gttumahpkb.html

[T28] Swift：枚举
来源：http://hz.sufxvd.cn/gtchslmkpu.html

enum Color { case red, green }
来源：http://hz.daria6918.cn/gtkzoapigj.html

[T29] Swift：guard 提前返回
来源：http://hz.zhiwuduotai.top/gtgfllxgoz.html

guard let x = opt else { return }
来源：http://hz.ybcxt.top/gtbxooenzn.html

[T30] Swift：协议
来源：http://hz.shzxlz.cn/gtgdxbolsa.html

protocol Shape { func area() -> Double }
来源：http://hz.vqdsnc.cn/gtkhwkmjwr.html

[T31] Lua：Hello World
来源：http://hz.zhixingplan.top/gtwejxfwhr.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtywagmeqt.html

[T32] Lua：局部变量
来源：http://hz.cucudq.cn/gtddhehjct.html

local a = 1
来源：http://hz.gotoacloud.top/gtiukcgcxo.html

[T33] Lua：表（数组）
来源：http://hz.chenzaomai.com/gtpuzmwnip.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nanxinkj.top/gtzoidtxcc.html

[T34] Lua：遍历表
来源：http://hz.52xcode.cn/gtqwmtmhxf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.dashuyun.cn/gtxzaimaby.html

[T35] Lua：字典表
来源：http://hz.zhengqikj.top/gtfzsvydgz.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gogol.net.cn/gtsfeqpxnh.html

[T36] Lua：函数
来源：http://hz.aizwys.cn/gtpzghwleh.html

function add(a, b) return a + b end
来源：http://hz.zycfv.cn/gtozfpcbmh.html

[T37] Lua：字符串拼接
来源：http://hz.haohaochexian.top/gtmyiuyghf.html

"a" .. "b"
来源：http://hz.zdqjudy.top/gtctrryehu.html

[T38] Lua：条件
来源：http://hz.yonumen.top/gtrqdxdtpt.html

if x > 0 then print("正") end
来源：http://hz.sysykeji.top/gtkwvlylve.html

[T39] Lua：模式匹配
来源：http://hz.hammf.cn/gtkekdfirz.html

string.find(s, "%d+")
来源：http://hz.aibaodan.cn/gttbiyjkzt.html

[T40] Lua：元表
来源：http://hz.shuidangran.top/gtfaoaadke.html

setmetatable({}, { __index = base })
来源：http://hz.shangyingyoupin.top/gtuxhafgvm.html

[T41] Perl：Hello World
来源：http://hz.nanxuanxn.top/gtgwgwvgya.html

print "Hello\n";
来源：http://hz.jianghu66.top/gtusscihyq.html

[T42] Perl：变量类型
来源：http://hz.sysykeji.top/gttvmjgrlj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.feifeiyinyue.top/gtxuxxvcfp.html

[T43] Perl：字符串插值
来源：http://hz.tian-w.cn/gtqivznxaz.html

"值: $a"
来源：http://hz.dashuyun.cn/gtfdqmhmwv.html

[T44] Perl：条件
来源：http://hz.ywan-chungtsiang.top/gtzirnpuat.html

if ($a > 0) { print "正"; }
来源：http://hz.9152youxi.cn/gtuaaumvbu.html

[T45] Perl：数组遍历
来源：http://hz.ydjk.org.cn/gtqzufolgz.html

for my $x (@arr) { print $x; }
来源：http://hz.jinyuanbaomall.cn/gtwzlsgvxt.html

[T46] Perl：哈希操作
来源：http://hz.smart0.xyz/gtpekfwnlx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.xingfuxueyuan.xyz/gtdzwytuzg.html

[T47] Perl：正则捕获
来源：http://hz.wangshuangyany.cn/gtqpcdtorn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zycfv.cn/gtjxmcnzxc.html

[T48] Perl：正则替换
来源：http://hz.hfpthk.cn/gtuoogvsyo.html

$s =~ s/old/new/g;
来源：http://hz.zhiwuduotai.top/gtlwkiubsl.html

[T49] Perl：函数
来源：http://hz.jinqigufen.top/gttrybsnzi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.mhx1999.top/gticxrawgy.html

[T50] Perl：逐行读文件
来源：http://hz.bjfxy.top/gtyormbdcg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jinqigufen.top/gtbtrastbi.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuanzx.com/gtliknrwjk.html

[T51] Scala：Hello World
来源：http://hz.shzxlz.cn/gtchnygfsc.html

println("Hello")
来源：http://hz.yueranfly.top/gtlamvdzvw.html

[T52] Scala：变量
来源：http://hz.ybcxt.top/gtzbvkiove.html

val a = 1;  var b = 2
来源：http://hz.tanke756.top/gtcvkgwzix.html

[T53] Scala：字符串插值
来源：http://hz.zhengqikj.top/gtczkzbajy.html

s"值: $b"
来源：http://hz.tanke756.top/gtbljcvvqg.html

[T54] Scala：集合映射
来源：http://hz.tian-w.cn/gthyqmazlq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yueranfly.top/gtcvonbwii.html

[T55] Scala：集合过滤
来源：http://hz.yvedp.cn/gtluffansv.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.yj202588.top/gtayfqxxvd.html

[T56] Scala：样例类
来源：http://hz.zhaomingkeji.xyz/gtmlwscflu.html

case class User(name: String, age: Int)
来源：http://hz.aizwys.cn/gtopsjwhqv.html

[T57] Scala：模式匹配
来源：http://hz.ywan-chungtsiang.top/gtidjheoyi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhijiandao.cn/gtpzczdfhw.html

[T58] Scala：函数定义
来源：http://hz.aibaodan.cn/gtktaygttp.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.jlsjyb.cn/gtmebolzon.html

[T59] Scala：循环
来源：http://hz.xuetiantiany.cn/gtauikkcbj.html

for (i <- 1 to 10) println(i)
来源：http://hz.jinyuanbaomall.cn/gtnryunmwp.html

[T60] Scala：折叠
来源：http://hz.jinqigfzy.top/gttqjznziq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hysaishi.cn/gtheeeaxfp.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtctjjqmnx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jqgufenzy.top/gthxquzbrx.html

================================================================================
来源：http://hz.tanke756.top/gtuvizbooq.html

[U01] Py：创建虚拟环境
来源：http://hz.vqdsnc.cn/gtvmmpqrdi.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.jyoumei.cn/gtxiifjszn.html

[U02] Py：导出 / 安装依赖
来源：http://hz.ivvv.top/gtdzacdmie.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cdnleiting.top/gthigxtdqv.html

[U03] Py：加载 .env 配置
来源：http://hz.jyoumei.cn/gtzysjrsnq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.zdqjudy.top/gtlxbnuait.html

[U04] Py：变量调试打印
来源：http://hz.tian-w.cn/gtyxrhmhcx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.xinyue.icu/gtwptyewmw.html

[U05] Py：列表去重且保序
来源：http://hz.zhixingplan.top/gtfxodaoat.html

list(dict.fromkeys(arr))
来源：http://hz.hnxiangtu.top/gtlonvkmxr.html

[U06] Py：合并两个字典
来源：http://hz.jqgfzy.top/gtvzecisae.html

{**a, **b}
来源：http://hz.ehwqpu.com/gtkqxckpnh.html

[U07] Py：反转字典键值
来源：http://hz.316326.xyz/gtnrcutuor.html

{v: k for k, v in d.items()}
来源：http://hz.pycfn.com/gtcihtjvne.html

[U08] Py：展平二维列表
来源：http://hz.zhaomingkeji.xyz/gtdijbqrnz.html

[y for x in nested for y in x]
来源：http://hz.zhiwuduotai.top/gtimgsfbih.html

[U09] Py：字典取最大值的键
来源：http://hz.sweek.top/gtamtonzzg.html

max(d, key=d.get)
来源：http://hz.zhijiandao.cn/gtyyvmqqma.html

[U10] Py：按值排序字典
来源：http://hz.xinyue.icu/gttldcpktj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.shzxlz.cn/gtlwazkhpe.html

[U11] Py：生成器表达式
来源：http://hz.wangshuangyany.cn/gtfporrtjf.html

(x * 2 for x in arr)
来源：http://hz.aizwys.cn/gtozhrwfrg.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.chenlongwang.top/gtmldsomge.html

Counter(arr).most_common(3)
来源：http://hz.shuidangran.top/gtxtaemafs.html

[U13] Py：固定长度队列
来源：http://hz.xinyue.icu/gtngcxzkqq.html

deque(maxlen=10)
来源：http://hz.guowangkeji.top/gteycadfcy.html

[U14] Py：分组收集到列表
来源：http://hz.sweek.top/gtkdoggqxm.html

defaultdict(list)
来源：http://hz.dashuyun.cn/gtvjfsoynn.html

[U15] Py：高精度计时
来源：http://hz.birdmap.top/gtxlrjemhq.html

t = time.perf_counter()
来源：http://hz.0kj1m.cn/gttmudaiue.html

[U16] Py：命令行参数解析
来源：http://hz.daxiang520.top/gtvyjqkmza.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.nanxinkj.top/gtikwuriyr.html

[U17] Py：初始化日志
来源：http://hz.zhengqikj.top/gtedbcvvfc.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.zhengqikj.top/gtwtaqwmry.html

[U18] Py：预编译正则
来源：http://hz.meibo888.top/gtehzvyxmw.html

pat = re.compile(r"\d+")
来源：http://hz.fengsongda.top/gtehfqicqz.html

[U19] Py：正则替换带回调
来源：http://hz.zhengqikj.top/gtnjmhmwdq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.9152youxi.cn/gtbjdjnqrz.html

[U20] Py：缓存函数结果
来源：http://hz.fzhhl.top/gtpjxtnoui.html

@functools.lru_cache(maxsize=None)
来源：http://hz.meibo888.top/gttlzdcaig.html

[U21] Py：自定义上下文管理器
来源：http://hz.tian-w.cn/gtathnwltt.html

@contextlib.contextmanager
来源：http://hz.daria6918.cn/gthtpwrvxv.html

[U22] Py：矩阵转置
来源：http://hz.jqgufenzy.top/gtdgbexqnz.html

list(zip(*m))
来源：http://hz.pycfn.com/gtbrsqibto.html

[U23] Py：分块读取大文件
来源：http://hz.zhoulong.xyz/gtcrbxwdwk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.sxryk.cn/gtdjcpbdgb.html

[U24] Py：路径操作
来源：http://hz.havefunace.top/gtudfcmnyd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xinyue.icu/gtbzjnyrkw.html

[U25] Py：CSV 按字典读
来源：http://hz.cucudq.cn/gthacnlblm.html

csv.DictReader(f)
来源：http://hz.gzhubu.top/gtxyiasshm.html

[U26] Py：并发下载
来源：http://hz.yuxming.cn/gthkmcefwk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.shzxlz.cn/gtyofysszy.html

[U27] Py：异步 HTTP
来源：http://hz.jinqigufen.top/gtdvxeteug.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.kuanghao11.cn/gtwmmeldhp.html

[U28] Py：类型别名
来源：http://hz.jiagoushi.top/gtkjgckfxd.html

UserId = int
来源：http://hz.cqqwz.cn/gtagfkxmww.html

[U29] Py：属性校验
来源：http://hz.nwbrower.top/gtqbnsmgzp.html

@property 与 @x.setter 配合
来源：http://hz.cdnleiting.top/gtaybfzuhn.html

[U30] Py：数据类
来源：http://hz.yj20258888.top/gtgxnjtscn.html

@dataclass(slots=True)
来源：http://hz.gotoacloud.top/gtklrxgyou.html

[U31] Py：单测
来源：http://hz.gzhubu.top/gtwuhziicw.html

python -m pytest -q
来源：http://hz.zhixingplan.top/gtliyspcju.html

[U32] Py：代码格式化
来源：http://hz.sxryk.cn/gtljabhriz.html

ruff format . && ruff check --fix .
来源：http://hz.xingfuxueyuan.xyz/gtwkkgobzp.html

[U33] Py：打包发布
来源：http://hz.zhijiandao.cn/gtezhrtoyk.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.feifeiyinyue.top/gtqlabqvqh.html

[U34] Py：判断编码
来源：http://hz.wangdashe.top/gtjzxhchth.html

chardet.detect(raw)
来源：http://hz.havefunace.top/gtueslwfpa.html

[U35] Py：发送邮件
来源：http://hz.hnqzz.top/gtrseqcuqq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.yvedp.cn/gtgxlynmkp.html

[U36] Py：定时任务
来源：http://hz.wangshuangyany.cn/gtvqofbyaa.html

schedule.every(10).minutes.do(job)
来源：http://hz.dianchejie.cn/gtnkphzcvr.html

[U37] Py：读写 Excel
来源：http://hz.birdmap.top/gtzuupzmnd.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.shzxlz.cn/gtpieoyqjg.html

[U38] Py：获取脚本所在目录
来源：http://hz.52xcode.cn/gtmrawrfwv.html

Path(__file__).resolve().parent
来源：http://hz.jinyuanbaomall.cn/gtcexvgyfn.html

[U39] Py：判断是否在交互环境
来源：http://hz.fengsongda.top/gtxvtbkhjb.html

sys.stdout.isatty()
来源：http://hz.feifeiyinyue.top/gtitzkzidv.html

[U40] Py：打印到标准错误
来源：http://hz.shangyingyoupin.top/gtkfkvmauq.html

print("err", file=sys.stderr)
来源：http://hz.hongshengwenyu.top/gtoxiplvfg.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinghuilouyu.cn/gtgbrxukef.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xingfuxueyuan.xyz/gtualdhlcc.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.meibo888.top/gttmxtxxyc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.hnxiangtu.top/gttswfwyke.html

[U43] PHP：声明命名空间
来源：http://hz.zhaomingkeji.xyz/gtahkjapzb.html

namespace App\Http;
来源：http://hz.zycfv.cn/gtbyrekpmw.html

[U44] PHP：开启严格类型
来源：http://hz.hywenlv.cn/gtzesxsxqf.html

declare(strict_types=1);
来源：http://hz.gogol.net.cn/gthhbnkidw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jianghu66.top/gtkrryoitl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gthhrmyanu.html

[U46] PHP：可空类型
来源：http://hz.xingfuxueyuan.xyz/gtnmiphprr.html

?string $name = null
来源：http://hz.fengsongda.top/gthvlfdosi.html

[U47] PHP：联合类型
来源：http://hz.snrcjt.cn/gtrirgwhwz.html

int|string $id
来源：http://hz.zdqjudy.top/gtqoybegue.html

[U48] PHP：纯枚举
来源：http://hz.tianlin.xyz/gtunoynebf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.gogol.net.cn/gtquzirqpc.html

[U49] PHP：只读属性
来源：http://hz.dianchejie.cn/gtowkuhyky.html

public readonly string $name
来源：http://hz.gzhubu.top/gtcnedczay.html

[U50] PHP：构造器属性提升
来源：http://hz.ppjwa.cn/gtxtltvjii.html

public function __construct(private int $id) {}
来源：http://hz.sweek.top/gtkojyrfjk.html

[U51] PHP：数组解构
来源：http://hz.xylfe.cn/gtapowqrvk.html

[$a, $b] = $arr;
来源：http://hz.hongshengwenyu.top/gtzwudvnli.html

[U52] PHP：箭头函数
来源：http://hz.daria6918.cn/gtmcqeuuwq.html

$double = fn($x) => $x * 2;
来源：http://hz.wangshuangyany.cn/gtvhurciim.html

[U53] PHP：空合并运算符
来源：http://hz.c1oappe.top/gtizutreqk.html

$v = $a ?? $b ?? "default";
来源：http://hz.wangdashe.top/gtjrigaeln.html

[U54] PHP：空安全调用
来源：http://hz.cqqwz.cn/gtfahzylpg.html

$obj?->method()
来源：http://hz.ppjwa.cn/gttabubgrg.html

[U55] PHP：match 表达式
来源：http://hz.hnqzz.top/gtahurivlg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.chenzaomai.com/gtbptaxiho.html

[U56] PHP：命名参数
来源：http://hz.hnxiangtu.top/gtbaaisogi.html

f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gtjtiqzvjd.html

[U57] PHP：字符串插值
来源：http://hz.ehwqpu.com/gtyuxfuvug.html

"值: {$a}"
来源：http://hz.yj20258888.top/gtiqitgvqo.html

[U58] PHP：数组三件套
来源：http://hz.haohaochexian.top/gtpdehmbvn.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.hammf.cn/gtxvumofnz.html

[U59] PHP：自定义排序
来源：http://hz.tianlin.xyz/gtytmxrujh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.havefunace.top/gtawhqcyrx.html

[U60] PHP：JSON 编解码
来源：http://hz.cqqwz.cn/gtffjrflbr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.vqdsnc.cn/gtugtvesab.html

[U61] PHP：正则
来源：http://hz.shzxlz.cn/gtiykqxheo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.smart0.xyz/gtomfjtvkb.html

[U62] PHP：日期对象
来源：http://hz.birdmap.top/gtmtzsqtnt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.ybcxt.top/gtbtbwepvl.html

[U63] PHP：文件读写
来源：http://hz.ivvv.top/gtqgqsscrk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.chenzaomai.com/gtjeoxampb.html

[U64] PHP：目录遍历
来源：http://hz.yonumen.top/gtatewpjnc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.redwolf501.top/gtcigjiuwy.html

[U65] PHP：会话
来源：http://hz.guannengcc.top/gtzczhdwtl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.vqdsnc.cn/gtxcfmsino.html

[U66] PHP：设置 Cookie
来源：http://hz.sufxvd.cn/gtcicbwjnh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.wangshuangyany.cn/gtcgivsadk.html

[U67] PHP：处理文件上传
来源：http://hz.nwbrower.top/gtwcyjswir.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.ydzc1.top/gtxuyonfxy.html

[U68] PHP：PDO 连接
来源：http://hz.cdnleiting.top/gtidlswuml.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.bjfxy.top/gtzettnzoa.html

[U69] PHP：PDO 预处理
来源：http://hz.zhongyouzk.top/gtbpqstajs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.yj20258888.top/gttdfvipaa.html

[U70] PHP：PDO 事务
来源：http://hz.fengsongda.top/gtzjmcgcuy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.yvedp.cn/gthzkrppnv.html

[U71] PHP：抛出异常
来源：http://hz.shanyushiyangtech.top/gtinhjgqcc.html

throw new RuntimeException("失败", 500);
来源：http://hz.ehwqpu.com/gtdkhiozvl.html

[U72] PHP：写错误日志
来源：http://hz.ydzc1.top/gtptpjuaxc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.yueranfly.top/gtodbtzigx.html

[U73] PHP：读取 ini 配置
来源：http://hz.zdqjudy.top/gtgsncvhkd.html

parse_ini_file("config.ini", true)
来源：http://hz.jyoumei.cn/gtkeutokei.html

[U74] PHP：读取环境变量
来源：http://hz.nanxinkj.top/gttdskbtbq.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hnxiangtu.top/gtnaehxbni.html

[U75] PHP：依赖注入
来源：http://hz.52xcode.cn/gthcidwncs.html

composer require psr/container
来源：http://hz.zhijiandao.cn/gtotguaohs.html

[U76] PHP：简单路由
来源：http://hz.hongshengwenyu.top/gtbrrsrgrb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.meibo888.top/gtfbtqddgr.html

[U77] PHP：模板渲染
来源：http://hz.sweek.top/gtbsqcmqyd.html

composer require twig/twig
来源：http://hz.haohaochexian.top/gtiwulgqjy.html

[U78] PHP：单元测试
来源：http://hz.yuxming.cn/gtweablhvx.html

composer require --dev phpunit/phpunit
来源：http://hz.dashuyun.cn/gtbgpptdeb.html

[U79] PHP：静态分析
来源：http://hz.xuanzx.com/gtgefpwfxp.html

composer require --dev phpstan/phpstan
来源：http://hz.pengpengdd.cyou/gtlibplikw.html

[U80] PHP：代码规范修复
来源：http://hz.jlsjyb.cn/gtcytznsfp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.cdnleiting.top/gtckvuuuvi.html

[U81] JS：初始化项目
来源：http://hz.jqgfzy.top/gtyxnenabx.html

npm init -y;  npm i express
来源：http://hz.ppjwa.cn/gtyhxltihh.html

[U82] JS：package.json 脚本
来源：http://hz.tianlin.xyz/gtaoayjinu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.0kj1m.cn/gtuhogfohl.html


<!-- 参考信息 -->