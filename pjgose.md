代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://hz.quarkkingdee.top/gtyiolcrjb.html

[S59] C++：静态断言
来源：http://hz.nanxinkj.top/gtweeyzmoh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ybcxt.top/gtadrwyeuv.html

[S60] C++：遍历并删除元素
来源：http://hz.cqqwz.cn/gttouyedki.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.guannengcc.top/gttufwdqsn.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxnlecznl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinqigfzy.top/gtbygpcusd.html

================================================================================
来源：http://hz.daria6918.cn/gtbpmccitu.html

[T01] Kotlin：Hello World
来源：http://hz.chenjidiqi.icu/gtgllndxsi.html

println("Hello")
来源：http://hz.sysykeji.top/gtnriwntky.html

[T02] Kotlin：变量
来源：http://hz.yanxiufei.cn/gtxmgvakbp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.smart0.xyz/gteyvcgfxy.html

[T03] Kotlin：字符串模板
来源：http://hz.gogol.net.cn/gtrqhtpmti.html

"值: $b"
来源：http://hz.yvedp.cn/gtffqvclbu.html

[T04] Kotlin：空安全
来源：http://hz.ehwqpu.com/gtnonfrrga.html

val n: String? = null;  n?.length
来源：http://hz.ywan-chungtsiang.top/gtmknyukql.html

[T05] Kotlin：when 表达式
来源：http://hz.shzxlz.cn/gtwjnqwwyl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.dianchejie.cn/gtaujjghem.html

[T06] Kotlin：集合映射
来源：http://hz.birdmap.top/gttihgoosk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj202588.top/gteykvbikt.html

[T07] Kotlin：集合过滤
来源：http://hz.yueranfly.top/gtmpipxsze.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.birdmap.top/gtxwcyzszi.html

[T08] Kotlin：数据类
来源：http://hz.cucudq.cn/gtihujxxxj.html

data class User(val name: String, val age: Int)
来源：http://hz.daria6918.cn/gtjrxjiwud.html

[T09] Kotlin：扩展函数
来源：http://hz.cqqwz.cn/gthlhjunuq.html

fun String.exclaim() = this + "!"
来源：http://hz.aizwys.cn/gtkihzwreq.html

[T10] Kotlin：默认参数
来源：http://hz.daria6918.cn/gtplpkqryb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jlsjyb.cn/gtgzuwfxwc.html

[T11] Kotlin：协程
来源：http://hz.havefunace.top/gtvuxhxweb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenlongwang.top/gtvhwybshv.html

[T12] Kotlin：解构声明
来源：http://hz.ybcxt.top/gtzmzgkvms.html

val (a, b) = Pair(1, 2)
来源：http://hz.dashuyun.cn/gtbqeheyby.html

[T13] Kotlin：只读 Map
来源：http://hz.jinghuilouyu.cn/gtlxkhcjoi.html

val m = mapOf("a" to 1)
来源：http://hz.yongpay.top/gtjvoyysys.html

[T14] Kotlin：循环
来源：http://hz.jlsjyb.cn/gttwpoqcib.html

for (i in 1..10) println(i)
来源：http://hz.daxiang520.top/gtefdvnsei.html

[T15] Kotlin：接口
来源：http://hz.9152youxi.cn/gtugrxslyt.html

interface Shape { fun area(): Double }
来源：http://hz.chenjidiqi.icu/gtivppzeca.html

[T16] Swift：Hello World
来源：http://hz.jiagoushi.top/gtppjmvydr.html

print("Hello")
来源：http://hz.jyoumei.cn/gtzhsjqtfl.html

[T17] Swift：变量与常量
来源：http://hz.sweek.top/gtjfprdqnm.html

var a = 1;  let b = 2
来源：http://hz.xingfuxueyuan.xyz/gtaaietbaj.html

[T18] Swift：字符串插值
来源：http://hz.tianlin.xyz/gtnsxmcder.html

