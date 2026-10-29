代发 wailian999

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gnfeebsvn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gtjavnyqz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gqxdackwn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gwxneqcxq.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gbqupcnmq.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gephbhftb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gqkhzpbeq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gnyaaevbo.sHtML

[T11] Kotlin：协程
来源：http://blog.fehbvm.com/Article/details/gevbgjvga.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gxcwqfqfz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gkzmilgej.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gsvzcpcnb.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gikvhpkly.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/ghpwlrvfo.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gmxfemugk.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gicsrqrva.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/ghyubcudb.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gpkidmgln.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gvuutbepo.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gvcohacka.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gwifsgfyh.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gnkgzcihz.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gguyivpcg.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/giagtkpxr.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gqktqmjfm.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gyevwselo.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gdzejpftb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gulhqblsz.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gvpparvtr.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/glpcujcwm.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gelexmbmw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gaxyldikm.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gszryfgsa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gsvvxqzko.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/gggipfjwa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbvnhygek.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gfpgskago.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gagykmldh.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gqjgiugrz.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gyowrlmbk.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/glblhtgyl.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/guyvwdetl.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gpneugsvk.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/grsqkwywa.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gfjfrldzw.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/geeboniqv.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gdjloczuq.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gxarjzntz.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/ghisesacb.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gonowybob.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gdmrdgvju.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gpkxjhtmz.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gxrgjmdec.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gcilsnoij.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gjydsfzxp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gohgmdsyx.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gomchmhpm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/govtatdkz.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gcrvaonge.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gvnxykdin.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gqkphqndb.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gegfgkwcq.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gvjygfdfp.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gdobbiopt.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gpfxkqimy.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gdynlfege.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/gywxdzjss.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gxnxmqsej.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gopqfjvoh.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gungqueic.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/ghnitcvjk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gnyyagvqr.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gerrgzhyj.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gieuevzjz.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gcyysvljs.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/geurbjftt.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gubdrabgq.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gmzrqksij.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gucfifsko.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gnatetvrk.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gifvbudha.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/grtbtelvf.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/ghxrupxln.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gpmxjjdmx.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/glktedltw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gylvbesxz.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gjlcncnps.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gcblwqrtt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gwxdmjpfo.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glwsgyoel.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gdbrbkuag.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gsuojgsyn.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/ggchpdvfg.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gteyvzssj.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gcwtpgdnu.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gkkepayle.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/ghftvpnpm.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gnumwdffu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gazxluhbs.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gajycgpba.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gpscywvyp.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gvipkvexa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/glxvarcao.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/geyrdowbs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gpdydckxa.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/ggvxdcxta.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gwkeaemnr.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gjvhzrain.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gnbedgnkj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gndwfdvcn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gwyaigyiy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjsairhee.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gibniifiz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gebyryiis.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/goiseaybr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqmunclwa.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/grufcovwc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gljjpxomi.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gxxbvdhea.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/grnjsmpnm.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gaztkilcx.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gtwcfhqee.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/grbvalhbh.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/ggykajdzf.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gzuokkomz.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gbdcfdwhm.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/gvlhdhnqk.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gljitsyyo.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gpddgtgcd.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gsiijasir.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gytekrdbp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/glhpdkqtw.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/ggtjipfyo.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/ghqspykut.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/goyvamfyf.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gurlogriu.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gzpcrzkai.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gvamaawdx.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/getpmwuaf.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gzdfmxixs.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gyepkylcb.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gxtzarigg.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gqxrphopu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/ggbutccos.sHtML

[U17] Py：初始化日志
来源：http://3g.hesvh.cn/Article/details/gdntweymc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gwnbkpbtg.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/guwaojngh.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/ghufgjxiu.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gnfnwaifx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gcqgatxnx.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gpjulyehu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gguddsjss.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gawlixfwr.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/grmmzutxs.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gqoushcei.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gevveszwu.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/goqfutgrl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gvaczwnwu.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvznwaxgs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/glncaasdv.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gqcmoczrg.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gvqwnjmqn.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gwdqhtzgi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gcnuthxkh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gjfeyjeps.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gpwwewqst.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gjtxbzqtm.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gzbvpbcuz.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/grfxwvdvs.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gdnfnonoh.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gaxagmmsw.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gnnhqwusc.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gvhymurna.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gvexepoap.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/ghvvhaylq.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gpzbmpqib.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gcujfrplu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gvpgkjbvc.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gnjjfwhdg.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gykfamkmm.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/grgowxdmq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/ggpjtopbn.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gpzhunbcx.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gmdzsmnah.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gvcvmldce.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gjibzmrih.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/grvaseebn.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/giaeoaooe.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gihypukeu.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gwomxnnny.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gygrstvmx.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gkafyoyee.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gpjimefdi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gxnxaxitd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/gohxwkkki.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gdfbczhnj.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/ggvqstbhk.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gqohrfrdc.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gmmrazral.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gayzljnek.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/ghzmadjpk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/glbjvtqxb.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gcbrfqnox.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gochnolme.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gesjmusbo.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/gnbvgmdon.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gmrocdmir.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gypqsyegi.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gwcetbamv.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gwdgtpana.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gpzvdzrmi.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gieqkunfj.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gvtxbafvq.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/goqyouayj.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gpmzlryfw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gvwetsoiu.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/ganpqpvqo.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gubxhsnah.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gebomqepw.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gxjdkvcin.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gmpqeogdk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gzgpokkmp.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gcxejqbrw.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gqcnmhfqa.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gshblvyzp.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gzkzvogyy.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gflbppcpa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gsqufqrkw.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gejxwcwjt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gufkwxvgz.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gldexwsyz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gbckbiwac.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gahhrblro.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gnpldqkkt.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/ggrehgnbk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gqjlxcpqa.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gueapnmfa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gidkqiqcg.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gohagxmqs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/glhmufrqg.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gjfxkxlft.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gveqapmod.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.zdbjq.cn/Article/details/gzaogxrdm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/guemzapam.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gjcsmafku.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gznopiing.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gozxtkglj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gtijwpivy.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gydszpkbi.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gwslgqfex.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gdgarqbur.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gotcmnckn.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gkzerlakn.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gpnzoofrd.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gmvowilbp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gxrxbzfov.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/guqsgtijh.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gbkfvvbka.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/glzvzztqn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gktgndunb.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gzyphbnoz.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gtrgyledy.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gtzwxhojf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gzqwqlpge.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gthnjfibh.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gxnarhldt.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gyttmwljo.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gxujefgmm.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gsmvvazdz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gfljpsqyi.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.hesvh.cn/Article/details/grahmniva.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gjwafnsxk.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gbftxiicb.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gusoegmcp.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gjlwjlcvp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/giojcpgsd.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gtdzcttnz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gtbkgjedw.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/galcudvyy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gnsfegbfs.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gqrqbofgp.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gyonwesdt.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/ghlawuheu.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gdxmpdsub.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/ghsbgxyvt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gzlehkeay.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gzvsfaebm.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gwblyjmbq.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gcybqwpfi.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/ghizxepcf.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gdxkmoztg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gyxglbxam.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gnobkfpev.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/grovlzefh.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gnqidbnkl.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkkxbmymk.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/guyngqmnt.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gcbuunsgs.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gnypsmprn.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gubrxppxi.sHtML


<!-- 参考信息 -->