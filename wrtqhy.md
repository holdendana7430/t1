代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://hz.cucudq.cn/gtlsegagcl.html

[S59] C++：静态断言
来源：http://hz.zycfv.cn/gtthbvduuv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hammf.cn/gtszmzsohu.html

[S60] C++：遍历并删除元素
来源：http://hz.kuanghao11.cn/gteqnzpcnk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenjidiqi.icu/gtyahfiinm.html

================================================================================
来源：http://hz.smart0.xyz/gtxftvvgec.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guowangkeji.top/gtqixbqhmy.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtaympngcr.html

[T01] Kotlin：Hello World
来源：http://hz.shzxlz.cn/gtahtqhtej.html

println("Hello")
来源：http://hz.shzxlz.cn/gtblxurctz.html

[T02] Kotlin：变量
来源：http://hz.shuidangran.top/gtpwxafnjj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.meibo888.top/gtemnhnead.html

[T03] Kotlin：字符串模板
来源：http://hz.dashuyun.cn/gtjsftetnw.html

"值: $b"
来源：http://hz.jinqigfzy.top/gtzwfanbsp.html

[T04] Kotlin：空安全
来源：http://hz.zhaomingkeji.xyz/gtrbxzzmdx.html

val n: String? = null;  n?.length
来源：http://hz.yongpay.top/gtjjczlcnf.html

[T05] Kotlin：when 表达式
来源：http://hz.zycfv.cn/gtgeftbpat.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cucudq.cn/gtuvslejvw.html

[T06] Kotlin：集合映射
来源：http://hz.yuxming.cn/gttokjoauz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.quarkkingdee.top/gtdtperziq.html

[T07] Kotlin：集合过滤
来源：http://hz.bjfxy.top/gtksglrjkx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tanke756.top/gtviyxtxsv.html

[T08] Kotlin：数据类
来源：http://hz.jinyuanbaomall.cn/gtakuynqbv.html

data class User(val name: String, val age: Int)
来源：http://hz.jianghu66.top/gtpbcjbcqe.html

[T09] Kotlin：扩展函数
来源：http://hz.jiagoushi.top/gtkvpqlbad.html

fun String.exclaim() = this + "!"
来源：http://hz.cheryme.top/gtdiowrwin.html

[T10] Kotlin：默认参数
来源：http://hz.xuetiantiany.cn/gtnwteznlj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zdqjudy.top/gttgyamotv.html

[T11] Kotlin：协程
来源：http://hz.guannengcc.top/gtcqtugbkl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.c1oappe.top/gtiopqkwqu.html

[T12] Kotlin：解构声明
来源：http://hz.tian-w.cn/gtossmeenz.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuanzhike.top/gtawfswzbj.html

[T13] Kotlin：只读 Map
来源：http://hz.mhx1999.top/gtudbuoibv.html

val m = mapOf("a" to 1)
来源：http://hz.yanxiufei.cn/gttiokgyex.html

[T14] Kotlin：循环
来源：http://hz.shangyingyoupin.top/gtwrneadkv.html

for (i in 1..10) println(i)
来源：http://hz.quarkkingdee.top/gtnzgmltbk.html

[T15] Kotlin：接口
来源：http://hz.wangdashe.top/gtqgwgukta.html

interface Shape { fun area(): Double }
来源：http://hz.cheryme.top/gtoeaurzkn.html

[T16] Swift：Hello World
来源：http://hz.jianghu66.top/gtkqxdywjl.html

print("Hello")
来源：http://hz.ppjwa.cn/gtxmyhzfjs.html

[T17] Swift：变量与常量
来源：http://hz.sweek.top/gtahjhtgxl.html

var a = 1;  let b = 2
来源：http://hz.dianchejie.cn/gtqndfqhso.html

[T18] Swift：字符串插值
来源：http://hz.sysykeji.top/gtpbhgxrgm.html

"值: \(b)"
来源：http://hz.svipenyu.cn/gtvwtrtbae.html

[T19] Swift：可选绑定
来源：http://hz.cqqwz.cn/gtwzfxtnnv.html

if let n = opt { print(n) }
来源：http://hz.fzhhl.top/gtvmqdhifn.html

[T20] Swift：数组操作
来源：http://hz.ydzc1.top/gtegndguky.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yueranfly.top/gtiekjfilz.html

[T21] Swift：遍历
来源：http://hz.feifeiyinyue.top/gtzvjbiagw.html

for x in a { print(x) }
来源：http://hz.hysaishi.cn/gtfqybfqwp.html

