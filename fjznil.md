代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sweek.top/gtoyouzpvg.html

[S57] C++：编译期常量
来源：http://hz.cucudq.cn/gtprlwexoy.html

constexpr int N = 10;
来源：http://hz.c1oappe.top/gtrxvogfqn.html

[S58] C++：命名空间
来源：http://hz.sxryk.cn/gtezhddbmq.html

namespace ns { int f() { return 1; } }
来源：http://hz.dashuyun.cn/gtlfdixyoa.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gttnnwlauo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ehwqpu.com/gtcshxuhoo.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigufen.top/gtyjwwjyme.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hnqzz.top/gtzgnwweqq.html

================================================================================
来源：http://hz.jqgfzy.top/gtxbeimhdp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fzhhl.top/gtccxhnwdr.html

================================================================================
来源：http://hz.hnqzz.top/gtxghhdajx.html

[T01] Kotlin：Hello World
来源：http://hz.chenzaomai.com/gtbegfigzf.html

println("Hello")
来源：http://hz.hnqzz.top/gtlnnahnje.html

[T02] Kotlin：变量
来源：http://hz.gotoacloud.top/gtfuszzmfx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aizwys.cn/gtngzszobl.html

[T03] Kotlin：字符串模板
来源：http://hz.hongshengwenyu.top/gtlhuuzfws.html

"值: $b"
来源：http://hz.redwolf501.top/gtshwsbzsp.html

[T04] Kotlin：空安全
来源：http://hz.sxryk.cn/gtxrixgjvr.html

val n: String? = null;  n?.length
来源：http://hz.hnxiangtu.top/gtvhbhkowd.html

[T05] Kotlin：when 表达式
来源：http://hz.meibo888.top/gtqpbbkyub.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cucudq.cn/gttcvsgpdl.html

[T06] Kotlin：集合映射
来源：http://hz.wangshuangyany.cn/gtxnvexngz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sufxvd.cn/gtygnfpvhp.html

[T07] Kotlin：集合过滤
来源：http://hz.shangyingyoupin.top/gtghhbmtds.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigfzy.top/gtfrkcjdjc.html

[T08] Kotlin：数据类
来源：http://hz.shuidangran.top/gtqgcshmfn.html

data class User(val name: String, val age: Int)
来源：http://hz.cdnleiting.top/gtxolbryqn.html

[T09] Kotlin：扩展函数
来源：http://hz.tian-w.cn/gtlebbaqcu.html

fun String.exclaim() = this + "!"
来源：http://hz.xylfe.cn/gtxfikbwny.html

[T10] Kotlin：默认参数
来源：http://hz.yuanzhike.top/gtwyxgpjbx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.dashuyun.cn/gtqtzhrofi.html

[T11] Kotlin：协程
来源：http://hz.guowangkeji.top/gtsyhnmuka.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydzc1.top/gtstrpneqh.html

[T12] Kotlin：解构声明
来源：http://hz.ydzc1.top/gtcildznur.html

val (a, b) = Pair(1, 2)
来源：http://hz.fengsongda.top/gteevyarve.html

[T13] Kotlin：只读 Map
来源：http://hz.xziqi.cn/gtgancswrf.html

val m = mapOf("a" to 1)
来源：http://hz.hnqzz.top/gtfkibvewp.html

[T14] Kotlin：循环
来源：http://hz.yueranfly.top/gtkbkpvbdp.html

for (i in 1..10) println(i)
来源：http://hz.zdqjudy.top/gtcnygeifi.html

[T15] Kotlin：接口
来源：http://hz.ydzc1.top/gtherqjpao.html

interface Shape { fun area(): Double }
来源：http://hz.fengsongda.top/gtebromdki.html

[T16] Swift：Hello World
来源：http://hz.zhengqikj.top/gtguptkyya.html

print("Hello")
来源：http://hz.zhoulong.xyz/gtpssdzqli.html

[T17] Swift：变量与常量
来源：http://hz.mhx1999.top/gtodpztcdc.html

var a = 1;  let b = 2
来源：http://hz.hywenlv.cn/gtrmuliiwn.html

[T18] Swift：字符串插值
来源：http://hz.shuidangran.top/gtctfizdbo.html

"值: \(b)"
来源：http://hz.zhengqikj.top/gtuljvmtwk.html

[T19] Swift：可选绑定
来源：http://hz.yuxming.cn/gtdyulzljp.html

if let n = opt { print(n) }
来源：http://hz.yuxming.cn/gtuyhacdtc.html

