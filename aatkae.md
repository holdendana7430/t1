代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinyuanbaomall.cn/gtzjxbktvj.html

[S57] C++：编译期常量
来源：http://hz.nanxuanxn.top/gtwiwzsupj.html

constexpr int N = 10;
来源：http://hz.jinqigfzy.top/gtnmcmvlbg.html

[S58] C++：命名空间
来源：http://hz.shzxlz.cn/gtwtalvcdy.html

namespace ns { int f() { return 1; } }
来源：http://hz.gotoacloud.top/gtyasyfrwj.html

[S59] C++：静态断言
来源：http://hz.feifeiyinyue.top/gttlalpies.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj202588.top/gtzzybeoxl.html

[S60] C++：遍历并删除元素
来源：http://hz.havefunace.top/gtrogldepv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gzhubu.top/gtfzafbjuv.html

================================================================================
来源：http://hz.nanxinkj.top/gtrojwgznr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.chenjidiqi.icu/gtfmgtkbwx.html

================================================================================
来源：http://hz.aizwys.cn/gtoggzrvxu.html

[T01] Kotlin：Hello World
来源：http://hz.jqgfzy.top/gtvkyuxkav.html

println("Hello")
来源：http://hz.52xcode.cn/gtomonqkpz.html

[T02] Kotlin：变量
来源：http://hz.0kj1m.cn/gtpbxggdmw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ywan-chungtsiang.top/gtelczkmpl.html

[T03] Kotlin：字符串模板
来源：http://hz.jqgufenzy.top/gtxdewumvl.html

"值: $b"
来源：http://hz.tanke756.top/gtrabzulhc.html

[T04] Kotlin：空安全
来源：http://hz.pengpengdd.cyou/gttkupkiuz.html

val n: String? = null;  n?.length
来源：http://hz.ppjwa.cn/gteceberlq.html

[T05] Kotlin：when 表达式
来源：http://hz.yongpay.top/gtszodtkcd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hywenlv.cn/gtafwgxlpv.html

[T06] Kotlin：集合映射
来源：http://hz.chenjidiqi.icu/gtlcavtkzi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.guowangkeji.top/gtjxfmnbse.html

[T07] Kotlin：集合过滤
来源：http://hz.cheryme.top/gtnlhlrbcu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.pengpengdd.cyou/gtdkqcalre.html

[T08] Kotlin：数据类
来源：http://hz.dianchejie.cn/gtlixgdrgp.html

data class User(val name: String, val age: Int)
来源：http://hz.havefunace.top/gtfoklbpnv.html

[T09] Kotlin：扩展函数
来源：http://hz.haohaochexian.top/gtcgdbybqa.html

fun String.exclaim() = this + "!"
来源：http://hz.xingfuxueyuan.xyz/gtxjwlqxil.html

[T10] Kotlin：默认参数
来源：http://hz.jianghu66.top/gthjgcppkc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.fzhhl.top/gtihtrgnck.html

[T11] Kotlin：协程
来源：http://hz.svipenyu.cn/gtgxjyhobt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.quarkkingdee.top/gtbalajren.html

[T12] Kotlin：解构声明
来源：http://hz.zhiwuduotai.top/gtzuvzgzcr.html

val (a, b) = Pair(1, 2)
来源：http://hz.redwolf501.top/gtuycnaczy.html

[T13] Kotlin：只读 Map
来源：http://hz.sufxvd.cn/gtmknvjgzc.html

val m = mapOf("a" to 1)
来源：http://hz.xuetiantiany.cn/gtqsfnpzyd.html

[T14] Kotlin：循环
来源：http://hz.nanxuanxn.top/gtzbxmqxyz.html

for (i in 1..10) println(i)
来源：http://hz.jinqigfzy.top/gtgdjdrfmd.html

[T15] Kotlin：接口
来源：http://hz.sysykeji.top/gtvdawdriw.html

interface Shape { fun area(): Double }
来源：http://hz.yuanzhike.top/gtauazkytm.html

