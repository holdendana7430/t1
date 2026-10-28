代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yueranfly.top/gtqbwvvqeo.html

[S57] C++：编译期常量
来源：http://hz.nwbrower.top/gtfbnbmqni.html

constexpr int N = 10;
来源：http://hz.cqqwz.cn/gtexwwevrt.html

[S58] C++：命名空间
来源：http://hz.jinqigufen.top/gtwvijtkdi.html

namespace ns { int f() { return 1; } }
来源：http://hz.c1oappe.top/gtrcssubtg.html

[S59] C++：静态断言
来源：http://hz.shzxlz.cn/gtujehvuzf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yuxming.cn/gtalmvbnkq.html

[S60] C++：遍历并删除元素
来源：http://hz.redwolf501.top/gtqugyzoqq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.vqdsnc.cn/gthxuicogw.html

================================================================================
来源：http://hz.snrcjt.cn/gttvavjzre.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinghuilouyu.cn/gtpmoucwgp.html

================================================================================
来源：http://hz.jianghu66.top/gtgrhencra.html

[T01] Kotlin：Hello World
来源：http://hz.yongpay.top/gtmgodfbsl.html

println("Hello")
来源：http://hz.gotoacloud.top/gtzcssclai.html

[T02] Kotlin：变量
来源：http://hz.9152youxi.cn/gtdsnoxnxm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgfzy.top/gtrruaxnhv.html

[T03] Kotlin：字符串模板
来源：http://hz.dianchejie.cn/gthywnjbfn.html

"值: $b"
来源：http://hz.gaohongyu789.top/gtntxucsat.html

[T04] Kotlin：空安全
来源：http://hz.jinqigufen.top/gtyefrovns.html

val n: String? = null;  n?.length
来源：http://hz.yuanzhike.top/gtbdvawpoo.html

[T05] Kotlin：when 表达式
来源：http://hz.dashuyun.cn/gtztcrujkc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xingfuxueyuan.xyz/gtqbonsfkm.html

[T06] Kotlin：集合映射
来源：http://hz.nwbrower.top/gtlfvxgsxb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinqigufen.top/gtmvdesqzi.html

[T07] Kotlin：集合过滤
来源：http://hz.316326.xyz/gtrzbpsmmd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhixingplan.top/gtjudjblbm.html

[T08] Kotlin：数据类
来源：http://hz.wangdashe.top/gtfqwqsiax.html

data class User(val name: String, val age: Int)
来源：http://hz.yanxiufei.cn/gtaknjjajf.html

[T09] Kotlin：扩展函数
来源：http://hz.zhengqikj.top/gtcbhjxtkn.html

fun String.exclaim() = this + "!"
来源：http://hz.jianghu66.top/gtjmxcpozh.html

[T10] Kotlin：默认参数
来源：http://hz.jinyuanbaomall.cn/gtaoanlzmo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.chenlongwang.top/gtvqusddbu.html

[T11] Kotlin：协程
来源：http://hz.xuanzx.com/gtmlerjrmn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhiwuduotai.top/gttauuepfp.html

[T12] Kotlin：解构声明
来源：http://hz.quarkkingdee.top/gtrnzomvpo.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuxming.cn/gtfvpmkfls.html

[T13] Kotlin：只读 Map
来源：http://hz.yuxming.cn/gtsbpsgmzo.html

val m = mapOf("a" to 1)
来源：http://hz.iojbl.cn/gtucacbpvw.html

[T14] Kotlin：循环
来源：http://hz.hongshengwenyu.top/gtsgttbbiy.html

for (i in 1..10) println(i)
来源：http://hz.xylfe.cn/gtfwvprvpy.html

[T15] Kotlin：接口
来源：http://hz.pengpengdd.cyou/gtobvgllhi.html

interface Shape { fun area(): Double }
来源：http://hz.feifeiyinyue.top/gtkxuqqeyp.html

[T16] Swift：Hello World
来源：http://hz.yuanzhike.top/gtbjheydtr.html

