代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xziqi.cn/gtbshpvxvn.html

[S57] C++：编译期常量
来源：http://hz.daria6918.cn/gtjplpmzof.html

constexpr int N = 10;
来源：http://hz.ydzc1.top/gtxeclpmsm.html

[S58] C++：命名空间
来源：http://hz.ppjwa.cn/gtotlyjlgv.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhongyouzk.top/gtgndfsvnh.html

[S59] C++：静态断言
来源：http://hz.jinghuilouyu.cn/gtubocuylb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenjidiqi.icu/gtzkgzphfs.html

[S60] C++：遍历并删除元素
来源：http://hz.gotoacloud.top/gtodmafvpy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ybcxt.top/gtnjjobgmd.html

================================================================================
来源：http://hz.pycfn.com/gtcuyhqjuw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj202588.top/gtebprbyzz.html

================================================================================
来源：http://hz.fengsongda.top/gtbuzvgwqc.html

[T01] Kotlin：Hello World
来源：http://hz.jqgufenzy.top/gtgheaarvn.html

println("Hello")
来源：http://hz.iojbl.cn/gtalihkrie.html

[T02] Kotlin：变量
来源：http://hz.ydzc1.top/gtlxhqerzb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhongyouzk.top/gtjyixpxms.html

[T03] Kotlin：字符串模板
来源：http://hz.svipenyu.cn/gtzqsjcczy.html

"值: $b"
来源：http://hz.hywenlv.cn/gtegvkoasd.html

[T04] Kotlin：空安全
来源：http://hz.andypj.xyz/gtigczrlry.html

val n: String? = null;  n?.length
来源：http://hz.wangdashe.top/gtmjwsmrls.html

[T05] Kotlin：when 表达式
来源：http://hz.c1oappe.top/gtujepenad.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinghuilouyu.cn/gtryuslmns.html

[T06] Kotlin：集合映射
来源：http://hz.sufxvd.cn/gtyzcnrrst.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.meibo888.top/gtyhmrpfdc.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gtkotlvewo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.meibo888.top/gtlskfuqte.html

[T08] Kotlin：数据类
来源：http://hz.hnxiangtu.top/gttcdcvjhx.html

data class User(val name: String, val age: Int)
来源：http://hz.zhaomingkeji.xyz/gtxeiuasfg.html

[T09] Kotlin：扩展函数
来源：http://hz.quarkkingdee.top/gtfszvhaqf.html

fun String.exclaim() = this + "!"
来源：http://hz.yuanzhike.top/gthrypcbjw.html

[T10] Kotlin：默认参数
来源：http://hz.vqdsnc.cn/gtqikneunk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhiwuduotai.top/gtroaymwdr.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gtcerkozuu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.feifeiyinyue.top/gtbdfzgdwd.html

[T12] Kotlin：解构声明
来源：http://hz.yvedp.cn/gtiozpteec.html

val (a, b) = Pair(1, 2)
来源：http://hz.fzhhl.top/gtltkmntfg.html

[T13] Kotlin：只读 Map
来源：http://hz.meibo888.top/gtaljehbub.html

val m = mapOf("a" to 1)
来源：http://hz.zhengqikj.top/gtgjatowtb.html

[T14] Kotlin：循环
来源：http://hz.hongshengwenyu.top/gtcivujhcg.html

for (i in 1..10) println(i)
来源：http://hz.zhaomingkeji.xyz/gtrvibqmul.html

[T15] Kotlin：接口
来源：http://hz.daxiang520.top/gtmgnhjfzh.html

interface Shape { fun area(): Double }
来源：http://hz.dianchejie.cn/gtlzjhbpdi.html

[T16] Swift：Hello World
来源：http://hz.jinqigfzy.top/gtohxjrvgx.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtlkggnzup.html

[T17] Swift：变量与常量
来源：http://hz.daxiang520.top/gtvljcofyf.html

var a = 1;  let b = 2
来源：http://hz.shanyushiyangtech.top/gtsvghujxl.html

[T18] Swift：字符串插值
来源：http://hz.yongpay.top/gtnlstfokl.html

"值: \(b)"
来源：http://hz.c1oappe.top/gtmmxeuiio.html

[T19] Swift：可选绑定
来源：http://hz.birdmap.top/gtdzxuklae.html

if let n = opt { print(n) }
来源：http://hz.ppjwa.cn/gtpodsmwzg.html

[T20] Swift：数组操作
来源：http://hz.nanxinkj.top/gtfgypkdmr.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gzhubu.top/gtuonfdkdp.html