[T16] Swift：Hello World
来源：http://hz.aibaodan.cn/gtgkcihksh.html

print("Hello")
来源：http://hz.chenzaomai.com/gtupqoegfj.html

[T17] Swift：变量与常量
来源：http://hz.52xcode.cn/gtzhlmkoaz.html

var a = 1;  let b = 2
来源：http://hz.zhaomingkeji.xyz/gtkugwslpw.html

[T18] Swift：字符串插值
来源：http://hz.hfpthk.cn/gthbvesfnu.html

"值: \(b)"
来源：http://hz.jiagoushi.top/gtlalzaqjo.html

[T19] Swift：可选绑定
来源：http://hz.pycfn.com/gtinimpkzr.html

if let n = opt { print(n) }
来源：http://hz.aizwys.cn/gtemddclbj.html

[T20] Swift：数组操作
来源：http://hz.zhengqikj.top/gtidjxfhyi.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yueranfly.top/gtsorqrkms.html

[T21] Swift：遍历
来源：http://hz.nanxinkj.top/gtkmulxues.html

for x in a { print(x) }
来源：http://hz.yongpay.top/gtdrfdjctu.html

[T22] Swift：字典
来源：http://hz.hammf.cn/gttgryvqup.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sufxvd.cn/gtgnwrxqeb.html

[T23] Swift：函数
来源：http://hz.316326.xyz/gtvijaevfa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cheryme.top/gtzswbxwdz.html

[T24] Swift：闭包
来源：http://hz.redwolf501.top/gteerlmbpp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.mhx1999.top/gtobzamqpo.html

[T25] Swift：结构体
来源：http://hz.9152youxi.cn/gtqbxgjkab.html

struct P { var x: Int }
来源：http://hz.ybcxt.top/gtplulopnv.html

[T26] Swift：类与重写
来源：http://hz.bjfxy.top/gtogbxsgym.html

class A: Base { override func f() {} }
来源：http://hz.52xcode.cn/gtedloakya.html

[T27] Swift：错误处理
来源：http://hz.zhiwuduotai.top/gtkcgtttwi.html

do { try f() } catch { print(error) }
来源：http://hz.hywenlv.cn/gtmzwbyniy.html

[T28] Swift：枚举
来源：http://hz.meibo888.top/gtjshwjnjw.html

enum Color { case red, green }
来源：http://hz.nanxuanxn.top/gtoubijqqs.html

[T29] Swift：guard 提前返回
来源：http://hz.smart0.xyz/gtyihbgndg.html

guard let x = opt else { return }
来源：http://hz.gotoacloud.top/gtgwohinvc.html

[T30] Swift：协议
来源：http://hz.xziqi.cn/gtnqkdyswf.html

protocol Shape { func area() -> Double }
来源：http://hz.sxryk.cn/gtswicnhju.html

[T31] Lua：Hello World
来源：http://hz.guannengcc.top/gtcxaugbxc.html

print("Hello")
来源：http://hz.zhijiandao.cn/gtfmyefjmb.html

[T32] Lua：局部变量
来源：http://hz.xinyue.icu/gtbfvmtmen.html

local a = 1
来源：http://hz.yuanzhike.top/gtrrkkigeu.html

[T33] Lua：表（数组）
来源：http://hz.sxryk.cn/gtoglqmdhy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xinyue.icu/gtfhugikao.html

[T34] Lua：遍历表
来源：http://hz.jiagoushi.top/gtcygphpdo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.yj20258888.top/gtwwrsrrse.html

[T35] Lua：字典表
来源：http://hz.zdqjudy.top/gtzjuwvice.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gaohongyu789.top/gttzofelzp.html

[T36] Lua：函数
来源：http://hz.andypj.xyz/gtdjyznwls.html

function add(a, b) return a + b end
来源：http://hz.yongpay.top/gtczxhvqxv.html

[T37] Lua：字符串拼接
来源：http://hz.yueranfly.top/gtpimwgrmo.html