print("Hello")
来源：http://hz.yongpay.top/gtbjgqlwhk.html

[T17] Swift：变量与常量
来源：http://hz.xinyue.icu/gtkdcatqzw.html

var a = 1;  let b = 2
来源：http://hz.c1oappe.top/gtnjkzbofb.html

[T18] Swift：字符串插值
来源：http://hz.gaohongyu789.top/gtynbuumei.html

"值: \(b)"
来源：http://hz.jinqigufen.top/gtlvtjbech.html

[T19] Swift：可选绑定
来源：http://hz.jinyuanbaomall.cn/gtvnzodjqy.html

if let n = opt { print(n) }
来源：http://hz.guowangkeji.top/gthaayfcke.html

[T20] Swift：数组操作
来源：http://hz.guannengcc.top/gtjmnwzknt.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yuxming.cn/gtaybwyoep.html

[T21] Swift：遍历
来源：http://hz.c1oappe.top/gtmsjeetol.html

for x in a { print(x) }
来源：http://hz.feifeiyinyue.top/gtiteequyx.html

[T22] Swift：字典
来源：http://hz.zhijiandao.cn/gtrkytptzp.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinqigfzy.top/gtxdoozibo.html

[T23] Swift：函数
来源：http://hz.meibo888.top/gtbelsrwyq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.guowangkeji.top/gtydcirgco.html

[T24] Swift：闭包
来源：http://hz.9152youxi.cn/gtiocisrss.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ydjk.org.cn/gtjrdnlghg.html

[T25] Swift：结构体
来源：http://hz.yj202588.top/gttkgdtlvn.html

struct P { var x: Int }
来源：http://hz.guannengcc.top/gtrkuymjrg.html

[T26] Swift：类与重写
来源：http://hz.jqgufenzy.top/gthlyvlcwq.html

class A: Base { override func f() {} }
来源：http://hz.quarkkingdee.top/gtycaquwfw.html

[T27] Swift：错误处理
来源：http://hz.cheryme.top/gteucoejov.html

do { try f() } catch { print(error) }
来源：http://hz.pengpengdd.cyou/gtnaeultjq.html

[T28] Swift：枚举
来源：http://hz.jqgfzy.top/gtlahurugk.html

enum Color { case red, green }
来源：http://hz.hnxiangtu.top/gtttyeipjo.html

[T29] Swift：guard 提前返回
来源：http://hz.yuanzhike.top/gttqcnsufj.html

guard let x = opt else { return }
来源：http://hz.nanxinkj.top/gtwqapftbx.html

[T30] Swift：协议
来源：http://hz.ppjwa.cn/gtkvcuxysw.html

protocol Shape { func area() -> Double }
来源：http://hz.sysykeji.top/gtriytmzob.html

[T31] Lua：Hello World
来源：http://hz.gogol.net.cn/gtqhsyvndg.html

print("Hello")
来源：http://hz.zhiwuduotai.top/gtoobusgmk.html

[T32] Lua：局部变量
来源：http://hz.zhaomingkeji.xyz/gtognpfohz.html

local a = 1
来源：http://hz.sufxvd.cn/gtpitdhsya.html

[T33] Lua：表（数组）
来源：http://hz.xuanzx.com/gtfyhwoqqy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj20258888.top/gtbhhfxles.html

[T34] Lua：遍历表
来源：http://hz.sysykeji.top/gtgwmzvjry.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.shangyingyoupin.top/gtpvytnvdm.html

[T35] Lua：字典表
来源：http://hz.chenjidiqi.icu/gtewvazbni.html

local d = { a = 1 };  d.b = 2
来源：http://hz.haohaochexian.top/gtqbsyzrki.html

[T36] Lua：函数
来源：http://hz.yvedp.cn/gtpzlinkov.html

function add(a, b) return a + b end
来源：http://hz.xylfe.cn/gtaewtggor.html