[T20] Swift：数组操作
来源：http://hz.zhiwuduotai.top/gthpedyojs.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.bjfxy.top/gtghiimwsx.html

[T21] Swift：遍历
来源：http://hz.0kj1m.cn/gtofohxjga.html

for x in a { print(x) }
来源：http://hz.jinqigfzy.top/gtwigomtjs.html

[T22] Swift：字典
来源：http://hz.yanxiufei.cn/gtsudddyjw.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.haohaochexian.top/gtkmdqucgy.html

[T23] Swift：函数
来源：http://hz.yj202588.top/gtjrqonhdw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hywenlv.cn/gtcdznjkiv.html

[T24] Swift：闭包
来源：http://hz.chenzaomai.com/gtdjplastc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.birdmap.top/gtezfeeoqf.html

[T25] Swift：结构体
来源：http://hz.ydzc1.top/gttjduujeh.html

struct P { var x: Int }
来源：http://hz.yanxiufei.cn/gtiggldzoe.html

[T26] Swift：类与重写
来源：http://hz.shangyingyoupin.top/gtbgbfwflo.html

class A: Base { override func f() {} }
来源：http://hz.birdmap.top/gtraigriis.html

[T27] Swift：错误处理
来源：http://hz.hnqzz.top/gthovrrpcz.html

do { try f() } catch { print(error) }
来源：http://hz.jinqigfzy.top/gtoutvqbyk.html

[T28] Swift：枚举
来源：http://hz.sufxvd.cn/gthhyoymxy.html

enum Color { case red, green }
来源：http://hz.pycfn.com/gtspjutpfz.html

[T29] Swift：guard 提前返回
来源：http://hz.svipenyu.cn/gtxiynvxqd.html

guard let x = opt else { return }
来源：http://hz.daxiang520.top/gtdwgsqtca.html

[T30] Swift：协议
来源：http://hz.jiagoushi.top/gtdwagqisz.html

protocol Shape { func area() -> Double }
来源：http://hz.shanyushiyangkeji.top/gtwvsvmvpj.html

[T31] Lua：Hello World
来源：http://hz.havefunace.top/gtyqrfvpbg.html

print("Hello")
来源：http://hz.ywan-chungtsiang.top/gtlvszmofh.html

[T32] Lua：局部变量
来源：http://hz.ppjwa.cn/gtyzglynhr.html

local a = 1
来源：http://hz.xingfuxueyuan.xyz/gtuiqifcgf.html

[T33] Lua：表（数组）
来源：http://hz.hnxiangtu.top/gtlqcmokuh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.dashuyun.cn/gtrqiuxsfn.html

[T34] Lua：遍历表
来源：http://hz.vqdsnc.cn/gtlqfzqbrj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.pengpengdd.cyou/gtueezwtsm.html

[T35] Lua：字典表
来源：http://hz.ywan-chungtsiang.top/gtxmeformx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.jlsjyb.cn/gtnlzabrbd.html

[T36] Lua：函数
来源：http://hz.shangyingyoupin.top/gtherfdntf.html

function add(a, b) return a + b end
来源：http://hz.dianchejie.cn/gtvqfpthrr.html

[T37] Lua：字符串拼接
来源：http://hz.nanxuanxn.top/gtfaifeqna.html

"a" .. "b"
来源：http://hz.xuetiantiany.cn/gtxmsgaaby.html

[T38] Lua：条件
来源：http://hz.chenzaomai.com/gtkeqlzjkp.html

if x > 0 then print("正") end
来源：http://hz.shanyushiyangkeji.top/gtwqsaaokt.html

[T39] Lua：模式匹配
来源：http://hz.smart0.xyz/gtpkjvhwhb.html

string.find(s, "%d+")
来源：http://hz.shzxlz.cn/gtkyzjrzqz.html

[T40] Lua：元表
来源：http://hz.yvedp.cn/gtcnejnwrs.html

setmetatable({}, { __index = base })
来源：http://hz.yangfankeji.com/gtzqvlnjwt.html

[T41] Perl：Hello World
来源：http://hz.feifeiyinyue.top/gtcfmarbxk.html

print "Hello\n";
来源：http://hz.pycfn.com/gtwkjiobmn.html

[T42] Perl：变量类型
来源：http://hz.ybcxt.top/gtiqighxcn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.vqdsnc.cn/gtrzqtfpit.html

[T43] Perl：字符串插值
来源：http://hz.sxryk.cn/gtkchlftbf.html