"a" .. "b"
来源：http://hz.cucudq.cn/gtryrmawcj.html

[T38] Lua：条件
来源：http://hz.dianchejie.cn/gteyyayqil.html

if x > 0 then print("正") end
来源：http://hz.pycfn.com/gtvcxbdrlg.html

[T39] Lua：模式匹配
来源：http://hz.chenzaomai.com/gtskknwyxs.html

string.find(s, "%d+")
来源：http://hz.wangshuangyany.cn/gtxlyddobp.html

[T40] Lua：元表
来源：http://hz.jinghuilouyu.cn/gtxhzniuvw.html

setmetatable({}, { __index = base })
来源：http://hz.bjfxy.top/gthffturiq.html

[T41] Perl：Hello World
来源：http://hz.snrcjt.cn/gtakvmwwhk.html

print "Hello\n";
来源：http://hz.yvedp.cn/gtbyhhvtty.html

[T42] Perl：变量类型
来源：http://hz.cdnleiting.top/gttwmakbue.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.jiagoushi.top/gtldspywte.html

[T43] Perl：字符串插值
来源：http://hz.andypj.xyz/gtojyzcdwg.html

"值: $a"
来源：http://hz.316326.xyz/gtmlfrkzby.html

[T44] Perl：条件
来源：http://hz.yanxiufei.cn/gtwsyjdixa.html

if ($a > 0) { print "正"; }
来源：http://hz.dianchejie.cn/gtaxhwbjof.html

[T45] Perl：数组遍历
来源：http://hz.jinqigfzy.top/gtaqjiyrnw.html

for my $x (@arr) { print $x; }
来源：http://hz.mhx1999.top/gtlmuirace.html

[T46] Perl：哈希操作
来源：http://hz.guannengcc.top/gtmbvhstun.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.shzxlz.cn/gtryfjhwre.html

[T47] Perl：正则捕获
来源：http://hz.chenlongwang.top/gtugfgxxke.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.sxryk.cn/gtgcocsdml.html

[T48] Perl：正则替换
来源：http://hz.52xcode.cn/gtctlnzfai.html

$s =~ s/old/new/g;
来源：http://hz.9152youxi.cn/gtrrvseblr.html

[T49] Perl：函数
来源：http://hz.ydzc1.top/gtddymobgk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.tian-w.cn/gtrfuspsbg.html

[T50] Perl：逐行读文件
来源：http://hz.shanyushiyangtech.top/gttfraoruz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.svipenyu.cn/gtfmufsywf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shanyushiyangtech.top/gtkcuegsxo.html

[T51] Scala：Hello World
来源：http://hz.redwolf501.top/gtpuldclya.html

println("Hello")
来源：http://hz.zhengqikj.top/gtreqpkxch.html

[T52] Scala：变量
来源：http://hz.daria6918.cn/gtijedwory.html

val a = 1;  var b = 2
来源：http://hz.hnqzz.top/gtsuaixwmj.html

[T53] Scala：字符串插值
来源：http://hz.guowangkeji.top/gtcaahlnfh.html

s"值: $b"
来源：http://hz.snrcjt.cn/gtreynsxma.html

[T54] Scala：集合映射
来源：http://hz.yj20258.top/gtrfckroep.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.tianlin.xyz/gtyakfcrce.html

[T55] Scala：集合过滤
来源：http://hz.vqdsnc.cn/gthydbtmhm.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.ydjk.org.cn/gtrfsfzboy.html

[T56] Scala：样例类
来源：http://hz.aibaodan.cn/gtveggnfgx.html

case class User(name: String, age: Int)
来源：http://hz.iojbl.cn/gtkvzezbuv.html

[T57] Scala：模式匹配
来源：http://hz.52xcode.cn/gtltkzcwyo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.cashguo.top/gtjnjhskgo.html

[T58] Scala：函数定义
来源：http://hz.wangdashe.top/gtkqzwfjtk.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.bjfxy.top/gthmnqkebb.html