[T21] Swift：遍历
来源：http://hz.aizwys.cn/gtfviexipz.html

for x in a { print(x) }
来源：http://hz.52xcode.cn/gtnsughubr.html

[T22] Swift：字典
来源：http://hz.hnqzz.top/gtezzmrwth.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.fengsongda.top/gthfitszyi.html

[T23] Swift：函数
来源：http://hz.zhaomingkeji.xyz/gteyjnbydh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yvedp.cn/gtvajsdakf.html

[T24] Swift：闭包
来源：http://hz.zhixingplan.top/gtstplmfhh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.snrcjt.cn/gtvpfsksdi.html

[T25] Swift：结构体
来源：http://hz.bjfxy.top/gtwpxdnvxv.html

struct P { var x: Int }
来源：http://hz.ybcxt.top/gttguksmme.html

[T26] Swift：类与重写
来源：http://hz.cheryme.top/gtnniwsxqe.html

class A: Base { override func f() {} }
来源：http://hz.yangfankeji.com/gtfxwxstkr.html

[T27] Swift：错误处理
来源：http://hz.xziqi.cn/gtajskqeqk.html

do { try f() } catch { print(error) }
来源：http://hz.daxiang520.top/gtbipgthki.html

[T28] Swift：枚举
来源：http://hz.316326.xyz/gtmutuypgd.html

enum Color { case red, green }
来源：http://hz.ybcxt.top/gtwqncmbye.html

[T29] Swift：guard 提前返回
来源：http://hz.jinghuilouyu.cn/gtlagjukry.html

guard let x = opt else { return }
来源：http://hz.52xcode.cn/gtphjzitwo.html

[T30] Swift：协议
来源：http://hz.nanxinkj.top/gtpxatvqvo.html

protocol Shape { func area() -> Double }
来源：http://hz.xinyue.icu/gtsfnwqsie.html

[T31] Lua：Hello World
来源：http://hz.cdnleiting.top/gtbfnfebib.html

print("Hello")
来源：http://hz.dashuyun.cn/gthdrjbytm.html

[T32] Lua：局部变量
来源：http://hz.jinqigfzy.top/gtqhprsilx.html

local a = 1
来源：http://hz.dianchejie.cn/gtxdtpptcv.html

[T33] Lua：表（数组）
来源：http://hz.fengsongda.top/gtpilnycjh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.dianchejie.cn/gtckrcqofk.html

[T34] Lua：遍历表
来源：http://hz.hfpthk.cn/gtcfdtsqil.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.tianlin.xyz/gtvldlpuav.html

[T35] Lua：字典表
来源：http://hz.tanke756.top/gtanvekzsh.html

local d = { a = 1 };  d.b = 2
来源：http://hz.dashuyun.cn/gtcysycbnw.html

[T36] Lua：函数
来源：http://hz.iojbl.cn/gtpaqipwad.html

function add(a, b) return a + b end
来源：http://hz.hnxiangtu.top/gtwhzcrbnn.html

[T37] Lua：字符串拼接
来源：http://hz.zycfv.cn/gtawpxzghm.html

"a" .. "b"
来源：http://hz.jinqigfzy.top/gtqzzwgmgz.html

[T38] Lua：条件
来源：http://hz.tianlin.xyz/gtavvwzvkl.html

if x > 0 then print("正") end
来源：http://hz.xingfuxueyuan.xyz/gtqsaykgio.html

[T39] Lua：模式匹配
来源：http://hz.jinqigfzy.top/gtnpuwtatq.html

string.find(s, "%d+")
来源：http://hz.pengpengdd.cyou/gtiqeznfam.html

[T40] Lua：元表
来源：http://hz.daxiang520.top/gtzjoomdiv.html

setmetatable({}, { __index = base })
来源：http://hz.gzhubu.top/gtykwsjbjv.html

[T41] Perl：Hello World
来源：http://hz.xinyue.icu/gtejqnxjwm.html

print "Hello\n";
来源：http://hz.tianlin.xyz/gtatxabdzo.html

[T42] Perl：变量类型
来源：http://hz.ppjwa.cn/gtxmxxzmoq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.guannengcc.top/gtqhauvuel.html

[T43] Perl：字符串插值
来源：http://hz.cashguo.top/gtpsvccaaz.html

"值: $a"
来源：http://hz.cqqwz.cn/gtjcnplsbu.html

[T44] Perl：条件
来源：http://hz.yj202588.top/gtxgoqwcoq.html