"值: $a"
来源：http://hz.yvedp.cn/gtaqyjirtu.html

[T44] Perl：条件
来源：http://hz.xuanzx.com/gttpulligz.html

if ($a > 0) { print "正"; }
来源：http://hz.chenjidiqi.icu/gtbustlkqw.html

[T45] Perl：数组遍历
来源：http://hz.hnqzz.top/gtwzktfgnm.html

for my $x (@arr) { print $x; }
来源：http://hz.sweek.top/gtwbqwqjjs.html

[T46] Perl：哈希操作
来源：http://hz.ivvv.top/gtxniwwibq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhongyouzk.top/gtupixiuuh.html

[T47] Perl：正则捕获
来源：http://hz.yanxiufei.cn/gthssxcdzm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.pycfn.com/gtqysymwtc.html

[T48] Perl：正则替换
来源：http://hz.zhiwuduotai.top/gtdabfvmrl.html

$s =~ s/old/new/g;
来源：http://hz.havefunace.top/gttveijeih.html

[T49] Perl：函数
来源：http://hz.wangshuangyany.cn/gtyothwwux.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.gogol.net.cn/gthlxuhpsd.html

[T50] Perl：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtnmrznxul.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yangfankeji.com/gtnpuaxwwa.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.bjfxy.top/gtnjdamaoq.html

[T51] Scala：Hello World
来源：http://hz.guannengcc.top/gtgmrvgexw.html

println("Hello")
来源：http://hz.yongpay.top/gtywphnonr.html

[T52] Scala：变量
来源：http://hz.sufxvd.cn/gttphvhkiy.html

val a = 1;  var b = 2
来源：http://hz.tian-w.cn/gtxsyibfhr.html

[T53] Scala：字符串插值
来源：http://hz.jyoumei.cn/gtjqnwjbmo.html

s"值: $b"
来源：http://hz.jlsjyb.cn/gthixddkxh.html

[T54] Scala：集合映射
来源：http://hz.jinqigufen.top/gtgolosgot.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.xziqi.cn/gtsecfbozu.html

[T55] Scala：集合过滤
来源：http://hz.shangyingyoupin.top/gtkxkqbjvt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.nanxuanxn.top/gtxurpgyel.html

[T56] Scala：样例类
来源：http://hz.aizwys.cn/gttiuoaxqq.html

case class User(name: String, age: Int)
来源：http://hz.dashuyun.cn/gthnqstpxy.html

[T57] Scala：模式匹配
来源：http://hz.cdnleiting.top/gtwkmmltiw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.jinghuilouyu.cn/gtkqxralxo.html

[T58] Scala：函数定义
来源：http://hz.cdnleiting.top/gthdayzpzg.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.zhixingplan.top/gtlhydwvpi.html

[T59] Scala：循环
来源：http://hz.zhongyouzk.top/gtqpvowmtc.html

for (i <- 1 to 10) println(i)
来源：http://hz.hnxiangtu.top/gtoovidklz.html

[T60] Scala：折叠
来源：http://hz.sweek.top/gtkkdcigpx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.hongshengwenyu.top/gthtnzsigb.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtweqnckom.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gtizmtqysa.html

================================================================================
来源：http://hz.mhx1999.top/gtnynvhuzy.html

[U01] Py：创建虚拟环境
来源：http://hz.jianghu66.top/gtghtcpcvi.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.haohaochexian.top/gtbevtcfli.html

[U02] Py：导出 / 安装依赖
来源：http://hz.mhx1999.top/gtcviqhfwy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.pengpengdd.cyou/gtjysrfraa.html

[U03] Py：加载 .env 配置
来源：http://hz.yuxming.cn/gtvutbbalt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shzxlz.cn/gtivsnctck.html

[U04] Py：变量调试打印
来源：http://hz.hnxiangtu.top/gtzgbuzlnl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zdqjudy.top/gtfjbzsemm.html

[U05] Py：列表去重且保序
来源：http://hz.ppjwa.cn/gthpgptrwv.html

list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtehqurerr.html

[U06] Py：合并两个字典
来源：http://hz.shuidangran.top/gtgxhdcgla.html

{**a, **b}
来源：http://hz.jqgfzy.top/gtlhskwibk.html

[U07] Py：反转字典键值
来源：http://hz.wangdashe.top/gtgshmmome.html

{v: k for k, v in d.items()}
来源：http://hz.jqgfzy.top/gtulerarum.html

[U08] Py：展平二维列表
来源：http://hz.hysaishi.cn/gtlmktllbl.html