[T22] Swift：字典
来源：http://hz.nanxuanxn.top/gtegcxemux.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.guannengcc.top/gtmibyibdc.html

[T23] Swift：函数
来源：http://hz.cashguo.top/gtojrrnjrl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xylfe.cn/gtledinkgj.html

[T24] Swift：闭包
来源：http://hz.smart0.xyz/gtobxmlgpc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuanzhike.top/gthkwvejvb.html

[T25] Swift：结构体
来源：http://hz.chenzaomai.com/gtjibkkqgf.html

struct P { var x: Int }
来源：http://hz.vqdsnc.cn/gtiglilpeb.html

[T26] Swift：类与重写
来源：http://hz.hnqzz.top/gttrmougxx.html

class A: Base { override func f() {} }
来源：http://hz.bjfxy.top/gtplgipjij.html

[T27] Swift：错误处理
来源：http://hz.jinqigufen.top/gtfgphcqaq.html

do { try f() } catch { print(error) }
来源：http://hz.wangdashe.top/gthpxuswnh.html

[T28] Swift：枚举
来源：http://hz.jqgufenzy.top/gtvnqidsqm.html

enum Color { case red, green }
来源：http://hz.jyoumei.cn/gthprhtjoe.html

[T29] Swift：guard 提前返回
来源：http://hz.shuidangran.top/gthqlnnhni.html

guard let x = opt else { return }
来源：http://hz.hongshengwenyu.top/gtolbckgml.html

[T30] Swift：协议
来源：http://hz.zhoulong.xyz/gtnvdrgabe.html

protocol Shape { func area() -> Double }
来源：http://hz.feifeiyinyue.top/gtycelosoq.html

[T31] Lua：Hello World
来源：http://hz.gogol.net.cn/gtwsauaqwg.html

print("Hello")
来源：http://hz.zhongyouzk.top/gtxvxmuqgo.html

[T32] Lua：局部变量
来源：http://hz.yangfankeji.com/gtacmuhnmu.html

local a = 1
来源：http://hz.jqgufenzy.top/gtcwcmphda.html

[T33] Lua：表（数组）
来源：http://hz.daria6918.cn/gttjdanyiw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shangyingyoupin.top/gtptxwvfgp.html

[T34] Lua：遍历表
来源：http://hz.zhaomingkeji.xyz/gtvhtuqsdo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xuetiantiany.cn/gtjevpkmvv.html

[T35] Lua：字典表
来源：http://hz.aibaodan.cn/gtwhtvxafg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.quarkkingdee.top/gtspewjdkc.html

[T36] Lua：函数
来源：http://hz.gaohongyu789.top/gtzspgogpl.html

function add(a, b) return a + b end
来源：http://hz.smart0.xyz/gtypibxpny.html

[T37] Lua：字符串拼接
来源：http://hz.ivvv.top/gtdgqrnuct.html

"a" .. "b"
来源：http://hz.gzhubu.top/gthzbsvklh.html

[T38] Lua：条件
来源：http://hz.zhaomingkeji.xyz/gtjfcrcwmv.html

if x > 0 then print("正") end
来源：http://hz.yj20258888.top/gtcvlucxam.html

[T39] Lua：模式匹配
来源：http://hz.tian-w.cn/gtaxivhdvz.html

string.find(s, "%d+")
来源：http://hz.yj20258.top/gthazmrebw.html

[T40] Lua：元表
来源：http://hz.cdnleiting.top/gtymkaiqil.html

setmetatable({}, { __index = base })
来源：http://hz.sxryk.cn/gttmrlamsj.html

[T41] Perl：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtjawcwoni.html

print "Hello\n";
来源：http://hz.xylfe.cn/gtvccfxfaq.html

[T42] Perl：变量类型
来源：http://hz.feifeiyinyue.top/gtgpcpziih.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.shanyushiyangkeji.top/gtnvdopjgc.html

[T43] Perl：字符串插值
来源：http://hz.jianghu66.top/gtselpfyjv.html

"值: $a"
来源：http://hz.guowangkeji.top/gtoesygmjr.html

[T44] Perl：条件
来源：http://hz.xylfe.cn/gtjwgcalkc.html

if ($a > 0) { print "正"; }
来源：http://hz.gogol.net.cn/gtmpwkyklo.html

[T45] Perl：数组遍历
来源：http://hz.smart0.xyz/gtlhihclfm.html

for my $x (@arr) { print $x; }
来源：http://hz.cheryme.top/gtckgjsjyl.html

