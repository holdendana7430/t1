代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ybcxt.top/gtbrhdryhp.html

[S55] C++：结构化绑定
来源：http://hz.yueranfly.top/gtuioevdbt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.havefunace.top/gtzomjkaje.html

[S56] C++：optional
来源：http://hz.smart0.xyz/gttieqqqus.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtuhvtnoaa.html

[S57] C++：编译期常量
来源：http://hz.jinqigfzy.top/gtioyfxymz.html

constexpr int N = 10;
来源：http://hz.nwbrower.top/gtqeguwerw.html

[S58] C++：命名空间
来源：http://hz.nanxuanxn.top/gttyrpotsv.html

namespace ns { int f() { return 1; } }
来源：http://hz.gotoacloud.top/gtnbopogjq.html

[S59] C++：静态断言
来源：http://hz.yangfankeji.com/gtmzukbflx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tanke756.top/gtfzrwikgv.html

[S60] C++：遍历并删除元素
来源：http://hz.316326.xyz/gtzohybqew.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.svipenyu.cn/gtujhjvtfb.html

================================================================================
来源：http://hz.snrcjt.cn/gttsaajjbn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yueranfly.top/gtqqmwytwj.html

================================================================================
来源：http://hz.hammf.cn/gtnrrxklbh.html

[T01] Kotlin：Hello World
来源：http://hz.quarkkingdee.top/gtakfshwip.html

println("Hello")
来源：http://hz.hywenlv.cn/gtnxcqomxq.html

[T02] Kotlin：变量
来源：http://hz.hammf.cn/gtamuquskw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sweek.top/gtcvwcvpwc.html

[T03] Kotlin：字符串模板
来源：http://hz.dashuyun.cn/gthqlwyptf.html

"值: $b"
来源：http://hz.zdqjudy.top/gtwinluksm.html

[T04] Kotlin：空安全
来源：http://hz.birdmap.top/gtgnjvywrb.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gtviefnccd.html

[T05] Kotlin：when 表达式
来源：http://hz.cheryme.top/gtoztpszsv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.guowangkeji.top/gtcsrxhgvo.html

[T06] Kotlin：集合映射
来源：http://hz.hfpthk.cn/gteqvyytjb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yonumen.top/gtvircoris.html

[T07] Kotlin：集合过滤
来源：http://hz.chenjidiqi.icu/gtswjyozam.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xuanzx.com/gtqfnbpbou.html

[T08] Kotlin：数据类
来源：http://hz.dianchejie.cn/gtpjzlotfk.html

data class User(val name: String, val age: Int)
来源：http://hz.yangfankeji.com/gtjzybrsgv.html

[T09] Kotlin：扩展函数
来源：http://hz.hywenlv.cn/gtpccspspj.html

fun String.exclaim() = this + "!"
来源：http://hz.xziqi.cn/gtvwzyiuzg.html

[T10] Kotlin：默认参数
来源：http://hz.xylfe.cn/gtkkrlhylu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.smart0.xyz/gtpmvgsfgj.html

[T11] Kotlin：协程
来源：http://hz.birdmap.top/gtnjnwqfum.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.havefunace.top/gtjrxvtegj.html

[T12] Kotlin：解构声明
来源：http://hz.aizwys.cn/gtijzmumrz.html

val (a, b) = Pair(1, 2)
来源：http://hz.shangyingyoupin.top/gtbpgyxvuo.html

[T13] Kotlin：只读 Map
来源：http://hz.jqgfzy.top/gtpquokegl.html

val m = mapOf("a" to 1)
来源：http://hz.smart0.xyz/gtoomuzqur.html

[T14] Kotlin：循环
来源：http://hz.jinyuanbaomall.cn/gtatmmpjon.html

for (i in 1..10) println(i)
来源：http://hz.cdnleiting.top/gtqznosqws.html

[T15] Kotlin：接口
来源：http://hz.cqqwz.cn/gtpcpopxfm.html

interface Shape { fun area(): Double }
来源：http://hz.ehwqpu.com/gtmxhuesvv.html