if ($a > 0) { print "正"; }
来源：http://hz.sxryk.cn/gtofedohao.html

[T45] Perl：数组遍历
来源：http://hz.hongshengwenyu.top/gtdjctykvl.html

for my $x (@arr) { print $x; }
来源：http://hz.yvedp.cn/gtvttsroyp.html

[T46] Perl：哈希操作
来源：http://hz.ehwqpu.com/gtdwmnnltf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinyuanbaomall.cn/gtxvogrdwd.html

[T47] Perl：正则捕获
来源：http://hz.nanxuanxn.top/gtctdgfqzj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yuxming.cn/gtnjaonhtf.html

[T48] Perl：正则替换
来源：http://hz.fzhhl.top/gttnahuqbp.html

$s =~ s/old/new/g;
来源：http://hz.daria6918.cn/gtzuaubmhv.html

[T49] Perl：函数
来源：http://hz.tian-w.cn/gtahmhjerp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.52xcode.cn/gtjqkjobwu.html

[T50] Perl：逐行读文件
来源：http://hz.ybcxt.top/gtnlcoelwi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jianghu66.top/gtdtgxnpqh.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.hfpthk.cn/gtntczakjr.html

[T51] Scala：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtzhhmiqdt.html

println("Hello")
来源：http://hz.kuanghao11.cn/gtecazvsev.html

[T52] Scala：变量
来源：http://hz.zhiwuduotai.top/gtqxvrfgjp.html

val a = 1;  var b = 2
来源：http://hz.xuetiantiany.cn/gtuxypmkws.html

[T53] Scala：字符串插值
来源：http://hz.svipenyu.cn/gtmpzvohzu.html

s"值: $b"
来源：http://hz.aizwys.cn/gtplzbxnip.html

[T54] Scala：集合映射
来源：http://hz.chenzaomai.com/gtnekhgbjb.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.vqdsnc.cn/gtyrjazdxw.html

[T55] Scala：集合过滤
来源：http://hz.xingfuxueyuan.xyz/gtdulwxwrt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shanyushiyangkeji.top/gtmeiuvtuz.html

[T56] Scala：样例类
来源：http://hz.birdmap.top/gtkefdfmdy.html

case class User(name: String, age: Int)
来源：http://hz.xuetiantiany.cn/gtogrdkotj.html

[T57] Scala：模式匹配
来源：http://hz.chenzaomai.com/gtoutedvie.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.tianlin.xyz/gtwcdnubmw.html

[T58] Scala：函数定义
来源：http://hz.pycfn.com/gtfjeeebtx.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.aizwys.cn/gtcktddlrk.html

[T59] Scala：循环
来源：http://hz.ywan-chungtsiang.top/gtmqgaihig.html

for (i <- 1 to 10) println(i)
来源：http://hz.hammf.cn/gtaexvwnbj.html

[T60] Scala：折叠
来源：http://hz.dashuyun.cn/gtjgriccxu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.chenzaomai.com/gtlhgluowq.html

================================================================================
来源：http://hz.yongpay.top/gtrzbdlyem.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.jiagoushi.top/gtglptzapd.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtadaublmv.html

[U01] Py：创建虚拟环境
来源：http://hz.haohaochexian.top/gtdvasjtop.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.tian-w.cn/gtzydceilj.html

[U02] Py：导出 / 安装依赖
来源：http://hz.c1oappe.top/gtuhdnjsez.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.cdnleiting.top/gtvlndjeai.html

[U03] Py：加载 .env 配置
来源：http://hz.zhongyouzk.top/gttqgxarrl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shuidangran.top/gthbgznflh.html

[U04] Py：变量调试打印
来源：http://hz.zhiwuduotai.top/gtmgtcxqoa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.nanxinkj.top/gtoczgjoik.html

[U05] Py：列表去重且保序
来源：http://hz.zdqjudy.top/gttnqiwijg.html

list(dict.fromkeys(arr))
来源：http://hz.hongshengwenyu.top/gtdcxobyjz.html

[U06] Py：合并两个字典
来源：http://hz.smart0.xyz/gtvjxvqrqa.html

{**a, **b}
来源：http://hz.jlsjyb.cn/gtoshzeuyv.html

[U07] Py：反转字典键值
来源：http://hz.jqgufenzy.top/gtjrbtudsr.html

{v: k for k, v in d.items()}
来源：http://hz.yongpay.top/gtmybdlkyc.html

[U08] Py：展平二维列表
来源：http://hz.jinghuilouyu.cn/gtznviokyj.html