[T37] Lua：字符串拼接
来源：http://hz.mhx1999.top/gtwmbfzhcp.html

"a" .. "b"
来源：http://hz.gotoacloud.top/gthoczwbxf.html

[T38] Lua：条件
来源：http://hz.shanyushiyangtech.top/gtdylsctoh.html

if x > 0 then print("正") end
来源：http://hz.hnxiangtu.top/gttlubnkbr.html

[T39] Lua：模式匹配
来源：http://hz.birdmap.top/gtibwijwfb.html

string.find(s, "%d+")
来源：http://hz.52xcode.cn/gtcixefqin.html

[T40] Lua：元表
来源：http://hz.cucudq.cn/gtwyjtanjy.html

setmetatable({}, { __index = base })
来源：http://hz.ppjwa.cn/gtdzmoxsvb.html

[T41] Perl：Hello World
来源：http://hz.yongpay.top/gtwrvecurz.html

print "Hello\n";
来源：http://hz.shzxlz.cn/gtmpmtttgz.html

[T42] Perl：变量类型
来源：http://hz.jlsjyb.cn/gtlzaucuir.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gaohongyu789.top/gttbtsuuwl.html

[T43] Perl：字符串插值
来源：http://hz.hywenlv.cn/gtnjiizsmb.html

"值: $a"
来源：http://hz.redwolf501.top/gtzgloronz.html

[T44] Perl：条件
来源：http://hz.mhx1999.top/gttbtwelnh.html

if ($a > 0) { print "正"; }
来源：http://hz.snrcjt.cn/gtehixlwez.html

[T45] Perl：数组遍历
来源：http://hz.bjfxy.top/gtflqjexbo.html

for my $x (@arr) { print $x; }
来源：http://hz.sysykeji.top/gtbxzfgreg.html

[T46] Perl：哈希操作
来源：http://hz.havefunace.top/gtwlrhlzza.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.hammf.cn/gtfkwzhmul.html

[T47] Perl：正则捕获
来源：http://hz.cashguo.top/gtbhtwyeez.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.kuanghao11.cn/gtczyehnei.html

[T48] Perl：正则替换
来源：http://hz.guowangkeji.top/gtduvbizld.html

$s =~ s/old/new/g;
来源：http://hz.yuxming.cn/gtmjevtdju.html

[T49] Perl：函数
来源：http://hz.jqgfzy.top/gtgpsnuxxc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.52xcode.cn/gtplvnyuai.html

[T50] Perl：逐行读文件
来源：http://hz.52xcode.cn/gttjfmzazz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.dianchejie.cn/gtpqmmemwe.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhaomingkeji.xyz/gtzaakrsgy.html

[T51] Scala：Hello World
来源：http://hz.shzxlz.cn/gtrbomzzop.html

println("Hello")
来源：http://hz.sweek.top/gtmdfhgvma.html

[T52] Scala：变量
来源：http://hz.chenlongwang.top/gtchupuyyn.html

val a = 1;  var b = 2
来源：http://hz.ydzc1.top/gtrihuxomq.html

[T53] Scala：字符串插值
来源：http://hz.pengpengdd.cyou/gtddfqgdzg.html

s"值: $b"
来源：http://hz.ydjk.org.cn/gtfwsjgouc.html

[T54] Scala：集合映射
来源：http://hz.gotoacloud.top/gtermqbywb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.jinqigufen.top/gtdkhdnwyv.html

[T55] Scala：集合过滤
来源：http://hz.jinqigufen.top/gtnmqghmos.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.xinyue.icu/gtfhmoiqti.html

[T56] Scala：样例类
来源：http://hz.zhijiandao.cn/gtwmiodmim.html

case class User(name: String, age: Int)
来源：http://hz.nwbrower.top/gtsmiswhnr.html

[T57] Scala：模式匹配
来源：http://hz.0kj1m.cn/gtnprnttuu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.gzhubu.top/gtebovmapy.html