[T16] Swift：Hello World
来源：http://hz.meibo888.top/gtemtiwnoo.html

print("Hello")
来源：http://hz.gogol.net.cn/gtqskvlofw.html

[T17] Swift：变量与常量
来源：http://hz.fengsongda.top/gtujmwubok.html

var a = 1;  let b = 2
来源：http://hz.chenlongwang.top/gtkpoexpwx.html

[T18] Swift：字符串插值
来源：http://hz.jinqigufen.top/gtzdcgptga.html

"值: \(b)"
来源：http://hz.hammf.cn/gtgrlemryl.html

[T19] Swift：可选绑定
来源：http://hz.yangfankeji.com/gtulrgxbsa.html

if let n = opt { print(n) }
来源：http://hz.chenzaomai.com/gtzkeiloet.html

[T20] Swift：数组操作
来源：http://hz.316326.xyz/gtimoyuksb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.andypj.xyz/gtdqwzsmza.html

[T21] Swift：遍历
来源：http://hz.guannengcc.top/gtkgvufdcb.html

for x in a { print(x) }
来源：http://hz.fengsongda.top/gtcqidqrsa.html

[T22] Swift：字典
来源：http://hz.zhiwuduotai.top/gtiqzuxsap.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.wangdashe.top/gtckcczvhp.html

[T23] Swift：函数
来源：http://hz.jqgfzy.top/gttcwezmwh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shanyushiyangkeji.top/gtuuwwafvk.html

[T24] Swift：闭包
来源：http://hz.mhx1999.top/gtewwhbyft.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.hfpthk.cn/gtltjrajla.html

[T25] Swift：结构体
来源：http://hz.jyoumei.cn/gtqptsolks.html

struct P { var x: Int }
来源：http://hz.xuetiantiany.cn/gtnzjmbqol.html

[T26] Swift：类与重写
来源：http://hz.chenjidiqi.icu/gtemzvtpxp.html

class A: Base { override func f() {} }
来源：http://hz.yongpay.top/gtrirtkpvt.html

[T27] Swift：错误处理
来源：http://hz.xuetiantiany.cn/gttripwzjd.html

do { try f() } catch { print(error) }
来源：http://hz.tianlin.xyz/gtojcratol.html

[T28] Swift：枚举
来源：http://hz.ehwqpu.com/gtouuwawln.html

enum Color { case red, green }
来源：http://hz.chenzaomai.com/gtrdxopggj.html

[T29] Swift：guard 提前返回
来源：http://hz.chenjidiqi.icu/gtbpqwsoue.html

guard let x = opt else { return }
来源：http://hz.yj202588.top/gtqxdlzvjm.html

[T30] Swift：协议
来源：http://hz.daxiang520.top/gtgosllkbi.html

protocol Shape { func area() -> Double }
来源：http://hz.yongpay.top/gtvzqnondh.html

[T31] Lua：Hello World
来源：http://hz.jinqigufen.top/gtdiibgncx.html

print("Hello")
来源：http://hz.cdnleiting.top/gtyrdmugus.html

[T32] Lua：局部变量
来源：http://hz.daria6918.cn/gtdhprnzfr.html

local a = 1
来源：http://hz.aizwys.cn/gtcrrvdeta.html

[T33] Lua：表（数组）
来源：http://hz.zhengqikj.top/gtjmgnrqpw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.meibo888.top/gtmexbvxvv.html

[T34] Lua：遍历表
来源：http://hz.zhoulong.xyz/gtallufopa.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ydzc1.top/gthcrppkzj.html

[T35] Lua：字典表
来源：http://hz.chenjidiqi.icu/gtwgcyvmxq.html

local d = { a = 1 };  d.b = 2
来源：http://hz.guannengcc.top/gtbmkmsoxh.html

[T36] Lua：函数
来源：http://hz.tanke756.top/gtttqeinds.html

function add(a, b) return a + b end
来源：http://hz.wangshuangyany.cn/gtkxuguhrx.html