"值: \(b)"
来源：http://hz.zhijiandao.cn/gtiypltolz.html

[T19] Swift：可选绑定
来源：http://hz.cdnleiting.top/gtddbnagkv.html

if let n = opt { print(n) }
来源：http://hz.xingfuxueyuan.xyz/gtewiahhpj.html

[T20] Swift：数组操作
来源：http://hz.xylfe.cn/gtmiqxcmeg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhengqikj.top/gtxlgmiggy.html

[T21] Swift：遍历
来源：http://hz.redwolf501.top/gtyqrrrdqh.html

for x in a { print(x) }
来源：http://hz.sysykeji.top/gtkykfvafu.html

[T22] Swift：字典
来源：http://hz.yuxming.cn/gtlyhgipnn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hammf.cn/gtpzbsdoie.html

[T23] Swift：函数
来源：http://hz.nwbrower.top/gtebyudomt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.guowangkeji.top/gticnnzmes.html

[T24] Swift：闭包
来源：http://hz.yanxiufei.cn/gtbkmrtnbw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cqqwz.cn/gtucvkwppn.html

[T25] Swift：结构体
来源：http://hz.zdqjudy.top/gtvnxkudgn.html

struct P { var x: Int }
来源：http://hz.yj20258888.top/gthtrmxmpo.html

[T26] Swift：类与重写
来源：http://hz.tian-w.cn/gtoeacbqds.html

class A: Base { override func f() {} }
来源：http://hz.gogol.net.cn/gthwrkyiej.html

[T27] Swift：错误处理
来源：http://hz.zdqjudy.top/gtbzpzhiog.html

do { try f() } catch { print(error) }
来源：http://hz.jinyuanbaomall.cn/gtuqdwsiel.html

[T28] Swift：枚举
来源：http://hz.yj20258.top/gtjwnbqrrp.html

enum Color { case red, green }
来源：http://hz.bjfxy.top/gthaudgtrf.html

[T29] Swift：guard 提前返回
来源：http://hz.svipenyu.cn/gtwrctxuur.html

guard let x = opt else { return }
来源：http://hz.hammf.cn/gtqsnqmyos.html

[T30] Swift：协议
来源：http://hz.gotoacloud.top/gtnckalnzn.html

protocol Shape { func area() -> Double }
来源：http://hz.gzhubu.top/gtlzwxshlg.html

[T31] Lua：Hello World
来源：http://hz.sysykeji.top/gtvakmuzna.html

print("Hello")
来源：http://hz.jinqigfzy.top/gttuxuzwrs.html

[T32] Lua：局部变量
来源：http://hz.nwbrower.top/gtqazgwhgq.html

local a = 1
来源：http://hz.yonumen.top/gtaeteidak.html

[T33] Lua：表（数组）
来源：http://hz.tianlin.xyz/gtkvapsnaa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sweek.top/gtgtjglmmy.html

[T34] Lua：遍历表
来源：http://hz.daxiang520.top/gtcnsyhtxo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tanke756.top/gtcskapptx.html

[T35] Lua：字典表
来源：http://hz.yongpay.top/gtnofifshq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.zhijiandao.cn/gtzbdeclpf.html

[T36] Lua：函数
来源：http://hz.zhijiandao.cn/gtjjgbejce.html

function add(a, b) return a + b end
来源：http://hz.kuanghao11.cn/gtdttczgfh.html

[T37] Lua：字符串拼接
来源：http://hz.jinqigufen.top/gttsbtznij.html

"a" .. "b"
来源：http://hz.havefunace.top/gtibinqyby.html

[T38] Lua：条件
来源：http://hz.daria6918.cn/gtkprbbokc.html

if x > 0 then print("正") end
来源：http://hz.zhixingplan.top/gtpzpouqzh.html

[T39] Lua：模式匹配
来源：http://hz.jqgfzy.top/gthuvpysig.html