[T46] Perl：哈希操作
来源：http://hz.xuanzx.com/gtnmotuuay.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yj202588.top/gtixezfdww.html

[T47] Perl：正则捕获
来源：http://hz.chenzaomai.com/gtvxwtgmzr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xylfe.cn/gtzhcpgjzw.html

[T48] Perl：正则替换
来源：http://hz.smart0.xyz/gtjxzaavuh.html

$s =~ s/old/new/g;
来源：http://hz.xinyue.icu/gtmujphrbn.html

[T49] Perl：函数
来源：http://hz.sweek.top/gtwesmvhqw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nanxuanxn.top/gtntesirse.html

[T50] Perl：逐行读文件
来源：http://hz.cucudq.cn/gtcvnincqt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yuanzhike.top/gtsraulwhj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cucudq.cn/gtewyhcpbl.html

[T51] Scala：Hello World
来源：http://hz.chenjidiqi.icu/gtdqblzbef.html

println("Hello")
来源：http://hz.chenjidiqi.icu/gtlpmpbjnf.html

[T52] Scala：变量
来源：http://hz.cheryme.top/gtvhusckty.html

val a = 1;  var b = 2
来源：http://hz.yj20258.top/gtfbfgimcb.html

[T53] Scala：字符串插值
来源：http://hz.jinyuanbaomall.cn/gtogyzsrms.html

s"值: $b"
来源：http://hz.iojbl.cn/gtatmyzwxh.html

[T54] Scala：集合映射
来源：http://hz.yuxming.cn/gtvaxnjsck.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.tian-w.cn/gtwnnorjjg.html

[T55] Scala：集合过滤
来源：http://hz.c1oappe.top/gtqahpppru.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ehwqpu.com/gtogirbnfp.html

[T56] Scala：样例类
来源：http://hz.shanyushiyangkeji.top/gtumutcqcy.html

case class User(name: String, age: Int)
来源：http://hz.yanxiufei.cn/gttcehdpjq.html

[T57] Scala：模式匹配
来源：http://hz.jianghu66.top/gtywznooww.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.kuanghao11.cn/gtooayxzmz.html

[T58] Scala：函数定义
来源：http://hz.tianlin.xyz/gtssybqgwh.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.shangyingyoupin.top/gtwwgdgpmx.html

[T59] Scala：循环
来源：http://hz.zhijiandao.cn/gtxvjrvoqi.html

for (i <- 1 to 10) println(i)
来源：http://hz.jqgufenzy.top/gtzfayfdbc.html

[T60] Scala：折叠
来源：http://hz.guowangkeji.top/gtvllovvch.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.jqgfzy.top/gtfduhgkrm.html

================================================================================
来源：http://hz.nwbrower.top/gtozgfoyow.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigufen.top/gtkbfdyclt.html

================================================================================
来源：http://hz.0kj1m.cn/gtzjepppwn.html

[U01] Py：创建虚拟环境
来源：http://hz.zycfv.cn/gtacpiskrj.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.hammf.cn/gtayvjybpi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.quarkkingdee.top/gtowcreity.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.hywenlv.cn/gtbihriehf.html

[U03] Py：加载 .env 配置
来源：http://hz.andypj.xyz/gtmgogvcdr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shangyingyoupin.top/gtnrspypyl.html

[U04] Py：变量调试打印
来源：http://hz.ybcxt.top/gtrtfpjcjv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.9152youxi.cn/gtdecfpqnz.html

[U05] Py：列表去重且保序
来源：http://hz.andypj.xyz/gtxgpmvviv.html

list(dict.fromkeys(arr))
来源：http://hz.zycfv.cn/gtencphsvx.html

[U06] Py：合并两个字典
来源：http://hz.nanxuanxn.top/gtxwoyrubw.html

{**a, **b}
来源：http://hz.haohaochexian.top/gtlsiuayny.html

[U07] Py：反转字典键值
来源：http://hz.0kj1m.cn/gtagxnvvtp.html

{v: k for k, v in d.items()}
来源：http://hz.mhx1999.top/gtiprmpyvj.html

[U08] Py：展平二维列表
来源：http://hz.iojbl.cn/gteawgvpjy.html

[y for x in nested for y in x]
来源：http://hz.gaohongyu789.top/gtdhttbmve.html

[U09] Py：字典取最大值的键
来源：http://hz.cashguo.top/gtlvcybvth.html

max(d, key=d.get)
来源：http://hz.pycfn.com/gtesjjnvsn.html