[T37] Lua：字符串拼接
来源：http://hz.jinghuilouyu.cn/gtlcygwawl.html

"a" .. "b"
来源：http://hz.nanxuanxn.top/gtnepdcdzn.html

[T38] Lua：条件
来源：http://hz.jinqigfzy.top/gtybgcnnpv.html

if x > 0 then print("正") end
来源：http://hz.tanke756.top/gtruwivkfn.html

[T39] Lua：模式匹配
来源：http://hz.zdqjudy.top/gthhwwwfrr.html

string.find(s, "%d+")
来源：http://hz.smart0.xyz/gtqjhphljs.html

[T40] Lua：元表
来源：http://hz.cdnleiting.top/gtannflxmp.html

setmetatable({}, { __index = base })
来源：http://hz.zhoulong.xyz/gtgqctkjvh.html

[T41] Perl：Hello World
来源：http://hz.andypj.xyz/gtdlshjwyr.html

print "Hello\n";
来源：http://hz.jlsjyb.cn/gtrowmxecy.html

[T42] Perl：变量类型
来源：http://hz.hfpthk.cn/gtavbvxnmh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cucudq.cn/gtgacglqum.html

[T43] Perl：字符串插值
来源：http://hz.sweek.top/gtggylqcxw.html

"值: $a"
来源：http://hz.feifeiyinyue.top/gtqgfgfkkm.html

[T44] Perl：条件
来源：http://hz.cucudq.cn/gtantykgmi.html

if ($a > 0) { print "正"; }
来源：http://hz.xuanzx.com/gtlcezvsfd.html

[T45] Perl：数组遍历
来源：http://hz.fengsongda.top/gtjornzgqi.html

for my $x (@arr) { print $x; }
来源：http://hz.yuanzhike.top/gthzniujbc.html

[T46] Perl：哈希操作
来源：http://hz.daria6918.cn/gtvrftlfgg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.ydjk.org.cn/gtnajjpxlk.html

[T47] Perl：正则捕获
来源：http://hz.xylfe.cn/gtussnitmy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hongshengwenyu.top/gtouadjnyh.html

[T48] Perl：正则替换
来源：http://hz.zycfv.cn/gttmojcsxy.html

$s =~ s/old/new/g;
来源：http://hz.tianlin.xyz/gtmacwcnqo.html

[T49] Perl：函数
来源：http://hz.jyoumei.cn/gtmjojxrtd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ydzc1.top/gtodpaceym.html

[T50] Perl：逐行读文件
来源：http://hz.smart0.xyz/gtyscyvubj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.ywan-chungtsiang.top/gtdikpikoy.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zhongyouzk.top/gtdcvwmdts.html

[T51] Scala：Hello World
来源：http://hz.chenjidiqi.icu/gttzayzwhk.html

println("Hello")
来源：http://hz.yangfankeji.com/gtxuknhbiy.html

[T52] Scala：变量
来源：http://hz.tianlin.xyz/gtkyzlxzch.html

val a = 1;  var b = 2
来源：http://hz.hywenlv.cn/gthxngkzrk.html

[T53] Scala：字符串插值
来源：http://hz.guowangkeji.top/gtyxlslxxj.html

s"值: $b"
来源：http://hz.gogol.net.cn/gtygzabgop.html

[T54] Scala：集合映射
来源：http://hz.bjfxy.top/gtqrfjbwzc.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yvedp.cn/gtmecubiyh.html

[T55] Scala：集合过滤
来源：http://hz.gzhubu.top/gtadyykjyw.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shanyushiyangkeji.top/gtfzzmsour.html

[T56] Scala：样例类
来源：http://hz.andypj.xyz/gtinnccqvp.html

case class User(name: String, age: Int)
来源：http://hz.nanxinkj.top/gtuztodzig.html

[T57] Scala：模式匹配
来源：http://hz.gzhubu.top/gtxjqtjerc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.mhx1999.top/gtmalupozm.html

[T58] Scala：函数定义
来源：http://hz.jlsjyb.cn/gtcxqjmezy.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.ivvv.top/gtxftpoafx.html