[y for x in nested for y in x]
来源：http://hz.xuetiantiany.cn/gtesrjgqhb.html

[U09] Py：字典取最大值的键
来源：http://hz.cqqwz.cn/gtbidtqxqj.html

max(d, key=d.get)
来源：http://hz.daxiang520.top/gtggndmspy.html

[U10] Py：按值排序字典
来源：http://hz.xinyue.icu/gttptbnxyw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.birdmap.top/gttebudazd.html

[U11] Py：生成器表达式
来源：http://hz.316326.xyz/gtqnncvfgt.html

(x * 2 for x in arr)
来源：http://hz.0kj1m.cn/gtjanoagqa.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.ywan-chungtsiang.top/gtjeiymjre.html

Counter(arr).most_common(3)
来源：http://hz.hfpthk.cn/gtmjonvocn.html

[U13] Py：固定长度队列
来源：http://hz.xuetiantiany.cn/gtutwooksr.html

deque(maxlen=10)
来源：http://hz.dianchejie.cn/gtmyrgymho.html

[U14] Py：分组收集到列表
来源：http://hz.havefunace.top/gtepgagxdf.html

defaultdict(list)
来源：http://hz.chenjidiqi.icu/gtqtfvotma.html

[U15] Py：高精度计时
来源：http://hz.shuidangran.top/gtdkuydmhh.html

t = time.perf_counter()
来源：http://hz.zhiwuduotai.top/gtuwfsmzum.html

[U16] Py：命令行参数解析
来源：http://hz.daxiang520.top/gtddpwxhgu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.tanke756.top/gtrbakvpcw.html

[U17] Py：初始化日志
来源：http://hz.cashguo.top/gtxbuiapim.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.yangfankeji.com/gtclvoxexf.html

[U18] Py：预编译正则
来源：http://hz.zhijiandao.cn/gtodojnbay.html

pat = re.compile(r"\d+")
来源：http://hz.hammf.cn/gtjygrznhr.html

[U19] Py：正则替换带回调
来源：http://hz.daxiang520.top/gtcfhiambo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.zhixingplan.top/gttqzzrilo.html

[U20] Py：缓存函数结果
来源：http://hz.gotoacloud.top/gtzldnlrqt.html

@functools.lru_cache(maxsize=None)
来源：http://hz.jinyuanbaomall.cn/gtbaiaywrc.html

[U21] Py：自定义上下文管理器
来源：http://hz.ywan-chungtsiang.top/gtqlfeqhxz.html

@contextlib.contextmanager
来源：http://hz.yonumen.top/gtyyjlqqkn.html

[U22] Py：矩阵转置
来源：http://hz.andypj.xyz/gtxnnrwbcv.html

list(zip(*m))
来源：http://hz.iojbl.cn/gtdtywtlvx.html

[U23] Py：分块读取大文件
来源：http://hz.yj20258.top/gtvlextrtg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.pengpengdd.cyou/gtbfqxlhoc.html

[U24] Py：路径操作
来源：http://hz.pycfn.com/gtiohaukvv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.fengsongda.top/gtnudrztmq.html

[U25] Py：CSV 按字典读
来源：http://hz.cheryme.top/gtuwnkjiwr.html

csv.DictReader(f)
来源：http://hz.ppjwa.cn/gtsbwwjgzf.html

[U26] Py：并发下载
来源：http://hz.daxiang520.top/gtqnqfmupq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.svipenyu.cn/gtlqcrqwlb.html

[U27] Py：异步 HTTP
来源：http://hz.yuanzhike.top/gtqktzinzt.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.ppjwa.cn/gtogimbuix.html

[U28] Py：类型别名
来源：http://hz.bjfxy.top/gtdedsqrvc.html

UserId = int
来源：http://hz.cqqwz.cn/gtubakvpyi.html

[U29] Py：属性校验
来源：http://hz.jlsjyb.cn/gttvljmpvi.html

@property 与 @x.setter 配合
来源：http://hz.tian-w.cn/gtfoepzngh.html

[U30] Py：数据类
来源：http://hz.vqdsnc.cn/gtvwfksghn.html

@dataclass(slots=True)
来源：http://hz.xziqi.cn/gtyhcgyahw.html

[U31] Py：单测
来源：http://hz.yueranfly.top/gtijgewuhm.html

python -m pytest -q
来源：http://hz.cqqwz.cn/gtqiwpxhxx.html

[U32] Py：代码格式化
来源：http://hz.tanke756.top/gtzdygehsp.html