[U10] Py：按值排序字典
来源：http://hz.daria6918.cn/gtzjodxneu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yueranfly.top/gtcgjivdyx.html

[U11] Py：生成器表达式
来源：http://hz.hysaishi.cn/gtzcunfjxe.html

(x * 2 for x in arr)
来源：http://hz.tian-w.cn/gtvfvcvhsx.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.hnxiangtu.top/gtydkyziiu.html

Counter(arr).most_common(3)
来源：http://hz.ppjwa.cn/gtckiultgv.html

[U13] Py：固定长度队列
来源：http://hz.dianchejie.cn/gtdyiipufd.html

deque(maxlen=10)
来源：http://hz.jianghu66.top/gtdizqatvf.html

[U14] Py：分组收集到列表
来源：http://hz.chenzaomai.com/gtnqdzxmbz.html

defaultdict(list)
来源：http://hz.aibaodan.cn/gtpykdxoqr.html

[U15] Py：高精度计时
来源：http://hz.zhengqikj.top/gtvlqjqfsr.html

t = time.perf_counter()
来源：http://hz.tian-w.cn/gtkozfsvex.html

[U16] Py：命令行参数解析
来源：http://hz.ybcxt.top/gtrktnxriy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.yj202588.top/gtbaagxhxx.html

[U17] Py：初始化日志
来源：http://hz.xylfe.cn/gtfojlzbok.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.chenzaomai.com/gtwspayizu.html

[U18] Py：预编译正则
来源：http://hz.ppjwa.cn/gtsgcynmrp.html

pat = re.compile(r"\d+")
来源：http://hz.dianchejie.cn/gtikuiwsec.html

[U19] Py：正则替换带回调
来源：http://hz.daria6918.cn/gtmwrthyzr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.9152youxi.cn/gtmgwjjdem.html

[U20] Py：缓存函数结果
来源：http://hz.sufxvd.cn/gtckmcmrvb.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sufxvd.cn/gtsbimdlqd.html

[U21] Py：自定义上下文管理器
来源：http://hz.jinqigfzy.top/gtqctzwtcs.html

@contextlib.contextmanager
来源：http://hz.svipenyu.cn/gtbpgnluwn.html

[U22] Py：矩阵转置
来源：http://hz.andypj.xyz/gtlgzgpztn.html

list(zip(*m))
来源：http://hz.yj20258.top/gtvmwxzhjd.html

[U23] Py：分块读取大文件
来源：http://hz.jinghuilouyu.cn/gtguulrnvx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.mhx1999.top/gtuavnvoqn.html

[U24] Py：路径操作
来源：http://hz.tian-w.cn/gtdvekduxq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.yj20258.top/gtzdqjdmdd.html

[U25] Py：CSV 按字典读
来源：http://hz.0kj1m.cn/gtqdkozlaj.html

csv.DictReader(f)
来源：http://hz.hysaishi.cn/gtbqphytpd.html

[U26] Py：并发下载
来源：http://hz.hammf.cn/gtfwchzkut.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jinqigfzy.top/gtgfkxpkpb.html

[U27] Py：异步 HTTP
来源：http://hz.chenlongwang.top/gtzwtxprxa.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.guowangkeji.top/gtemvvcdnm.html

[U28] Py：类型别名
来源：http://hz.jyoumei.cn/gtmzihfqse.html

UserId = int
来源：http://hz.zhixingplan.top/gthawxymwg.html

[U29] Py：属性校验
来源：http://hz.9152youxi.cn/gtmfvbxnqq.html

@property 与 @x.setter 配合
来源：http://hz.guowangkeji.top/gtudxhnqtt.html

[U30] Py：数据类
来源：http://hz.ivvv.top/gtwxxeatrn.html

@dataclass(slots=True)
来源：http://hz.0kj1m.cn/gthicjreqp.html

[U31] Py：单测
来源：http://hz.chenlongwang.top/gtgxpogzyx.html

python -m pytest -q
来源：http://hz.andypj.xyz/gtijpvvhdi.html

[U32] Py：代码格式化
来源：http://hz.tanke756.top/gtejjebmtc.html

ruff format . && ruff check --fix .
来源：http://hz.sufxvd.cn/gtedwzkfey.html

[U33] Py：打包发布
来源：http://hz.zycfv.cn/gtdypifqww.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.guannengcc.top/gtnlylvpuh.html

[U34] Py：判断编码
来源：http://hz.sweek.top/gtsjqwogxn.html