[T58] Scala：函数定义
来源：http://hz.redwolf501.top/gtmagdsrcq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhiwuduotai.top/gteyapsjad.html

[T59] Scala：循环
来源：http://hz.yangfankeji.com/gtdazpdrhc.html

for (i <- 1 to 10) println(i)
来源：http://hz.shanyushiyangkeji.top/gtarvoxrhj.html

[T60] Scala：折叠
来源：http://hz.tanke756.top/gtvtuvzbuz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jyoumei.cn/gtfiecmetu.html

================================================================================
来源：http://hz.bjfxy.top/gtmdxyrzqv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.chenjidiqi.icu/gtsbsjjoug.html

================================================================================
来源：http://hz.yonumen.top/gtcyyspotn.html

[U01] Py：创建虚拟环境
来源：http://hz.cheryme.top/gtafkjaveu.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.sufxvd.cn/gthowimctb.html

[U02] Py：导出 / 安装依赖
来源：http://hz.jianghu66.top/gtyklndnsn.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.yangfankeji.com/gtdzsownvd.html

[U03] Py：加载 .env 配置
来源：http://hz.zhaomingkeji.xyz/gtxlndxast.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.jqgfzy.top/gtrkwigyjt.html

[U04] Py：变量调试打印
来源：http://hz.yueranfly.top/gtaanoxsmj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.yj20258.top/gtqanzhyus.html

[U05] Py：列表去重且保序
来源：http://hz.bjfxy.top/gtnakpjtwe.html

list(dict.fromkeys(arr))
来源：http://hz.fzhhl.top/gtyvlqvypp.html

[U06] Py：合并两个字典
来源：http://hz.jiagoushi.top/gtwjdculht.html

{**a, **b}
来源：http://hz.dianchejie.cn/gtzkgoljud.html

[U07] Py：反转字典键值
来源：http://hz.nanxuanxn.top/gthditcmop.html

{v: k for k, v in d.items()}
来源：http://hz.zhoulong.xyz/gtdnkcuonj.html

[U08] Py：展平二维列表
来源：http://hz.ppjwa.cn/gtyhkomaql.html

[y for x in nested for y in x]
来源：http://hz.ybcxt.top/gtzzwdjzip.html

[U09] Py：字典取最大值的键
来源：http://hz.yvedp.cn/gtfhhpnmgo.html

max(d, key=d.get)
来源：http://hz.ydzc1.top/gtcpickatp.html

[U10] Py：按值排序字典
来源：http://hz.ydjk.org.cn/gtfgvcdkik.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.jinqigfzy.top/gttuodvonm.html

[U11] Py：生成器表达式
来源：http://hz.ybcxt.top/gtzgblfcfd.html

(x * 2 for x in arr)
来源：http://hz.yj20258888.top/gtrbusyomh.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yuanzhike.top/gtbsrqqxqr.html

Counter(arr).most_common(3)
来源：http://hz.zhiwuduotai.top/gthoqbqcav.html

[U13] Py：固定长度队列
来源：http://hz.sufxvd.cn/gtytefxutj.html

deque(maxlen=10)
来源：http://hz.hywenlv.cn/gtuogrpqkd.html

[U14] Py：分组收集到列表
来源：http://hz.pycfn.com/gteknsjftn.html

defaultdict(list)
来源：http://hz.nwbrower.top/gthoypqcxf.html

[U15] Py：高精度计时
来源：http://hz.redwolf501.top/gtsezmgxzx.html

t = time.perf_counter()
来源：http://hz.cqqwz.cn/gtxmhujetb.html

[U16] Py：命令行参数解析
来源：http://hz.meibo888.top/gtnmtoepzo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.gaohongyu789.top/gtgmaldnsv.html

[U17] Py：初始化日志
来源：http://hz.52xcode.cn/gtugdmcqmq.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenlongwang.top/gtigfevzyi.html

[U18] Py：预编译正则
来源：http://hz.ehwqpu.com/gtrieimgph.html