[T59] Scala：循环
来源：http://hz.shanyushiyangkeji.top/gtvldwwuup.html

for (i <- 1 to 10) println(i)
来源：http://hz.guowangkeji.top/gtrgwmmbkr.html

[T60] Scala：折叠
来源：http://hz.chenzaomai.com/gtevgqazvw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.havefunace.top/gtgspkkzaf.html

================================================================================
来源：http://hz.yueranfly.top/gtrugwdfur.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.havefunace.top/gtlexpubfx.html

================================================================================
来源：http://hz.birdmap.top/gtoqlheajg.html

[U01] Py：创建虚拟环境
来源：http://hz.yueranfly.top/gtvoeqkpiw.html

python -m venv .venv && source .venv/bin/activate
来源：http://hz.daria6918.cn/gtlputedib.html

[U02] Py：导出 / 安装依赖
来源：http://hz.xinyue.icu/gtbmhvauwf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hz.xingfuxueyuan.xyz/gtejlkapxt.html

[U03] Py：加载 .env 配置
来源：http://hz.jinyuanbaomall.cn/gtmoilqstj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://hz.hnxiangtu.top/gtckezrhrl.html

[U04] Py：变量调试打印
来源：http://hz.nwbrower.top/gtyxcttqcj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hz.9152youxi.cn/gtohdzpjhe.html

[U05] Py：列表去重且保序
来源：http://hz.ppjwa.cn/gtiyqjfxmv.html

list(dict.fromkeys(arr))
来源：http://hz.hfpthk.cn/gtlctqqnbt.html

[U06] Py：合并两个字典
来源：http://hz.smart0.xyz/gtosbxbxni.html

{**a, **b}
来源：http://hz.gogol.net.cn/gtknpjocvb.html

[U07] Py：反转字典键值
来源：http://hz.vqdsnc.cn/gtssjfkqtl.html

{v: k for k, v in d.items()}
来源：http://hz.gotoacloud.top/gtcyegqvrp.html

[U08] Py：展平二维列表
来源：http://hz.hysaishi.cn/gtzfhqkvyu.html

[y for x in nested for y in x]
来源：http://hz.shanyushiyangtech.top/gtimvoetes.html

[U09] Py：字典取最大值的键
来源：http://hz.yj20258888.top/gtquuydxgf.html

max(d, key=d.get)
来源：http://hz.hfpthk.cn/gtxmcnxikk.html

[U10] Py：按值排序字典
来源：http://hz.hfpthk.cn/gtgeewrfws.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hz.yvedp.cn/gtziqlxbpy.html

[U11] Py：生成器表达式
来源：http://hz.guowangkeji.top/gtiqbdnvay.html

(x * 2 for x in arr)
来源：http://hz.jinghuilouyu.cn/gtuojplvkb.html

[U12] Py：取出现最多的 3 个元素
来源：http://hz.smart0.xyz/gtejjgufpk.html

Counter(arr).most_common(3)
来源：http://hz.sweek.top/gtrhsajxdw.html

[U13] Py：固定长度队列
来源：http://hz.ehwqpu.com/gtwlurrjqy.html

deque(maxlen=10)
来源：http://hz.shzxlz.cn/gtzrcoupus.html

[U14] Py：分组收集到列表
来源：http://hz.zhoulong.xyz/gtwxbjiqeh.html

defaultdict(list)
来源：http://hz.sysykeji.top/gtdpxogope.html

[U15] Py：高精度计时
来源：http://hz.52xcode.cn/gtdwnbpynb.html

t = time.perf_counter()
来源：http://hz.gaohongyu789.top/gtrzqtupmt.html

[U16] Py：命令行参数解析
来源：http://hz.guowangkeji.top/gtxmnqtrbi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hz.hywenlv.cn/gtiswplmux.html

[U17] Py：初始化日志
来源：http://hz.jinghuilouyu.cn/gtvqijmypk.html

logging.basicConfig(level=logging.INFO)
来源：http://hz.fengsongda.top/gtzswyqxxo.html