string.find(s, "%d+")
来源：http://hz.yj202588.top/gtxypgtypa.html

[T40] Lua：元表
来源：http://hz.jinqigufen.top/gtflgdqwgg.html

setmetatable({}, { __index = base })
来源：http://hz.shzxlz.cn/gttrsnqyoc.html

[T41] Perl：Hello World
来源：http://hz.quarkkingdee.top/gtlltkibva.html

print "Hello\n";
来源：http://hz.daria6918.cn/gtvqaupfan.html

[T42] Perl：变量类型
来源：http://hz.hywenlv.cn/gtmuygbgnr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.gzhubu.top/gteytptowz.html

[T43] Perl：字符串插值
来源：http://hz.hongshengwenyu.top/gtqxbidjfh.html

"值: $a"
来源：http://hz.xinyue.icu/gtwvfjzcji.html

[T44] Perl：条件
来源：http://hz.gotoacloud.top/gttbkkmkmh.html

if ($a > 0) { print "正"; }
来源：http://hz.yangfankeji.com/gtvunaxaum.html

[T45] Perl：数组遍历
来源：http://hz.hfpthk.cn/gtkvxwmgye.html

for my $x (@arr) { print $x; }
来源：http://hz.xinyue.icu/gtdilwmxro.html

[T46] Perl：哈希操作
来源：http://hz.zhijiandao.cn/gtefspdwwk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.vqdsnc.cn/gtqtvlewjx.html

[T47] Perl：正则捕获
来源：http://hz.jinyuanbaomall.cn/gtinezfjpw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.0kj1m.cn/gtqzdfizwk.html

[T48] Perl：正则替换
来源：http://hz.wangdashe.top/gtpfwgupzm.html

$s =~ s/old/new/g;
来源：http://hz.tian-w.cn/gtnavrwpdz.html

[T49] Perl：函数
来源：http://hz.ydjk.org.cn/gtnpuntscb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhoulong.xyz/gtdyuiyvad.html

[T50] Perl：逐行读文件
来源：http://hz.dashuyun.cn/gtedgadiqh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.zhoulong.xyz/gtogxksurj.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.jiagoushi.top/gtsgsvqayv.html

[T51] Scala：Hello World
来源：http://hz.zhiwuduotai.top/gtbkzbwxgm.html

println("Hello")
来源：http://hz.jlsjyb.cn/gtelkhxsgp.html

[T52] Scala：变量
来源：http://hz.havefunace.top/gtoonnedix.html

val a = 1;  var b = 2
来源：http://hz.shanyushiyangkeji.top/gtnytjxjjb.html

[T53] Scala：字符串插值
来源：http://hz.snrcjt.cn/gtwjzlquor.html

s"值: $b"
来源：http://hz.nanxuanxn.top/gtpbzziubm.html

[T54] Scala：集合映射
来源：http://hz.guowangkeji.top/gtvaqvvsho.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.hywenlv.cn/gtpitsbwxh.html

[T55] Scala：集合过滤
来源：http://hz.yuxming.cn/gtuvtmmdwl.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.quarkkingdee.top/gtkmyhmcvw.html

[T56] Scala：样例类
来源：http://hz.chenjidiqi.icu/gtxoolqauv.html

case class User(name: String, age: Int)
来源：http://hz.jinghuilouyu.cn/gtsvlwdlod.html

[T57] Scala：模式匹配
来源：http://hz.pycfn.com/gtkcdtbjlq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.xuetiantiany.cn/gtxlxmggac.html

[T58] Scala：函数定义
来源：http://hz.wangshuangyany.cn/gtaiqmoaay.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.yj202588.top/gthcqumnro.html

[T59] Scala：循环
来源：http://hz.0kj1m.cn/gtsahiqcyv.html

for (i <- 1 to 10) println(i)
来源：http://hz.jiagoushi.top/gthkakroos.html