pat = re.compile(r"\d+")
来源：http://hz.ydjk.org.cn/gtfcjffbyz.html

[U19] Py：正则替换带回调
来源：http://hz.cdnleiting.top/gtxshxnyxa.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yj202588.top/gtkfcrjepi.html

[U20] Py：缓存函数结果
来源：http://hz.birdmap.top/gtkijeiowf.html

@functools.lru_cache(maxsize=None)
来源：http://hz.nanxinkj.top/gtbamdikne.html

[U21] Py：自定义上下文管理器
来源：http://hz.shanyushiyangtech.top/gtuoxabumv.html

@contextlib.contextmanager
来源：http://hz.jinyuanbaomall.cn/gtvyicmmra.html

[U22] Py：矩阵转置
来源：http://hz.nwbrower.top/gtyleyfdpq.html

list(zip(*m))
来源：http://hz.nanxuanxn.top/gtznuslvft.html

[U23] Py：分块读取大文件
来源：http://hz.yueranfly.top/gtstxwkjdz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.yj202588.top/gtnrytvgpi.html

[U24] Py：路径操作
来源：http://hz.tianlin.xyz/gtsmdlqdgy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.jqgfzy.top/gtqsitphqo.html

[U25] Py：CSV 按字典读
来源：http://hz.jqgufenzy.top/gtgodadflp.html

csv.DictReader(f)
来源：http://hz.shangyingyoupin.top/gtqhfenppy.html

[U26] Py：并发下载
来源：http://hz.havefunace.top/gtkcrmdwpq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.tanke756.top/gtxgmfhxmq.html

[U27] Py：异步 HTTP
来源：http://hz.jinghuilouyu.cn/gtjvarpavl.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.shanyushiyangtech.top/gtzvhmdlwu.html

[U28] Py：类型别名
来源：http://hz.tianlin.xyz/gtvnctcicy.html

UserId = int
来源：http://hz.hnqzz.top/gtpefffxzm.html

[U29] Py：属性校验
来源：http://hz.jqgufenzy.top/gtixlksink.html

@property 与 @x.setter 配合
来源：http://hz.jinghuilouyu.cn/gtjtrfseiu.html

[U30] Py：数据类
来源：http://hz.shanyushiyangkeji.top/gtstkatqea.html

@dataclass(slots=True)
来源：http://hz.sxryk.cn/gtgiavrdzd.html

[U31] Py：单测
来源：http://hz.chenlongwang.top/gtczqqzakb.html

python -m pytest -q
来源：http://hz.hnqzz.top/gtjkiwqlwe.html

[U32] Py：代码格式化
来源：http://hz.gogol.net.cn/gtxwaihvjw.html

ruff format . && ruff check --fix .
来源：http://hz.andypj.xyz/gtyllvxxnd.html

[U33] Py：打包发布
来源：http://hz.cucudq.cn/gtrinifmxj.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.hysaishi.cn/gtmdwvjgko.html

[U34] Py：判断编码
来源：http://hz.ydjk.org.cn/gtmrtapkqs.html

chardet.detect(raw)
来源：http://hz.jinghuilouyu.cn/gttojpowjk.html

[U35] Py：发送邮件
来源：http://hz.fengsongda.top/gtwwziopnz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.sysykeji.top/gtvipussqf.html

[U36] Py：定时任务
来源：http://hz.wangdashe.top/gttdconyfy.html

schedule.every(10).minutes.do(job)
来源：http://hz.ppjwa.cn/gtkquaotfm.html

[U37] Py：读写 Excel
来源：http://hz.jyoumei.cn/gtbuurfent.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.tian-w.cn/gtvvfgehxc.html

[U38] Py：获取脚本所在目录
来源：http://hz.dianchejie.cn/gtfkmxudie.html

Path(__file__).resolve().parent
来源：http://hz.hongshengwenyu.top/gtfupycrtu.html

[U39] Py：判断是否在交互环境
来源：http://hz.redwolf501.top/gtdncminbv.html