[U18] Py：预编译正则
来源：http://hz.dianchejie.cn/gtljfzjhmf.html

pat = re.compile(r"\d+")
来源：http://hz.hfpthk.cn/gtdempiamp.html

[U19] Py：正则替换带回调
来源：http://hz.hnxiangtu.top/gtfgzuxamt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hz.yonumen.top/gtsldsuopi.html

[U20] Py：缓存函数结果
来源：http://hz.gotoacloud.top/gtbhfxnhjp.html

@functools.lru_cache(maxsize=None)
来源：http://hz.shanyushiyangtech.top/gtoopxiocy.html

[U21] Py：自定义上下文管理器
来源：http://hz.daria6918.cn/gtgxbfxdwc.html

@contextlib.contextmanager
来源：http://hz.pycfn.com/gtrvajodjw.html

[U22] Py：矩阵转置
来源：http://hz.dianchejie.cn/gtskwfrzks.html

list(zip(*m))
来源：http://hz.cqqwz.cn/gtzvprqzvb.html

[U23] Py：分块读取大文件
来源：http://hz.shangyingyoupin.top/gtdmsibtah.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hz.shanyushiyangtech.top/gtsvygjpxr.html

[U24] Py：路径操作
来源：http://hz.gzhubu.top/gtishflhtr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hz.sufxvd.cn/gtljeobgge.html

[U25] Py：CSV 按字典读
来源：http://hz.xingfuxueyuan.xyz/gtjmkqkivr.html

csv.DictReader(f)
来源：http://hz.gogol.net.cn/gtweueoxqg.html

[U26] Py：并发下载
来源：http://hz.nanxuanxn.top/gtegodssnm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hz.gogol.net.cn/gtjmuvdjrg.html

[U27] Py：异步 HTTP
来源：http://hz.cqqwz.cn/gtywzyoknr.html

aiohttp.ClientSession() 配合 async with
来源：http://hz.hnxiangtu.top/gtjqxyxnwy.html

[U28] Py：类型别名
来源：http://hz.yanxiufei.cn/gtfjqxgran.html

UserId = int
来源：http://hz.316326.xyz/gtxgdozwpr.html

[U29] Py：属性校验
来源：http://hz.guannengcc.top/gtghreujhl.html

@property 与 @x.setter 配合
来源：http://hz.aibaodan.cn/gtbesbmphn.html

[U30] Py：数据类
来源：http://hz.jqgufenzy.top/gtbxrieqfm.html

@dataclass(slots=True)
来源：http://hz.yueranfly.top/gtxgasxirl.html

[U31] Py：单测
来源：http://hz.yuxming.cn/gtknazduva.html

python -m pytest -q
来源：http://hz.c1oappe.top/gtqpdaqyad.html

[U32] Py：代码格式化
来源：http://hz.hnxiangtu.top/gtuowlouls.html

ruff format . && ruff check --fix .
来源：http://hz.dianchejie.cn/gtpjcbyvmg.html

[U33] Py：打包发布
来源：http://hz.hammf.cn/gtxyxawaye.html

python -m build  （依赖 pyproject.toml）
来源：http://hz.snrcjt.cn/gtiovfhymo.html

[U34] Py：判断编码
来源：http://hz.jinghuilouyu.cn/gtidlwgcpq.html

chardet.detect(raw)
来源：http://hz.nwbrower.top/gtzctscsit.html

[U35] Py：发送邮件
来源：http://hz.xuanzx.com/gtxkbhheyb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hz.gaohongyu789.top/gtcgtoelyc.html

[U36] Py：定时任务
来源：http://hz.hnxiangtu.top/gtllysjdtj.html

schedule.every(10).minutes.do(job)
来源：http://hz.zhixingplan.top/gthkgtqxed.html

[U37] Py：读写 Excel
来源：http://hz.jinyuanbaomall.cn/gtzkldwdnl.html

pandas.read_excel / DataFrame.to_excel
来源：http://hz.birdmap.top/gtrdgpebem.html