[T59] Scala：循环
来源：http://hz.ppjwa.cn/gtgqkqddhn.html

for (i <- 1 to 10) println(i)
来源：http://hz.sufxvd.cn/gtkhgpqjsj.html

[T60] Scala：折叠
来源：http://hz.yvedp.cn/gtetskiuqk.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.ywan-chungtsiang.top/gtdmzkjouq.html

================================================================================
来源：http://hz.guannengcc.top/gtatqecjyg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.xziqi.cn/gtiknsghxt.html

================================================================================
来源：http://hz.zhoulong.xyz/gtwqyhyryx.html

[U01] Py：创建虚拟环境
来源：http://hz.0kj1m.cn/gtgvejyqiv.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.zhengqikj.top/gtggrbtlzi.html

[U02] Py：导出 / 安装依赖
来源：http://hz.zhixingplan.top/gthgfrhbet.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.gzhubu.top/gtozstkkud.html

[U03] Py：加载 .env 配置
来源：http://hz.fengsongda.top/gtgrljvili.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.shanyushiyangtech.top/gtsdgkqpgu.html

[U04] Py：变量调试打印
来源：http://hz.quarkkingdee.top/gtdfxvycch.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.zhiwuduotai.top/gtxsaqyipd.html

[U05] Py：列表去重且保序
来源：http://hz.tanke756.top/gturshfhth.html

list(dict.fromkeys(arr))
来源：http://hz.haohaochexian.top/gtqycctooi.html

[U06] Py：合并两个字典
来源：http://hz.daria6918.cn/gtmuwmdrtx.html

{**a, **b}
来源：http://hz.xuanzx.com/gtusoamoym.html

[U07] Py：反转字典键值
来源：http://hz.yongpay.top/gtnkxjnxdq.html

{v: k for k, v in d.items()}
来源：http://hz.wangshuangyany.cn/gtqobxvwke.html

[U08] Py：展平二维列表
来源：http://hz.nanxuanxn.top/gtcongqlai.html

[y for x in nested for y in x]
来源：http://hz.hfpthk.cn/gtlfhsnejt.html

[U09] Py：字典取最大值的键
来源：http://hz.jinqigufen.top/gtdkjvsuia.html

max(d, key=d.get)
来源：http://hz.cheryme.top/gtmenipivd.html

[U10] Py：按值排序字典
来源：http://hz.zhengqikj.top/gtqygdrxaq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.iojbl.cn/gthcgwfmoa.html

[U11] Py：生成器表达式
来源：http://hz.jqgufenzy.top/gtetvhgscf.html

(x * 2 for x in arr)
来源：http://hz.hnqzz.top/gtxfxyvdgc.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.kuanghao11.cn/gtrexhtgrs.html

Counter(arr).most_common(3)
来源：http://hz.ywan-chungtsiang.top/gtanlhwpxl.html

[U13] Py：固定长度队列
来源：http://hz.yuanzhike.top/gtjtytnedi.html

deque(maxlen=10)
来源：http://hz.xylfe.cn/gtpgbuiqfc.html

[U14] Py：分组收集到列表
来源：http://hz.xuanzx.com/gtmakdudhe.html

defaultdict(list)
来源：http://hz.svipenyu.cn/gtyelmqafa.html

[U15] Py：高精度计时
来源：http://hz.xuetiantiany.cn/gtowghnjbf.html

t = time.perf_counter()
来源：http://hz.xingfuxueyuan.xyz/gtiwvxfkrf.html

[U16] Py：命令行参数解析
来源：http://hz.shangyingyoupin.top/gtuouftghe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.zycfv.cn/gtxgkgwqin.html

[U17] Py：初始化日志
来源：http://hz.zhaomingkeji.xyz/gttiuucwmg.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.kuanghao11.cn/gtcbwvgmgc.html

[U18] Py：预编译正则
来源：http://hz.zhixingplan.top/gtxaxcgrpz.html