sys.stdout.isatty()
来源：http://hz.jiagoushi.top/gtgefbbzxc.html

[U40] Py：打印到标准错误
来源：http://hz.316326.xyz/gtolxborvo.html

print("err", file=sys.stderr)
来源：http://hz.316326.xyz/gtzjvaqbrm.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.jinqigfzy.top/gtfcnnnfwo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.ybcxt.top/gtpmufaasm.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.xuetiantiany.cn/gtqazatslb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhongyouzk.top/gtqfzxswgv.html

[U43] PHP：声明命名空间
来源：http://hz.chenlongwang.top/gtxwcygarz.html

namespace App\Http;
来源：http://hz.jinqigufen.top/gthrqodork.html

[U44] PHP：开启严格类型
来源：http://hz.pengpengdd.cyou/gtvtqhjykq.html

declare(strict_types=1);
来源：http://hz.svipenyu.cn/gtddwwtxdn.html

[U45] PHP：类型声明与返回类型
来源：http://hz.cashguo.top/gtslguiblq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gthnztmrgn.html

[U46] PHP：可空类型
来源：http://hz.yongpay.top/gtpuajvaoe.html

?string $name = null
来源：http://hz.chenzaomai.com/gtaprzshjz.html

[U47] PHP：联合类型
来源：http://hz.chenzaomai.com/gtaqarhmnj.html

int|string $id
来源：http://hz.shangyingyoupin.top/gtsuzibeyu.html

[U48] PHP：纯枚举
来源：http://hz.chenzaomai.com/gtqsuppcvr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.hnxiangtu.top/gtslejbugp.html

[U49] PHP：只读属性
来源：http://hz.9152youxi.cn/gtdhsnlaci.html

public readonly string $name
来源：http://hz.zhongyouzk.top/gtuwnmmdjc.html

[U50] PHP：构造器属性提升
来源：http://hz.yonumen.top/gtwmlpiquq.html

public function __construct(private int $id) {}
来源：http://hz.xingfuxueyuan.xyz/gtgivxqxnh.html

[U51] PHP：数组解构
来源：http://hz.jinyuanbaomall.cn/gtjpkdhqnq.html

[$a, $b] = $arr;
来源：http://hz.zhijiandao.cn/gtnfgaivqc.html

[U52] PHP：箭头函数
来源：http://hz.yonumen.top/gtcszzgvnr.html

$double = fn($x) => $x * 2;
来源：http://hz.hnqzz.top/gtqleooeiw.html

[U53] PHP：空合并运算符
来源：http://hz.yanxiufei.cn/gtqthhtkjj.html

$v = $a ?? $b ?? "default";
来源：http://hz.yongpay.top/gtvsiavbrj.html

[U54] PHP：空安全调用
来源：http://hz.snrcjt.cn/gtwcuurgat.html

$obj?->method()
来源：http://hz.sysykeji.top/gtgqfluicg.html

[U55] PHP：match 表达式
来源：http://hz.zdqjudy.top/gtvpkizhbc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.birdmap.top/gtzenjdgxi.html

[U56] PHP：命名参数
来源：http://hz.wangshuangyany.cn/gttjzojdsp.html

f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtmcwjmjrd.html

[U57] PHP：字符串插值
来源：http://hz.redwolf501.top/gtzyfscgsg.html

"值: {$a}"
来源：http://hz.tianlin.xyz/gtfxvdprvm.html

[U58] PHP：数组三件套
来源：http://hz.zhijiandao.cn/gtkooeydxg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.jinyuanbaomall.cn/gtzchzendm.html

[U59] PHP：自定义排序
来源：http://hz.ivvv.top/gtdhzuvitn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinghuilouyu.cn/gtrvyesbog.html

[U60] PHP：JSON 编解码
来源：http://hz.xingfuxueyuan.xyz/gtjajabnpx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhongyouzk.top/gthpcoeeho.html