[y for x in nested for y in x]
来源：http://hz.gzhubu.top/gtkjrizxjb.html

[U09] Py：字典取最大值的键
来源：http://hz.zhiwuduotai.top/gtayasjccv.html

max(d, key=d.get)
来源：http://hz.jianghu66.top/gtbcocpqrq.html

[U10] Py：按值排序字典
来源：http://hz.zhaomingkeji.xyz/gtcmiatnpt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.gaohongyu789.top/gtwcpcrvqn.html

[U11] Py：生成器表达式
来源：http://hz.redwolf501.top/gtkwxzasps.html

(x * 2 for x in arr)
来源：http://hz.iojbl.cn/gtcrdixzci.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.smart0.xyz/gtkjdxgtxj.html

Counter(arr).most_common(3)
来源：http://hz.nwbrower.top/gtmaaudkmf.html

[U13] Py：固定长度队列
来源：http://hz.snrcjt.cn/gtkuahxcet.html

deque(maxlen=10)
来源：http://hz.tanke756.top/gtodbelzlj.html

[U14] Py：分组收集到列表
来源：http://hz.gotoacloud.top/gtqktrgsnv.html

defaultdict(list)
来源：http://hz.52xcode.cn/gtdjghivgd.html

[U15] Py：高精度计时
来源：http://hz.yanxiufei.cn/gtimzxxbnr.html

t = time.perf_counter()
来源：http://hz.vqdsnc.cn/gtutcmksro.html

[U16] Py：命令行参数解析
来源：http://hz.snrcjt.cn/gtfrefgbju.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.sufxvd.cn/gtxwxrzler.html

[U17] Py：初始化日志
来源：http://hz.yanxiufei.cn/gtlmhpinud.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.bjfxy.top/gtvxdsutzq.html

[U18] Py：预编译正则
来源：http://hz.shangyingyoupin.top/gtzleohljh.html

pat = re.compile(r"\d+")
来源：http://hz.yuanzhike.top/gtyvxapdli.html

[U19] Py：正则替换带回调
来源：http://hz.andypj.xyz/gtzlxibknn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.cheryme.top/gthksewmjp.html

[U20] Py：缓存函数结果
来源：http://hz.xziqi.cn/gtjtlbzijf.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinqigfzy.top/gtbrwmyybb.html

[U21] Py：自定义上下文管理器
来源：http://hz.ywan-chungtsiang.top/gtcimjootb.html

@contextlib.contextmanager
来源：http://hz.nwbrower.top/gtgfoyoiek.html

[U22] Py：矩阵转置
来源：http://hz.snrcjt.cn/gtaagyirvf.html

list(zip(*m))
来源：http://hz.feifeiyinyue.top/gtbtjogbdt.html

[U23] Py：分块读取大文件
来源：http://hz.aibaodan.cn/gtsfkfpxja.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.jqgfzy.top/gtunbjiduh.html

[U24] Py：路径操作
来源：http://hz.yonumen.top/gtvtjgavgt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.feifeiyinyue.top/gtvjdljoji.html

[U25] Py：CSV 按字典读
来源：http://hz.shzxlz.cn/gttialryym.html

csv.DictReader(f)
来源：http://hz.ydjk.org.cn/gtxdgdkumo.html

[U26] Py：并发下载
来源：http://hz.yvedp.cn/gtlthgxkbw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.316326.xyz/gtvwlrmpuz.html

[U27] Py：异步 HTTP
来源：http://hz.gotoacloud.top/gtcjoykgrv.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.sweek.top/gttvsxgtni.html

[U28] Py：类型别名
来源：http://hz.redwolf501.top/gtmrktnugh.html

UserId = int
来源：http://hz.tanke756.top/gtmnnbijyd.html

[U29] Py：属性校验
来源：http://hz.cheryme.top/gteaxtboss.html

@property 与 @x.setter 配合
来源：http://hz.zdqjudy.top/gtlhooogfi.html

[U30] Py：数据类
来源：http://hz.zhijiandao.cn/gtrcflsgym.html

@dataclass(slots=True)
来源：http://hz.gotoacloud.top/gtsfxveroy.html

[U31] Py：单测
来源：http://hz.fzhhl.top/gtwimlmgdn.html

python -m pytest -q
来源：http://hz.ywan-chungtsiang.top/gtqtaavvnq.html

[U32] Py：代码格式化
来源：http://hz.hongshengwenyu.top/gtjeyrrcdo.html