chardet.detect(raw)
来源：http://hz.havefunace.top/gtecdygiaa.html

[U35] Py：发送邮件
来源：http://hz.aizwys.cn/gtdhnxscrj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.gzhubu.top/gtdgffoqpu.html

[U36] Py：定时任务
来源：http://hz.zhongyouzk.top/gtnkldsdjo.html

schedule.every(10).minutes.do(job)
来源：http://hz.jinqigufen.top/gtedrrlkvt.html

[U37] Py：读写 Excel
来源：http://hz.xziqi.cn/gtwlezgljo.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.birdmap.top/gtwqpmqmyi.html

[U38] Py：获取脚本所在目录
来源：http://hz.andypj.xyz/gtewqemepb.html

Path(__file__).resolve().parent
来源：http://hz.9152youxi.cn/gtpehmqamh.html

[U39] Py：判断是否在交互环境
来源：http://hz.jinghuilouyu.cn/gtocmvbboq.html

sys.stdout.isatty()
来源：http://hz.gotoacloud.top/gtazrmprrt.html

[U40] Py：打印到标准错误
来源：http://hz.chenlongwang.top/gthlzbmhxy.html

print("err", file=sys.stderr)
来源：http://hz.zhixingplan.top/gtmvskmang.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.shanyushiyangkeji.top/gtrgogcymm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.c1oappe.top/gtyrfkottv.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.cdnleiting.top/gtvpuwnoui.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.tian-w.cn/gtolfwmgvs.html

[U43] PHP：声明命名空间
来源：http://hz.bjfxy.top/gtvnrkmktu.html

namespace App\Http;
来源：http://hz.chenzaomai.com/gtgmpwklul.html

[U44] PHP：开启严格类型
来源：http://hz.aizwys.cn/gtvpsxkipw.html

declare(strict_types=1);
来源：http://hz.52xcode.cn/gtguiaymij.html

[U45] PHP：类型声明与返回类型
来源：http://hz.zdqjudy.top/gtrahzwvsm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtvufxbnrq.html

[U46] PHP：可空类型
来源：http://hz.ywan-chungtsiang.top/gtnrybjzjz.html

?string $name = null
来源：http://hz.tian-w.cn/gtfmypoxhm.html

[U47] PHP：联合类型
来源：http://hz.hnqzz.top/gtzmfgwhcb.html

int|string $id
来源：http://hz.yangfankeji.com/gtynrogeut.html

[U48] PHP：纯枚举
来源：http://hz.316326.xyz/gtakfcmzpe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.nanxinkj.top/gtzklgebmj.html

[U49] PHP：只读属性
来源：http://hz.xinyue.icu/gtzfsecpbo.html

public readonly string $name
来源：http://hz.cdnleiting.top/gtmgzzftkd.html

[U50] PHP：构造器属性提升
来源：http://hz.xuanzx.com/gtbuevrdhy.html

public function __construct(private int $id) {}
来源：http://hz.hongshengwenyu.top/gtpnqwwrew.html

[U51] PHP：数组解构
来源：http://hz.gaohongyu789.top/gtngjykgij.html

[$a, $b] = $arr;
来源：http://hz.hongshengwenyu.top/gtefkkrowm.html

[U52] PHP：箭头函数
来源：http://hz.jlsjyb.cn/gtgohcliuz.html

$double = fn($x) => $x * 2;
来源：http://hz.iojbl.cn/gtsfkcqzlj.html

[U53] PHP：空合并运算符
来源：http://hz.52xcode.cn/gtxhnewtgo.html

$v = $a ?? $b ?? "default";
来源：http://hz.chenlongwang.top/gtquqonodt.html

[U54] PHP：空安全调用
来源：http://hz.bjfxy.top/gtzdosfhlb.html

$obj?->method()
来源：http://hz.aizwys.cn/gtynklgcrg.html

[U55] PHP：match 表达式
来源：http://hz.feifeiyinyue.top/gtopjjhdcs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.ybcxt.top/gthhpnejsh.html

[U56] PHP：命名参数
来源：http://hz.nanxinkj.top/gtqttmmpjl.html

f(a: 1, b: 2)
来源：http://hz.sufxvd.cn/gtomciuztl.html

[U57] PHP：字符串插值
来源：http://hz.xuanzx.com/gtbfbjwrki.html

"值: {$a}"
来源：http://hz.xuanzx.com/gtqgtlsvgs.html

[U58] PHP：数组三件套
来源：http://hz.xinyue.icu/gtfqofqobf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.dianchejie.cn/gtyugxczcp.html