[U38] Py：获取脚本所在目录
来源：http://hz.xziqi.cn/gtflxgecwq.html

Path(__file__).resolve().parent
来源：http://hz.hammf.cn/gtpwxqwhrg.html

[U39] Py：判断是否在交互环境
来源：http://hz.yuanzhike.top/gtkhprtvtd.html

sys.stdout.isatty()
来源：http://hz.gotoacloud.top/gtmbeanrhf.html

[U40] Py：打印到标准错误
来源：http://hz.shanyushiyangtech.top/gtyavafpzp.html

print("err", file=sys.stderr)
来源：http://hz.jiagoushi.top/gtkvofligs.html

[U41] PHP：初始化 Composer 项目
来源：http://hz.tian-w.cn/gtnmfvrbkb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://hz.fengsongda.top/gtyabkznbw.html

[U42] PHP：PSR-4 自动加载
来源：http://hz.chenzaomai.com/gtnmzabqck.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hz.yueranfly.top/gtisyoqvun.html

[U43] PHP：声明命名空间
来源：http://hz.birdmap.top/gtzzgsuffr.html

namespace App\Http;
来源：http://hz.hysaishi.cn/gtjfwexnou.html

[U44] PHP：开启严格类型
来源：http://hz.shanyushiyangkeji.top/gtjajwbxqp.html

declare(strict_types=1);
来源：http://hz.dianchejie.cn/gtqegoxitw.html

[U45] PHP：类型声明与返回类型
来源：http://hz.redwolf501.top/gttpsdetmm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtblsytmjb.html

[U46] PHP：可空类型
来源：http://hz.yueranfly.top/gtlgqoiwuq.html

?string $name = null
来源：http://hz.ydjk.org.cn/gtgsbxzolq.html

[U47] PHP：联合类型
来源：http://hz.316326.xyz/gtlzwdcgca.html

int|string $id
来源：http://hz.zhaomingkeji.xyz/gtcknilqlm.html

[U48] PHP：纯枚举
来源：http://hz.9152youxi.cn/gtknxvcbrw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hz.cashguo.top/gtxcrzgriq.html

[U49] PHP：只读属性
来源：http://hz.yj20258888.top/gtvsxmpwyd.html

public readonly string $name
来源：http://hz.quarkkingdee.top/gtkuncwlog.html

[U50] PHP：构造器属性提升
来源：http://hz.shanyushiyangkeji.top/gtmezjowjq.html

public function __construct(private int $id) {}
来源：http://hz.wangdashe.top/gtnfmwmbzu.html

[U51] PHP：数组解构
来源：http://hz.feifeiyinyue.top/gtqrtyiohv.html

[$a, $b] = $arr;
来源：http://hz.zhijiandao.cn/gttubhuwpk.html

[U52] PHP：箭头函数
来源：http://hz.zhiwuduotai.top/gtbogstsws.html

$double = fn($x) => $x * 2;
来源：http://hz.nanxinkj.top/gtknuxdibu.html

[U53] PHP：空合并运算符
来源：http://hz.sufxvd.cn/gtwgwjpjco.html

$v = $a ?? $b ?? "default";
来源：http://hz.fzhhl.top/gttyxjvglz.html

[U54] PHP：空安全调用
来源：http://hz.ppjwa.cn/gtyztkbwbf.html

$obj?->method()
来源：http://hz.daria6918.cn/gtnhadfdsi.html

[U55] PHP：match 表达式
来源：http://hz.tianlin.xyz/gtwsvzcksj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hz.316326.xyz/gtdweazvbx.html

[U56] PHP：命名参数
来源：http://hz.andypj.xyz/gthzeeygyi.html

f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gtqmundeqr.html

[U57] PHP：字符串插值
来源：http://hz.yonumen.top/gtlnbonozo.html

"值: {$a}"
来源：http://hz.yonumen.top/gtpqrigigq.html

[U58] PHP：数组三件套
来源：http://hz.xingfuxueyuan.xyz/gtapavltag.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hz.yangfankeji.com/gtbzahmhiw.html