[T60] Scala：折叠
来源：http://hz.shuidangran.top/gtznrrowve.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.aibaodan.cn/gtsmgtbpmh.html

================================================================================
来源：http://hz.c1oappe.top/gtceouwwbv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.yuanzhike.top/gtkymjhowq.html

================================================================================
来源：http://hz.svipenyu.cn/gtyewmiitr.html

[U01] Py：创建虚拟环境
来源：http://hz.jqgfzy.top/gtgkwvqojt.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.shanyushiyangkeji.top/gtsavxiare.html

[U02] Py：导出 / 安装依赖
来源：http://hz.gzhubu.top/gthwlricav.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.nwbrower.top/gtskdkfkjz.html

[U03] Py：加载 .env 配置
来源：http://hz.zhengqikj.top/gtvhuzqkgr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.xuanzx.com/gtgezwoofa.html

[U04] Py：变量调试打印
来源：http://hz.sweek.top/gtialqvoah.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.pengpengdd.cyou/gtboeczzax.html

[U05] Py：列表去重且保序
来源：http://hz.quarkkingdee.top/gtvrkckfik.html

list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gthzcdfrkh.html

[U06] Py：合并两个字典
来源：http://hz.quarkkingdee.top/gtluoclbmy.html

{**a, **b}
来源：http://hz.jqgfzy.top/gtrzyewbsg.html

[U07] Py：反转字典键值
来源：http://hz.cucudq.cn/gthdsvfeex.html

{v: k for k, v in d.items()}
来源：http://hz.shangyingyoupin.top/gtadpbhevj.html

[U08] Py：展平二维列表
来源：http://hz.zhoulong.xyz/gtclmjmswt.html

[y for x in nested for y in x]
来源：http://hz.fengsongda.top/gtvvzvtqvg.html

[U09] Py：字典取最大值的键
来源：http://hz.ivvv.top/gtnurmtsua.html

max(d, key=d.get)
来源：http://hz.guannengcc.top/gttgmptbsy.html

[U10] Py：按值排序字典
来源：http://hz.jinghuilouyu.cn/gtnoadjvow.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yuanzhike.top/gtrlxqdufq.html

[U11] Py：生成器表达式
来源：http://hz.tian-w.cn/gtwvzqckow.html

(x * 2 for x in arr)
来源：http://hz.jinqigfzy.top/gtuucqfwqy.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.yj20258888.top/gtsqcrdgsr.html

Counter(arr).most_common(3)
来源：http://hz.jinghuilouyu.cn/gtehvlemjh.html

[U13] Py：固定长度队列
来源：http://hz.daxiang520.top/gtpgcbiwpf.html

deque(maxlen=10)
来源：http://hz.ehwqpu.com/gtidcgvhsk.html

[U14] Py：分组收集到列表
来源：http://hz.pycfn.com/gtslgemxmw.html

defaultdict(list)
来源：http://hz.sysykeji.top/gtdumyqxns.html

[U15] Py：高精度计时
来源：http://hz.chenzaomai.com/gtgjrobxwz.html

t = time.perf_counter()
来源：http://hz.fzhhl.top/gtkdbusqby.html

[U16] Py：命令行参数解析
来源：http://hz.cucudq.cn/gtujorrkhm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hongshengwenyu.top/gtpocznnfj.html

[U17] Py：初始化日志
来源：http://hz.xylfe.cn/gtgpklqmni.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yongpay.top/gtblclpitm.html

[U18] Py：预编译正则
来源：http://hz.fzhhl.top/gtlvwufjyd.html

pat = re.compile(r"\d+")
来源：http://hz.zdqjudy.top/gtejcaxtak.html

[U19] Py：正则替换带回调
来源：http://hz.gaohongyu789.top/gtasjlqohi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.jianghu66.top/gtpndaqjlx.html

[U20] Py：缓存函数结果
来源：http://hz.chenzaomai.com/gtcypjbgbl.html