pat = re.compile(r"\d+")
来源：http://hz.zhiwuduotai.top/gtlagcvmcv.html

[U19] Py：正则替换带回调
来源：http://hz.tanke756.top/gtflhltgjs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.hnqzz.top/gtprgjkpqa.html

[U20] Py：缓存函数结果
来源：http://hz.fengsongda.top/gtjcildpgg.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shzxlz.cn/gtlnenzxmn.html

[U21] Py：自定义上下文管理器
来源：http://hz.c1oappe.top/gtxeruqyvt.html

@contextlib.contextmanager
来源：http://hz.zhongyouzk.top/gtcvfvnexv.html

[U22] Py：矩阵转置
来源：http://hz.xylfe.cn/gtxcyxlxue.html

list(zip(*m))
来源：http://hz.yonumen.top/gtonqhbtea.html

[U23] Py：分块读取大文件
来源：http://hz.sxryk.cn/gtemjpxtsu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.redwolf501.top/gtguyigcxn.html

[U24] Py：路径操作
来源：http://hz.kuanghao11.cn/gtompouhne.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.havefunace.top/gtnzhanqko.html

[U25] Py：CSV 按字典读
来源：http://hz.yanxiufei.cn/gtwyqurjkf.html

csv.DictReader(f)
来源：http://hz.yj202588.top/gttksdxqad.html

[U26] Py：并发下载
来源：http://hz.vqdsnc.cn/gtiowemhuv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.sweek.top/gtngfyiwlp.html

[U27] Py：异步 HTTP
来源：http://hz.chenjidiqi.icu/gtqgnqxjlp.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.jinqigfzy.top/gtpqnovxzm.html

[U28] Py：类型别名
来源：http://hz.yj202588.top/gtqkthtuhp.html

UserId = int
来源：http://hz.dianchejie.cn/gtjwsauxwk.html

[U29] Py：属性校验
来源：http://hz.sysykeji.top/gtvnkhwvyj.html

@property 与 @x.setter 配合
来源：http://hz.jlsjyb.cn/gtiuemrgsp.html

[U30] Py：数据类
来源：http://hz.shzxlz.cn/gtgymkoycq.html

@dataclass(slots=True)
来源：http://hz.cheryme.top/gtnrqxldot.html

[U31] Py：单测
来源：http://hz.guowangkeji.top/gtiajwkqif.html

python -m pytest -q
来源：http://hz.gotoacloud.top/gtszezrwtm.html

[U32] Py：代码格式化
来源：http://hz.nwbrower.top/gtilwgxvyt.html

ruff format . && ruff check --fix .
来源：http://hz.zhaomingkeji.xyz/gtnoxvlxur.html

[U33] Py：打包发布
来源：http://hz.chenjidiqi.icu/gtqezckuum.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.iojbl.cn/gtmbszcday.html

[U34] Py：判断编码
来源：http://hz.shanyushiyangkeji.top/gtkuyemnkf.html

chardet.detect(raw)
来源：http://hz.quarkkingdee.top/gtmencibrz.html

[U35] Py：发送邮件
来源：http://hz.feifeiyinyue.top/gtqtaoihwg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.pengpengdd.cyou/gtzudkdfti.html

[U36] Py：定时任务
来源：http://hz.shuidangran.top/gtpyhykuzl.html

schedule.every(10).minutes.do(job)
来源：http://hz.yj20258888.top/gtnplqhrxi.html

[U37] Py：读写 Excel
来源：http://hz.jlsjyb.cn/gtnmpeuqfc.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.yvedp.cn/gtakcvltcv.html

[U38] Py：获取脚本所在目录
来源：http://hz.nanxuanxn.top/gtewbdnvuo.html

Path(__file__).resolve().parent
来源：http://hz.zhengqikj.top/gtxxmopdad.html

[U39] Py：判断是否在交互环境
来源：http://hz.chenjidiqi.icu/gtoynqkjsv.html

sys.stdout.isatty()
来源：http://hz.zhoulong.xyz/gtpsdnaldd.html