ruff format . && ruff check --fix .
来源：http://hz.chenlongwang.top/gtvcaevaax.html

[U33] Py：打包发布
来源：http://hz.hywenlv.cn/gteqwhofog.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.chenlongwang.top/gtwslhkyzd.html

[U34] Py：判断编码
来源：http://hz.kuanghao11.cn/gtbgdjadtu.html

chardet.detect(raw)
来源：http://hz.jyoumei.cn/gtdwjahjjo.html

[U35] Py：发送邮件
来源：http://hz.hysaishi.cn/gtiaeprrtl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.ivvv.top/gtjexhncxf.html

[U36] Py：定时任务
来源：http://hz.nwbrower.top/gtjnpcyrfo.html

schedule.every(10).minutes.do(job)
来源：http://hz.shanyushiyangkeji.top/gtwkyuqkru.html

[U37] Py：读写 Excel
来源：http://hz.dashuyun.cn/gtmcowsrjl.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.sweek.top/gtsmoyoqmb.html

[U38] Py：获取脚本所在目录
来源：http://hz.yuanzhike.top/gtbfvgyyvi.html

Path(__file__).resolve().parent
来源：http://hz.guannengcc.top/gtjyvntrzt.html

[U39] Py：判断是否在交互环境
来源：http://hz.hammf.cn/gttdlmzecp.html

sys.stdout.isatty()
来源：http://hz.jiagoushi.top/gtrhzbhihz.html

[U40] Py：打印到标准错误
来源：http://hz.andypj.xyz/gtdlwjphkk.html

print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtmfndasfl.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.cheryme.top/gtoboajygu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.xinyue.icu/gtcbdbkfhl.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.jiagoushi.top/gtssqbfgwj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.jqgfzy.top/gtokbpvnhk.html

[U43] PHP：声明命名空间
来源：http://hz.316326.xyz/gtzttgjsni.html

namespace App\Http;
来源：http://hz.zhiwuduotai.top/gtvbeggtps.html

[U44] PHP：开启严格类型
来源：http://hz.iojbl.cn/gthgeevjwz.html

declare(strict_types=1);
来源：http://hz.shanyushiyangkeji.top/gtlwidsncs.html

[U45] PHP：类型声明与返回类型
来源：http://hz.hnqzz.top/gtyyogsduz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shuidangran.top/gthveufmtt.html

[U46] PHP：可空类型
来源：http://hz.yuanzhike.top/gttgbaoznq.html

?string $name = null
来源：http://hz.yj20258.top/gtkacwlefd.html

[U47] PHP：联合类型
来源：http://hz.jinyuanbaomall.cn/gtuzftdbyh.html

int|string $id
来源：http://hz.ywan-chungtsiang.top/gtbpmlitef.html

[U48] PHP：纯枚举
来源：http://hz.zhoulong.xyz/gtypbgebso.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.ehwqpu.com/gtmkjomxnp.html

[U49] PHP：只读属性
来源：http://hz.vqdsnc.cn/gtcgyfcqpw.html

public readonly string $name
来源：http://hz.jinqigufen.top/gtsauogaxe.html

[U50] PHP：构造器属性提升
来源：http://hz.cdnleiting.top/gtybhsucaq.html

public function __construct(private int $id) {}
来源：http://hz.316326.xyz/gthvwnklih.html

[U51] PHP：数组解构
来源：http://hz.mhx1999.top/gtajskpmcy.html

[$a, $b] = $arr;
来源：http://hz.hammf.cn/gtqswjinhb.html

[U52] PHP：箭头函数
来源：http://hz.cheryme.top/gtketuyqti.html

$double = fn($x) => $x * 2;
来源：http://hz.jinqigufen.top/gtjomchdvd.html

[U53] PHP：空合并运算符
来源：http://hz.ywan-chungtsiang.top/gtlkpsxxzb.html

$v = $a ?? $b ?? "default";
来源：http://hz.hnxiangtu.top/gtvajjgenn.html

[U54] PHP：空安全调用
来源：http://hz.ehwqpu.com/gtwogfbnuj.html

$obj?->method()
来源：http://hz.svipenyu.cn/gtozdsowix.html

[U55] PHP：match 表达式
来源：http://hz.dashuyun.cn/gtoqzjiulz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.yangfankeji.com/gthxawbnct.html

[U56] PHP：命名参数
来源：http://hz.jinghuilouyu.cn/gtmdlvwmki.html

f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gtewznhybm.html