ruff format . && ruff check --fix .
来源：http://hz.gogol.net.cn/gtcvxwaobk.html

[U33] Py：打包发布
来源：http://hz.pycfn.com/gtcfhsiuzb.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.dianchejie.cn/gtfatusffs.html

[U34] Py：判断编码
来源：http://hz.chenzaomai.com/gtktpveilo.html

chardet.detect(raw)
来源：http://hz.daria6918.cn/gtyvkamgre.html

[U35] Py：发送邮件
来源：http://hz.vqdsnc.cn/gtqyqlysmp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.nanxuanxn.top/gtbbycqqqr.html

[U36] Py：定时任务
来源：http://hz.zhaomingkeji.xyz/gtenhacrwk.html

schedule.every(10).minutes.do(job)
来源：http://hz.sysykeji.top/gtiqzadejm.html

[U37] Py：读写 Excel
来源：http://hz.cucudq.cn/gtphihpvny.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.zhixingplan.top/gtqdyywiwx.html

[U38] Py：获取脚本所在目录
来源：http://hz.havefunace.top/gtdirodefc.html

Path(__file__).resolve().parent
来源：http://hz.tian-w.cn/gtlxgxqyqa.html

[U39] Py：判断是否在交互环境
来源：http://hz.sweek.top/gtaacfoxtx.html

sys.stdout.isatty()
来源：http://hz.jianghu66.top/gtotszsyxv.html

[U40] Py：打印到标准错误
来源：http://hz.shanyushiyangtech.top/gttghbswkv.html

print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gtnhdlhdwr.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yj202588.top/gtdirnkvew.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.jqgufenzy.top/gtwfaerojf.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.shanyushiyangkeji.top/gtxifxxrfx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.nanxinkj.top/gtfigyasqh.html

[U43] PHP：声明命名空间
来源：http://hz.kuanghao11.cn/gtelmbqcgq.html

namespace App\Http;
来源：http://hz.zhixingplan.top/gtvgqisoxh.html

[U44] PHP：开启严格类型
来源：http://hz.snrcjt.cn/gtdhcgfmoo.html

declare(strict_types=1);
来源：http://hz.feifeiyinyue.top/gtnrduspfo.html

[U45] PHP：类型声明与返回类型
来源：http://hz.svipenyu.cn/gtausdgppx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gtfdqzdqis.html

[U46] PHP：可空类型
来源：http://hz.yonumen.top/gtguvcsmzw.html

?string $name = null
来源：http://hz.316326.xyz/gtmrcmqyhm.html

[U47] PHP：联合类型
来源：http://hz.shuidangran.top/gtsivthwqv.html

int|string $id
来源：http://hz.jinqigfzy.top/gtgwehfzfp.html

[U48] PHP：纯枚举
来源：http://hz.jinghuilouyu.cn/gtilvovcge.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.yueranfly.top/gtfojzwtfa.html

[U49] PHP：只读属性
来源：http://hz.hammf.cn/gtqruytmko.html

public readonly string $name
来源：http://hz.yonumen.top/gtdmsrcqjy.html

[U50] PHP：构造器属性提升
来源：http://hz.daxiang520.top/gtbguhtxqq.html

public function __construct(private int $id) {}
来源：http://hz.aibaodan.cn/gtkkdmwpvw.html

[U51] PHP：数组解构
来源：http://hz.pycfn.com/gtskpssnzu.html

[$a, $b] = $arr;
来源：http://hz.ywan-chungtsiang.top/gtdyzuzycx.html

[U52] PHP：箭头函数
来源：http://hz.52xcode.cn/gtlejwyafz.html

$double = fn($x) => $x * 2;
来源：http://hz.pycfn.com/gtvhskjneb.html

[U53] PHP：空合并运算符
来源：http://hz.kuanghao11.cn/gtmdsmvcjd.html

$v = $a ?? $b ?? "default";
来源：http://hz.hnqzz.top/gterwfqfsj.html

[U54] PHP：空安全调用
来源：http://hz.shzxlz.cn/gtitumeegk.html

$obj?->method()
来源：http://hz.xinyue.icu/gtzcisrygo.html

[U55] PHP：match 表达式
来源：http://hz.gaohongyu789.top/gtwupnjnqk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.cucudq.cn/gtadapfzpk.html

[U56] PHP：命名参数
来源：http://hz.yueranfly.top/gthpbxcypz.html

f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtsavnmagh.html

[U57] PHP：字符串插值
来源：http://hz.pycfn.com/gtcemqtqhi.html