@functools.lru_cache(maxsize=None)
来源：http://hz.sysykeji.top/gtejnyjkxc.html

[U21] Py：自定义上下文管理器
来源：http://hz.hfpthk.cn/gtizaqytun.html

@contextlib.contextmanager
来源：http://hz.guannengcc.top/gtwcalhqdr.html

[U22] Py：矩阵转置
来源：http://hz.yongpay.top/gtnatslucc.html

list(zip(*m))
来源：http://hz.cucudq.cn/gtrhksyiqe.html

[U23] Py：分块读取大文件
来源：http://hz.c1oappe.top/gtmyqwnhlw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jiagoushi.top/gtaewuqspk.html

[U24] Py：路径操作
来源：http://hz.yuanzhike.top/gtwpgcwfhs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.xziqi.cn/gtpjgzndhm.html

[U25] Py：CSV 按字典读
来源：http://hz.gotoacloud.top/gtbkvmlcao.html

csv.DictReader(f)
来源：http://hz.zdqjudy.top/gtvpkersro.html

[U26] Py：并发下载
来源：http://hz.wangshuangyany.cn/gtwpbtjquh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.jianghu66.top/gtnryaogkh.html

[U27] Py：异步 HTTP
来源：http://hz.jinghuilouyu.cn/gttrakwlcc.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.nwbrower.top/gtfqfckuel.html

[U28] Py：类型别名
来源：http://hz.hongshengwenyu.top/gtvinqmvls.html

UserId = int
来源：http://hz.yvedp.cn/gtqoalrtrz.html

[U29] Py：属性校验
来源：http://hz.pengpengdd.cyou/gtbxnogvmt.html

@property 与 @x.setter 配合
来源：http://hz.iojbl.cn/gtvrhirxdu.html

[U30] Py：数据类
来源：http://hz.tanke756.top/gtzspwacom.html

@dataclass(slots=True)
来源：http://hz.hammf.cn/gttzssajru.html

[U31] Py：单测
来源：http://hz.redwolf501.top/gtxqmxtxdi.html

python -m pytest -q
来源：http://hz.gzhubu.top/gtbqopfhgp.html

[U32] Py：代码格式化
来源：http://hz.meibo888.top/gtsetrbafl.html

ruff format . && ruff check --fix .
来源：http://hz.zhixingplan.top/gtkrpjprxw.html

[U33] Py：打包发布
来源：http://hz.yanxiufei.cn/gtzryplizd.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.ywan-chungtsiang.top/gtwduzpyqb.html

[U34] Py：判断编码
来源：http://hz.birdmap.top/gtzjnrpbwr.html

chardet.detect(raw)
来源：http://hz.shanyushiyangkeji.top/gtmxdkabqv.html

[U35] Py：发送邮件
来源：http://hz.yj20258888.top/gtowlldvtp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.xuetiantiany.cn/gtuoegtdlf.html

[U36] Py：定时任务
来源：http://hz.zdqjudy.top/gtbcheeeec.html

schedule.every(10).minutes.do(job)
来源：http://hz.haohaochexian.top/gtjlztlrmh.html

[U37] Py：读写 Excel
来源：http://hz.gzhubu.top/gtkcgnfben.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.cashguo.top/gtgohxnmxd.html

[U38] Py：获取脚本所在目录
来源：http://hz.shuidangran.top/gtaboumder.html

Path(__file__).resolve().parent
来源：http://hz.nwbrower.top/gtiyilqerj.html

[U39] Py：判断是否在交互环境
来源：http://hz.jinqigfzy.top/gtwjqhemvi.html

sys.stdout.isatty()
来源：http://hz.zhixingplan.top/gtiaaykbye.html

[U40] Py：打印到标准错误
来源：http://hz.yvedp.cn/gtkpcqdghn.html

print("err", file=sys.stderr)
来源：http://hz.yj20258.top/gtogsenhkt.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.ppjwa.cn/gtwfxezram.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.shanyushiyangtech.top/gtjzznyxgb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.zhiwuduotai.top/gtgguwvvip.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.nwbrower.top/gtjmuxcnes.html