[U57] PHP：字符串插值
来源：http://hz.yongpay.top/gtvphlhrze.html

"值: {$a}"
来源：http://hz.havefunace.top/gttngtmbzn.html

[U58] PHP：数组三件套
来源：http://hz.ywan-chungtsiang.top/gtlgqpuavs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.daria6918.cn/gtoktznplc.html

[U59] PHP：自定义排序
来源：http://hz.chenzaomai.com/gthboaxqsx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuanzx.com/gtxkxgeprg.html

[U60] PHP：JSON 编解码
来源：http://hz.sufxvd.cn/gtgdmqvnvl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.jiagoushi.top/gtqygqohpc.html

[U61] PHP：正则
来源：http://hz.andypj.xyz/gtnlomaibn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhongyouzk.top/gtfccsgced.html

[U62] PHP：日期对象
来源：http://hz.bjfxy.top/gtxsivbkxb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.52xcode.cn/gtmhstyvyt.html

[U63] PHP：文件读写
来源：http://hz.316326.xyz/gttwutzsrx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.daxiang520.top/gtxkxphmvw.html

[U64] PHP：目录遍历
来源：http://hz.chenjidiqi.icu/gtygrozfbc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.9152youxi.cn/gtznedidlu.html

[U65] PHP：会话
来源：http://hz.sufxvd.cn/gtuqgidedb.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.andypj.xyz/gtzxnijesb.html

[U66] PHP：设置 Cookie
来源：http://hz.snrcjt.cn/gtjazzxesx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.yuanzhike.top/gtwhyurpki.html

[U67] PHP：处理文件上传
来源：http://hz.fzhhl.top/gtonjgoinj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zycfv.cn/gtrdisrjes.html

[U68] PHP：PDO 连接
来源：http://hz.quarkkingdee.top/gtwsoxcrpm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.xinyue.icu/gtkuoftcxv.html

[U69] PHP：PDO 预处理
来源：http://hz.zhoulong.xyz/gtufgatfnv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.daxiang520.top/gtfmzwwfro.html

[U70] PHP：PDO 事务
来源：http://hz.zhaomingkeji.xyz/gtqfxuhurh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.jyoumei.cn/gtviiyntnx.html

[U71] PHP：抛出异常
来源：http://hz.nanxinkj.top/gterwmvhqm.html

throw new RuntimeException("失败", 500);
来源：http://hz.yonumen.top/gtdobaaorx.html

[U72] PHP：写错误日志
来源：http://hz.jinqigufen.top/gtgfahpazw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ivvv.top/gtzlcpvcle.html

[U73] PHP：读取 ini 配置
来源：http://hz.xingfuxueyuan.xyz/gtwrqzedmw.html

parse_ini_file("config.ini", true)
来源：http://hz.zdqjudy.top/gtptswyeag.html

[U74] PHP：读取环境变量
来源：http://hz.xuanzx.com/gtriikmqzl.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zhaomingkeji.xyz/gtcuvodima.html

[U75] PHP：依赖注入
来源：http://hz.guannengcc.top/gtsjneggpg.html

composer require psr/container
来源：http://hz.yongpay.top/gtwcvmwkif.html

[U76] PHP：简单路由
来源：http://hz.hnqzz.top/gtokmfddzp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.shanyushiyangkeji.top/gtrszfyema.html

[U77] PHP：模板渲染
来源：http://hz.gotoacloud.top/gtsyvmuqvn.html

composer require twig/twig
来源：http://hz.sysykeji.top/gtjazzsthn.html

[U78] PHP：单元测试
来源：http://hz.jyoumei.cn/gtdqepqsge.html

composer require --dev phpunit/phpunit
来源：http://hz.yuanzhike.top/gtzregurrd.html

[U79] PHP：静态分析
来源：http://hz.dashuyun.cn/gtecytzdum.html

composer require --dev phpstan/phpstan
来源：http://hz.hfpthk.cn/gtkjsrlgpn.html

[U80] PHP：代码规范修复
来源：http://hz.zhixingplan.top/gtjelqqqpe.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.pengpengdd.cyou/gtqcemilsu.html

[U81] JS：初始化项目
来源：http://hz.zhijiandao.cn/gtqkjkwzqk.html

npm init -y;  npm i express
来源：http://hz.svipenyu.cn/gtaqkarnau.html

[U82] JS：package.json 脚本
来源：http://hz.wangdashe.top/gtczqzqrxn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.svipenyu.cn/gtbpghahjg.html


<!-- 参考信息 -->