"值: {$a}"
来源：http://hz.yanxiufei.cn/gtwnqwemnr.html

[U58] PHP：数组三件套
来源：http://hz.aibaodan.cn/gtfbiudket.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.nwbrower.top/gtymglkgew.html

[U59] PHP：自定义排序
来源：http://hz.guowangkeji.top/gtxexxfuuw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hfpthk.cn/gthhiaclgj.html

[U60] PHP：JSON 编解码
来源：http://hz.shanyushiyangtech.top/gtytzviozk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.316326.xyz/gtzxyyeinb.html

[U61] PHP：正则
来源：http://hz.yuanzhike.top/gthvupdzhq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.yongpay.top/gtayzaqioj.html

[U62] PHP：日期对象
来源：http://hz.hnxiangtu.top/gtxsujsmzp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.shanyushiyangtech.top/gthbocvoce.html

[U63] PHP：文件读写
来源：http://hz.xinyue.icu/gtruecomvn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.bjfxy.top/gtwulokhnr.html

[U64] PHP：目录遍历
来源：http://hz.hongshengwenyu.top/gtkttwnkrg.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.shanyushiyangkeji.top/gtrmofmunj.html

[U65] PHP：会话
来源：http://hz.cashguo.top/gtofturgve.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.hysaishi.cn/gtguipzbib.html

[U66] PHP：设置 Cookie
来源：http://hz.sufxvd.cn/gtarzpelhe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.gaohongyu789.top/gtowmenxqu.html

[U67] PHP：处理文件上传
来源：http://hz.zhijiandao.cn/gtnyklpoqu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.yj20258888.top/gtktfgaiin.html

[U68] PHP：PDO 连接
来源：http://hz.yonumen.top/gtninvgrzv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.chenjidiqi.icu/gtmxtvocxy.html

[U69] PHP：PDO 预处理
来源：http://hz.yonumen.top/gtsysjhimk.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gotoacloud.top/gtnjjivpum.html

[U70] PHP：PDO 事务
来源：http://hz.xinyue.icu/gtisiuetha.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xingfuxueyuan.xyz/gthgctnypc.html

[U71] PHP：抛出异常
来源：http://hz.zdqjudy.top/gtiegtdnrn.html

throw new RuntimeException("失败", 500);
来源：http://hz.shangyingyoupin.top/gtzycbgtuu.html

[U72] PHP：写错误日志
来源：http://hz.zhoulong.xyz/gtejupkxgo.html

error_log("失败: " . $e->getMessage());
来源：http://hz.jqgufenzy.top/gtvsofuvwn.html

[U73] PHP：读取 ini 配置
来源：http://hz.haohaochexian.top/gtslgsriil.html

parse_ini_file("config.ini", true)
来源：http://hz.gzhubu.top/gtxqvmptxd.html

[U74] PHP：读取环境变量
来源：http://hz.zhoulong.xyz/gtabrthgha.html

getenv("APP_ENV") ?: "production"
来源：http://hz.aibaodan.cn/gtjebsccnz.html

[U75] PHP：依赖注入
来源：http://hz.aizwys.cn/gtswkidaam.html

composer require psr/container
来源：http://hz.chenlongwang.top/gtwtgenvfw.html

[U76] PHP：简单路由
来源：http://hz.feifeiyinyue.top/gtierwtixx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.pycfn.com/gtuqfprxgw.html

[U77] PHP：模板渲染
来源：http://hz.0kj1m.cn/gtlracysgx.html

composer require twig/twig
来源：http://hz.ppjwa.cn/gtfaockuvv.html

[U78] PHP：单元测试
来源：http://hz.pycfn.com/gtkpblqbge.html

composer require --dev phpunit/phpunit
来源：http://hz.jinqigfzy.top/gtmuwumhyo.html

[U79] PHP：静态分析
来源：http://hz.andypj.xyz/gtjdibwgbs.html

composer require --dev phpstan/phpstan
来源：http://hz.sweek.top/gtxgkialzs.html

[U80] PHP：代码规范修复
来源：http://hz.cashguo.top/gtvifijbsp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.shangyingyoupin.top/gteromtzpo.html

[U81] JS：初始化项目
来源：http://hz.xuetiantiany.cn/gtymhfoawq.html

npm init -y;  npm i express
来源：http://hz.xingfuxueyuan.xyz/gtxzkczynx.html

[U82] JS：package.json 脚本
来源：http://hz.c1oappe.top/gttumsurld.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.pycfn.com/gtbqngopmu.html


<!-- 参考信息 -->