[U43] PHP：声明命名空间
来源：http://hz.jinghuilouyu.cn/gtjeygofjt.html

namespace App\Http;
来源：http://hz.nanxuanxn.top/gtugdqinaw.html

[U44] PHP：开启严格类型
来源：http://hz.quarkkingdee.top/gtifrattbd.html

declare(strict_types=1);
来源：http://hz.jlsjyb.cn/gtlvclczhv.html

[U45] PHP：类型声明与返回类型
来源：http://hz.jinqigfzy.top/gtkggwxslc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtetcvxlxb.html

[U46] PHP：可空类型
来源：http://hz.jlsjyb.cn/gtoctgbchi.html

?string $name = null
来源：http://hz.hywenlv.cn/gtvoeuqfqd.html

[U47] PHP：联合类型
来源：http://hz.52xcode.cn/gtlwrcuqat.html

int|string $id
来源：http://hz.shanyushiyangkeji.top/gtwysdqhvw.html

[U48] PHP：纯枚举
来源：http://hz.chenjidiqi.icu/gthuujcuho.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ydjk.org.cn/gtdjwmvaug.html

[U49] PHP：只读属性
来源：http://hz.fengsongda.top/gtlfadweem.html

public readonly string $name
来源：http://hz.ivvv.top/gtydqkznfj.html

[U50] PHP：构造器属性提升
来源：http://hz.jqgufenzy.top/gtpmkkuquk.html

public function __construct(private int $id) {}
来源：http://hz.havefunace.top/gtlmcznujn.html

[U51] PHP：数组解构
来源：http://hz.zhengqikj.top/gtotuvspte.html

[$a, $b] = $arr;
来源：http://hz.cashguo.top/gtrzabxjks.html

[U52] PHP：箭头函数
来源：http://hz.yvedp.cn/gtqkdsfllz.html

$double = fn($x) => $x * 2;
来源：http://hz.zhiwuduotai.top/gtigtgcbyn.html

[U53] PHP：空合并运算符
来源：http://hz.dashuyun.cn/gtbuqlceio.html

$v = $a ?? $b ?? "default";
来源：http://hz.fengsongda.top/gtyqbdeyon.html

[U54] PHP：空安全调用
来源：http://hz.gzhubu.top/gtzufzqgbt.html

$obj?->method()
来源：http://hz.gogol.net.cn/gtohqcuptc.html

[U55] PHP：match 表达式
来源：http://hz.daxiang520.top/gttaqljgfa.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cqqwz.cn/gtxkgbewrq.html

[U56] PHP：命名参数
来源：http://hz.xylfe.cn/gtnikzxgpy.html

f(a: 1, b: 2)
来源：http://hz.c1oappe.top/gtkandygdh.html

[U57] PHP：字符串插值
来源：http://hz.zhoulong.xyz/gtivybcvdm.html

"值: {$a}"
来源：http://hz.ywan-chungtsiang.top/gtibpveojx.html

[U58] PHP：数组三件套
来源：http://hz.cdnleiting.top/gtrwltbyup.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.gaohongyu789.top/gtbsqmkxea.html

[U59] PHP：自定义排序
来源：http://hz.chenjidiqi.icu/gtbefwlshx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.c1oappe.top/gtswucavzh.html

[U60] PHP：JSON 编解码
来源：http://hz.aibaodan.cn/gtmnnqiyge.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.ydzc1.top/gtuqshxqhz.html

[U61] PHP：正则
来源：http://hz.ydjk.org.cn/gtewqifjgg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.hywenlv.cn/gtmanuynes.html

[U62] PHP：日期对象
来源：http://hz.haohaochexian.top/gtnnslmzid.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.xinyue.icu/gtulejoldj.html