[U59] PHP：自定义排序
来源：http://hz.svipenyu.cn/gtpcacidos.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.c1oappe.top/gtfsgjdkwh.html

[U60] PHP：JSON 编解码
来源：http://hz.ywan-chungtsiang.top/gtjdrmcnyx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hz.quarkkingdee.top/gtzgjrvxib.html

[U61] PHP：正则
来源：http://hz.ydzc1.top/gtppqmkutd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.ybcxt.top/gtufyjfgds.html

[U62] PHP：日期对象
来源：http://hz.xziqi.cn/gtivsbhmmn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hz.yuanzhike.top/gtppbzikvx.html

[U63] PHP：文件读写
来源：http://hz.havefunace.top/gtusjseyam.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hz.316326.xyz/gtafirrxuh.html

[U64] PHP：目录遍历
来源：http://hz.quarkkingdee.top/gtnrrqeliq.html

glob("dir/*.php");  scandir("dir");
来源：http://hz.redwolf501.top/gtgpyuqugm.html

[U65] PHP：会话
来源：http://hz.birdmap.top/gtypgokviz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtlbpycgrn.html

[U66] PHP：设置 Cookie
来源：http://hz.cucudq.cn/gtmvqpbpon.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hz.zhoulong.xyz/gtjlniwchs.html

[U67] PHP：处理文件上传
来源：http://hz.gotoacloud.top/gtibkxzlta.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hz.zhixingplan.top/gtcziogtob.html

[U68] PHP：PDO 连接
来源：http://hz.shangyingyoupin.top/gtdpbscqhi.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.aizwys.cn/gtcwyinfpe.html

[U69] PHP：PDO 预处理
来源：http://hz.hammf.cn/gtfimefidm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hz.jlsjyb.cn/gtyqumpzae.html

[U70] PHP：PDO 事务
来源：http://hz.aizwys.cn/gtdzrtacur.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hz.ivvv.top/gtxlbqgdzw.html

[U71] PHP：抛出异常
来源：http://hz.shzxlz.cn/gtwekykwqu.html

throw new RuntimeException("失败", 500);
来源：http://hz.zycfv.cn/gtvvwxpyaz.html

[U72] PHP：写错误日志
来源：http://hz.ydzc1.top/gtuygcyltc.html

error_log("失败: " . $e->getMessage());
来源：http://hz.ydzc1.top/gtovezkexr.html

[U73] PHP：读取 ini 配置
来源：http://hz.yuxming.cn/gtnwgqeyiu.html

parse_ini_file("config.ini", true)
来源：http://hz.wangshuangyany.cn/gtnohdhkuj.html

[U74] PHP：读取环境变量
来源：http://hz.birdmap.top/gtzcxrlfej.html

getenv("APP_ENV") ?: "production"
来源：http://hz.jyoumei.cn/gtclvqddbw.html

[U75] PHP：依赖注入
来源：http://hz.chenjidiqi.icu/gtbqzewrta.html

composer require psr/container
来源：http://hz.yanxiufei.cn/gtyolcelej.html

[U76] PHP：简单路由
来源：http://hz.redwolf501.top/gtuqxarfzy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.xylfe.cn/gtlpqvkowo.html

[U77] PHP：模板渲染
来源：http://hz.yongpay.top/gtbcpujyiv.html

composer require twig/twig
来源：http://hz.fzhhl.top/gtghcydrmo.html

[U78] PHP：单元测试
来源：http://hz.xylfe.cn/gtiirbdemg.html

composer require --dev phpunit/phpunit
来源：http://hz.fengsongda.top/gtljuktqcr.html

[U79] PHP：静态分析
来源：http://hz.gaohongyu789.top/gtxqdncnep.html

composer require --dev phpstan/phpstan
来源：http://hz.tian-w.cn/gtbbqsuuon.html

[U80] PHP：代码规范修复
来源：http://hz.zycfv.cn/gttqzajxst.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.hywenlv.cn/gtsxhknjja.html


<!-- 参考信息 -->