[U61] PHP：正则
来源：http://hz.mhx1999.top/gtfjzsdbtw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydzc1.top/gtiegfmcls.html

[U62] PHP：日期对象
来源：http://hz.jqgufenzy.top/gtzetglgdl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.nanxinkj.top/gtydnliksx.html

[U63] PHP：文件读写
来源：http://hz.ivvv.top/gtcwbizalj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.guowangkeji.top/gtrecpkykt.html

[U64] PHP：目录遍历
来源：http://hz.zhoulong.xyz/gtiwcnzzzz.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.sufxvd.cn/gtoioruetu.html

[U65] PHP：会话
来源：http://hz.xylfe.cn/gtbqftzlnm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.pengpengdd.cyou/gtgigxweag.html

[U66] PHP：设置 Cookie
来源：http://hz.cdnleiting.top/gtpnwjvsmy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.fengsongda.top/gtmgbuuchl.html

[U67] PHP：处理文件上传
来源：http://hz.yj202588.top/gtlumeupkt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.jyoumei.cn/gtpjwlpiks.html

[U68] PHP：PDO 连接
来源：http://hz.shzxlz.cn/gtvfuiywqt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shzxlz.cn/gtrbcxyuhg.html

[U69] PHP：PDO 预处理
来源：http://hz.svipenyu.cn/gtceygoaty.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.dianchejie.cn/gtxtvvhxnv.html

[U70] PHP：PDO 事务
来源：http://hz.hnqzz.top/gtjdessesh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.meibo888.top/gtrlyoiydk.html

[U71] PHP：抛出异常
来源：http://hz.sysykeji.top/gtqllicmby.html

throw new RuntimeException("失败", 500);
来源：http://hz.pengpengdd.cyou/gtycgggixn.html

[U72] PHP：写错误日志
来源：http://hz.daxiang520.top/gtpcqioaop.html

error_log("失败: " . $e->getMessage());
来源：http://hz.snrcjt.cn/gtkyybllet.html

[U73] PHP：读取 ini 配置
来源：http://hz.shanyushiyangkeji.top/gtteqczsbo.html

parse_ini_file("config.ini", true)
来源：http://hz.jinyuanbaomall.cn/gtytpojdvj.html

[U74] PHP：读取环境变量
来源：http://hz.cqqwz.cn/gtbigikemt.html

getenv("APP_ENV") ?: "production"
来源：http://hz.hongshengwenyu.top/gtaxbqhrey.html

[U75] PHP：依赖注入
来源：http://hz.bjfxy.top/gterchwpxe.html

composer require psr/container
来源：http://hz.zhiwuduotai.top/gtmoarazne.html

[U76] PHP：简单路由
来源：http://hz.mhx1999.top/gttfrwbptj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.9152youxi.cn/gtedsavcad.html

[U77] PHP：模板渲染
来源：http://hz.52xcode.cn/gtbtysqizz.html

composer require twig/twig
来源：http://hz.wangshuangyany.cn/gtsktrvdod.html

[U78] PHP：单元测试
来源：http://hz.chenjidiqi.icu/gtnzecdbpf.html

composer require --dev phpunit/phpunit
来源：http://hz.cucudq.cn/gtxsuhsisw.html

[U79] PHP：静态分析
来源：http://hz.meibo888.top/gtuhrfnjdh.html

composer require --dev phpstan/phpstan
来源：http://hz.gzhubu.top/gtexaegltc.html

[U80] PHP：代码规范修复
来源：http://hz.yvedp.cn/gtnywslwsy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shzxlz.cn/gtlclpgxpw.html

[U81] JS：初始化项目
来源：http://hz.yj202588.top/gtctgdomty.html

npm init -y;  npm i express
来源：http://hz.9152youxi.cn/gtsokxrvfe.html

[U82] JS：package.json 脚本
来源：http://hz.gzhubu.top/gtcltrlyml.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.xylfe.cn/gttprcxcol.html


<!-- 参考信息 -->