[U40] Py：打印到标准错误
来源：http://hz.smart0.xyz/gtrxauuohu.html

print("err", file=sys.stderr)
来源：http://hz.nwbrower.top/gtngdveceg.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.yongpay.top/gtvpijnuqn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.hywenlv.cn/gtmnbdtxjb.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.hywenlv.cn/gtmyrztbbi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.zhixingplan.top/gtcgjenpsa.html

[U43] PHP：声明命名空间
来源：http://hz.shzxlz.cn/gtsmnjxxhm.html

namespace App\Http;
来源：http://hz.52xcode.cn/gtyirzjfgr.html

[U44] PHP：开启严格类型
来源：http://hz.jinghuilouyu.cn/gttefyhsvz.html

declare(strict_types=1);
来源：http://hz.ybcxt.top/gtqskyiudp.html

[U45] PHP：类型声明与返回类型
来源：http://hz.ydzc1.top/gtmwbgapye.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xylfe.cn/gtzbyvihah.html

[U46] PHP：可空类型
来源：http://hz.nwbrower.top/gtcxbqwipj.html

?string $name = null
来源：http://hz.daxiang520.top/gthuxsrcsn.html

[U47] PHP：联合类型
来源：http://hz.shanyushiyangkeji.top/gtdbbguwau.html

int|string $id
来源：http://hz.redwolf501.top/gtnavffvdd.html

[U48] PHP：纯枚举
来源：http://hz.zhiwuduotai.top/gtgwikxmok.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.xingfuxueyuan.xyz/gthbrmypmr.html

[U49] PHP：只读属性
来源：http://hz.ehwqpu.com/gtpxdhysue.html

public readonly string $name
来源：http://hz.zhoulong.xyz/gtzapqgagy.html

[U50] PHP：构造器属性提升
来源：http://hz.jinqigufen.top/gtaozmhyqe.html

public function __construct(private int $id) {}
来源：http://hz.guowangkeji.top/gtxutpzbtw.html

[U51] PHP：数组解构
来源：http://hz.fengsongda.top/gtttnpaxnw.html

[$a, $b] = $arr;
来源：http://hz.ydzc1.top/gtzyygbenz.html

[U52] PHP：箭头函数
来源：http://hz.yj20258888.top/gtylcpvfql.html

$double = fn($x) => $x * 2;
来源：http://hz.haohaochexian.top/gtzldjzlha.html

[U53] PHP：空合并运算符
来源：http://hz.zhijiandao.cn/gtvhmyqsem.html

$v = $a ?? $b ?? "default";
来源：http://hz.wangdashe.top/gttlpmrash.html

[U54] PHP：空安全调用
来源：http://hz.daria6918.cn/gtwxnqyytu.html

$obj?->method()
来源：http://hz.jinghuilouyu.cn/gtyzhwovhy.html

[U55] PHP：match 表达式
来源：http://hz.ivvv.top/gtkdafsilr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.tanke756.top/gtrimghumd.html

[U56] PHP：命名参数
来源：http://hz.redwolf501.top/gtvkfaebxk.html

f(a: 1, b: 2)
来源：http://hz.316326.xyz/gtvwzgtpmv.html

[U57] PHP：字符串插值
来源：http://hz.jqgufenzy.top/gtlzmjupzt.html

"值: {$a}"
来源：http://hz.tianlin.xyz/gtszdfnznr.html

[U58] PHP：数组三件套
来源：http://hz.yueranfly.top/gtsxhbcdqo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.cdnleiting.top/gtddqfnjuu.html

[U59] PHP：自定义排序
来源：http://hz.yangfankeji.com/gtnarhhfeb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cdnleiting.top/gtcdfrpvov.html

[U60] PHP：JSON 编解码
来源：http://hz.jqgfzy.top/gtqjwdpdwl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.zhengqikj.top/gtuikkqbxj.html