[U59] PHP：自定义排序
来源：http://hz.xylfe.cn/gtquzkemfk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhaomingkeji.xyz/gtqmyumxnk.html

[U60] PHP：JSON 编解码
来源：http://hz.sufxvd.cn/gtarfbtqpi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jinqigfzy.top/gtvbkehwab.html

[U61] PHP：正则
来源：http://hz.aizwys.cn/gtnbkgxueh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.9152youxi.cn/gtcbtskwvz.html

[U62] PHP：日期对象
来源：http://hz.mhx1999.top/gtcbfogkgg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.hysaishi.cn/gteyewxfgt.html

[U63] PHP：文件读写
来源：http://hz.hnxiangtu.top/gtzcgudlxm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.hongshengwenyu.top/gtinuvduom.html

[U64] PHP：目录遍历
来源：http://hz.xuetiantiany.cn/gtcorsskqo.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.hysaishi.cn/gtkevhzfcy.html

[U65] PHP：会话
来源：http://hz.aibaodan.cn/gtzeguzyql.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.wangshuangyany.cn/gtircqhdxj.html

[U66] PHP：设置 Cookie
来源：http://hz.jyoumei.cn/gtsnizcfxc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.meibo888.top/gthwftoapu.html

[U67] PHP：处理文件上传
来源：http://hz.zdqjudy.top/gtstmkirie.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.quarkkingdee.top/gttnwnctcr.html

[U68] PHP：PDO 连接
来源：http://hz.fengsongda.top/gtkqciwvdh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.yj202588.top/gtbtiqgiso.html

[U69] PHP：PDO 预处理
来源：http://hz.fengsongda.top/gtzvqozniy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.ybcxt.top/gtrvtorurq.html

[U70] PHP：PDO 事务
来源：http://hz.jqgufenzy.top/gtkfhswxqb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.gzhubu.top/gtklcdxvux.html

[U71] PHP：抛出异常
来源：http://hz.zhaomingkeji.xyz/gtccqwlziz.html

throw new RuntimeException("失败", 500);
来源：http://hz.xinyue.icu/gtmdtcojht.html

[U72] PHP：写错误日志
来源：http://hz.chenjidiqi.icu/gtrgqodolz.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shzxlz.cn/gtugjyiueo.html

[U73] PHP：读取 ini 配置
来源：http://hz.gzhubu.top/gtkzgbrkft.html

parse_ini_file("config.ini", true)
来源：http://hz.yonumen.top/gtejczfcig.html

[U74] PHP：读取环境变量
来源：http://hz.kuanghao11.cn/gtmfiokjak.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yongpay.top/gtpycgefil.html

[U75] PHP：依赖注入
来源：http://hz.sweek.top/gtbzhsnakw.html

composer require psr/container
来源：http://hz.ydzc1.top/gtawudkthh.html

[U76] PHP：简单路由
来源：http://hz.ivvv.top/gtyygblffn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.bjfxy.top/gtrrhuxbve.html

[U77] PHP：模板渲染
来源：http://hz.gotoacloud.top/gtayvbbgum.html

composer require twig/twig
来源：http://hz.jiagoushi.top/gtgzrajtkl.html

[U78] PHP：单元测试
来源：http://hz.jiagoushi.top/gthaggwcal.html

composer require --dev phpunit/phpunit
来源：http://hz.andypj.xyz/gtwgdhduut.html

[U79] PHP：静态分析
来源：http://hz.zhongyouzk.top/gtpxacytyd.html

composer require --dev phpstan/phpstan
来源：http://hz.jqgufenzy.top/gtuvlstclf.html

[U80] PHP：代码规范修复
来源：http://hz.chenjidiqi.icu/gtnuulvbks.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shanyushiyangkeji.top/gtnxuezjar.html

[U81] JS：初始化项目
来源：http://hz.aibaodan.cn/gtcygcqngg.html

npm init -y;  npm i express
来源：http://hz.xziqi.cn/gtaovkjnrz.html

[U82] JS：package.json 脚本
来源：http://hz.nanxuanxn.top/gtrawevvmh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.pengpengdd.cyou/gtmxoctklh.html

[U83] JS：ES Module 导入导出
来源：http://hz.yongpay.top/gtifcdgohi.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.c1oappe.top/gtfzmzexkf.html

[U84] JS：CommonJS 写法
来源：http://hz.smart0.xyz/gtznfofydy.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.daxiang520.top/gtzkvjemnk.html


<!-- 参考信息 -->