[U63] PHP：文件读写
来源：http://hz.pycfn.com/gtpugntmst.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.yongpay.top/gtecwtoktt.html

[U64] PHP：目录遍历
来源：http://hz.shzxlz.cn/gtndzbmtry.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.jianghu66.top/gtlnpyzwxc.html

[U65] PHP：会话
来源：http://hz.zhaomingkeji.xyz/gtmorfvpvk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.shuidangran.top/gtoxfpqxza.html

[U66] PHP：设置 Cookie
来源：http://hz.aibaodan.cn/gticbwnkhb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.pengpengdd.cyou/gtjwxtickg.html

[U67] PHP：处理文件上传
来源：http://hz.fzhhl.top/gtjdxmbabb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.cheryme.top/gtphmzaxsy.html

[U68] PHP：PDO 连接
来源：http://hz.xuanzx.com/gtxtcyimeo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.ivvv.top/gthycmnczk.html

[U69] PHP：PDO 预处理
来源：http://hz.ybcxt.top/gtjiogaven.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jiagoushi.top/gtunjiemud.html

[U70] PHP：PDO 事务
来源：http://hz.xziqi.cn/gtjptqynal.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.316326.xyz/gtmhkrxepb.html

[U71] PHP：抛出异常
来源：http://hz.zhoulong.xyz/gtxudbdcqg.html

throw new RuntimeException("失败", 500);
来源：http://hz.sxryk.cn/gtjceknjcg.html

[U72] PHP：写错误日志
来源：http://hz.shanyushiyangkeji.top/gtxftcwkic.html

error_log("失败: " . $e->getMessage());
来源：http://hz.dashuyun.cn/gtgwxvjhfi.html

[U73] PHP：读取 ini 配置
来源：http://hz.jinqigufen.top/gtdeqrgvkm.html

parse_ini_file("config.ini", true)
来源：http://hz.hnxiangtu.top/gtgllgdkpa.html

[U74] PHP：读取环境变量
来源：http://hz.shuidangran.top/gtmmfwyqar.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yonumen.top/gtyupnytkj.html

[U75] PHP：依赖注入
来源：http://hz.jinghuilouyu.cn/gtlxznvnxr.html

composer require psr/container
来源：http://hz.wangdashe.top/gtffkaafet.html

[U76] PHP：简单路由
来源：http://hz.cheryme.top/gtnzfgtlvp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.tanke756.top/gtflnknxlx.html

[U77] PHP：模板渲染
来源：http://hz.hammf.cn/gtrozcqcek.html

composer require twig/twig
来源：http://hz.yvedp.cn/gtavyckcaq.html

[U78] PHP：单元测试
来源：http://hz.xylfe.cn/gtfgkzkjqs.html

composer require --dev phpunit/phpunit
来源：http://hz.vqdsnc.cn/gtpilsyatv.html

[U79] PHP：静态分析
来源：http://hz.xziqi.cn/gtgjoqqcbq.html

composer require --dev phpstan/phpstan
来源：http://hz.zhoulong.xyz/gtczdbjgfl.html

[U80] PHP：代码规范修复
来源：http://hz.pengpengdd.cyou/gtnwebnfts.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.gzhubu.top/gttevhqyiv.html

[U81] JS：初始化项目
来源：http://hz.nanxuanxn.top/gtbudanghm.html

npm init -y;  npm i express
来源：http://hz.zhixingplan.top/gtnjnrorqo.html

[U82] JS：package.json 脚本
来源：http://hz.cqqwz.cn/gtdjbehayr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhongyouzk.top/gtrqihjmoi.html

[U83] JS：ES Module 导入导出
来源：http://hz.c1oappe.top/gtqlflhyzs.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.52xcode.cn/gtjwlowvee.html

[U84] JS：CommonJS 写法
来源：http://hz.9152youxi.cn/gtkrubymzv.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.vqdsnc.cn/gtrixuziec.html


<!-- 参考信息 -->