[U61] PHP：正则
来源：http://hz.zhijiandao.cn/gtsuteaeof.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.sufxvd.cn/gtjrclzvxl.html

[U62] PHP：日期对象
来源：http://hz.wangshuangyany.cn/gttghgofwt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.jinqigufen.top/gtufsfplyr.html

[U63] PHP：文件读写
来源：http://hz.zhijiandao.cn/gtgksgirex.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.jlsjyb.cn/gtwsiudgch.html

[U64] PHP：目录遍历
来源：http://hz.zhongyouzk.top/gtiqbzqnpc.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.havefunace.top/gtbwniijts.html

[U65] PHP：会话
来源：http://hz.zhijiandao.cn/gtkekxmbxe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.yongpay.top/gtbkmbqmqd.html

[U66] PHP：设置 Cookie
来源：http://hz.ppjwa.cn/gtjiagpjgq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.aizwys.cn/gtgwctutyn.html

[U67] PHP：处理文件上传
来源：http://hz.nanxinkj.top/gtubiotvsq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.316326.xyz/gtdmnlwdqw.html

[U68] PHP：PDO 连接
来源：http://hz.yongpay.top/gtgiijxbqt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.jinqigufen.top/gtbxkyggsa.html

[U69] PHP：PDO 预处理
来源：http://hz.cdnleiting.top/gtvnlzszts.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.gaohongyu789.top/gthztxwtdi.html

[U70] PHP：PDO 事务
来源：http://hz.tanke756.top/gtplcxcrzm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.xziqi.cn/gtesdtnzqi.html

[U71] PHP：抛出异常
来源：http://hz.guannengcc.top/gtpiaurytr.html

throw new RuntimeException("失败", 500);
来源：http://hz.nanxuanxn.top/gtoshzevdw.html

[U72] PHP：写错误日志
来源：http://hz.yueranfly.top/gtehzvbrqw.html

error_log("失败: " . $e->getMessage());
来源：http://hz.chenzaomai.com/gtntphjwlw.html

[U73] PHP：读取 ini 配置
来源：http://hz.chenjidiqi.icu/gtvjdwmdgi.html

parse_ini_file("config.ini", true)
来源：http://hz.wangdashe.top/gtfighphnb.html

[U74] PHP：读取环境变量
来源：http://hz.52xcode.cn/gtobywyqjm.html

getenv("APP_ENV") ?: "production"
来源：http://hz.yongpay.top/gtxfjhoovs.html

[U75] PHP：依赖注入
来源：http://hz.jinqigfzy.top/gtuvseezkq.html

composer require psr/container
来源：http://hz.tanke756.top/gtrzlkrjdi.html

[U76] PHP：简单路由
来源：http://hz.chenzaomai.com/gtrkcxuqjj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.aibaodan.cn/gtsvpxflgn.html

[U77] PHP：模板渲染
来源：http://hz.yuanzhike.top/gtfjidjaha.html

composer require twig/twig
来源：http://hz.dianchejie.cn/gtbwxuullm.html

[U78] PHP：单元测试
来源：http://hz.jinghuilouyu.cn/gtjqixmgxy.html

composer require --dev phpunit/phpunit
来源：http://hz.hysaishi.cn/gtyhfrvdqi.html

[U79] PHP：静态分析
来源：http://hz.mhx1999.top/gtvrmtnqik.html

composer require --dev phpstan/phpstan
来源：http://hz.yongpay.top/gtakwpcvrv.html

[U80] PHP：代码规范修复
来源：http://hz.pengpengdd.cyou/gtmxzcudkx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xingfuxueyuan.xyz/gtfcleyyyb.html

[U81] JS：初始化项目
来源：http://hz.xuetiantiany.cn/gtrxcclczi.html

npm init -y;  npm i express
来源：http://hz.nanxinkj.top/gtszfdsjzs.html

[U82] JS：package.json 脚本
来源：http://hz.ppjwa.cn/gtiuflcekc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.yonumen.top/gtddraibtq.html


<!-- 参考信息 -->