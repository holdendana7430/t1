代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2souqfpaw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gvydqsff.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2acbrsfqw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kdcrjtke.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ebdcmmoj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2reodaczs.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2toomxvcv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wpjgabol.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2grgrwmob.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dqdnmdry.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2cleljqrv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xdiipddf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tbnikzxi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2rypeeaom.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2peghltvd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2mznlgdhg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2elqvugip.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2giwxmuex.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vboznlwn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xjwdwtax.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hdyptppf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nvlwrfds.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2weabolal.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2djlsyfrc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gakcrxty.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hxcwwneu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vgrkeebr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2swbhfsad.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fkggbtyp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ewozxnrn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qqebvmjp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cskrcbtj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2ytebzcdh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2nftwlmqh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2bcabguur.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xprovpyo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wzbqgmiz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2csusukvy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2gkzlggwi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ddpbomfp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2swzuvvig.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2baqpgsqb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zktwobca.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2shwjyrlx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2thmmqqgw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vfqgmvys.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ghinaxts.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fcgcnyau.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mfhhhief.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kmnyzjjf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jbiyqawo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ybwzqlij.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gkhofism.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ezutpnnj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2dbpmazox.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2osahmycy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ypkukgau.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ypwcdryz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fbcmpzdp.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ygxvxucl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2knnxdpnc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wxsljzxh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2wwjaqvyd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2lwsiquci.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2axkyeyww.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2llqgfbih.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2wlqocwua.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2irpamnhc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qkjftjmm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jmjkpncp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mavsmfxn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2fbmlqput.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2zttywvzm.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ccqxbjov.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2anoieleb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2icuzhogr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iywwjgix.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2wsdbkcuu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2nrtjlijy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hmamrjdd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2phbyxwkt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2oyimphqf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2idfupqcd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2nxqcmcxz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vvvzeksz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tqijfdwr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mrvvsmiu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybtpeqck.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2sqvdphfj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2grnuhssq.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2lchwtmxn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2wrfartae.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkovwnlh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zgwudlpn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dlbrktdz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2onkjmebo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbrtaauf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2slzxngef.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fdypmbsb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2doexoqje.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2byezcglm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2owrneffm.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2paahycra.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hceowvhb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rbfmkrlx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aslmmgss.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gdngnhes.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2bgeqrbzh.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2myytqkcg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lwxhavus.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dtjkjsqm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2pgdwvxvb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2nlpgzgii.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nqumkbpb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jcokpnok.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2vegjjqzu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2niiebdms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfnvibsq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qmvwgine.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oolmuovw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ctrxftfn.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2pucxrcyd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2trbkqzlv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2wcnrwqca.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2eslxxrhz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2uizdiljo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2zwsoelzm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2nmdklogw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2hdqegnsy.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hgweqhgk.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2esnycrds.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zhhiykdx.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hzihxuua.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2eitxcvpr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2lxjfyuxs.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2nxxofjrg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2ckefvuam.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2mgkyadbe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vjopjqsn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2jrfjvbdx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wipmidto.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vkufqymz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zpsbambl.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dvvojlfz.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fuatqjoe.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2zboycezn.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wdvkqhyk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbllgor.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2rxtzxkxu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2kdnsxlaq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2dqidyzca.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2aqzzgwrl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2zyutkkky.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2mcdajgud.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2bjfwqjau.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tekvuekr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cfvktuct.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2pblzfrto.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ooegrgbs.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2zzemqwsp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2ecvbegqr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ciemnzms.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ddxweowl.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2stypagjf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2laydlvhl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2heescfrc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2refpyttw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ckgzosvo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2cgudxyan.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2obvmodmv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2gajcgzvj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ustlxyer.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2mygnpypz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2apuuiogf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2fhlieuqb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2gabefhhw.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2vuuzuqco.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2kmvixyfe.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jctpmxan.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2byyaajju.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2wehvlimt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2myfaejrq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ptwuhsop.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dxfsotsx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dnsyprrl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2cuxzmbcu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2bvbufjps.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2ezntcoax.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2fmtdxbba.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2gbtzfdxs.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yfwbfbqb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rptwpcmc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2urgkpayf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2bklrgfur.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2eykoagyt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2xyavczys.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2gwyiqgxj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2otvjusfj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2wxnbulei.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tmtuipgp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2dmswrbbz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hpewtudl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2jaweunym.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qiejcbch.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nmmnrvuj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2nrucvwej.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2axklmaho.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wngtzebn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fxccwxsf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hrpnqaay.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2loexyehj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2jjqjlmja.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2axglcslq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2qfodheqp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vcrdeswt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2phndwbpy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2szcdxlne.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2cngfnoyr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yrqskhmi.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2kppwxukc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2xspqtutr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2tsjxgfhc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2irbcbdkv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rsrrocbw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2cnvuclhu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lmghbzej.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2yintumdo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2pymblint.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2tpapnbgu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zlnmpgrp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ycjnqrnj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lgsbnvqv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hlpotqvp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2ijtmhfmf.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2jxgbwcap.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xhggbmtk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ylykqias.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xgriibwx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2kuqtoksn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iwlrfdcl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2hsqgrgsr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mgwhluqg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2naupxgxy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ojpkjifz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ugfjswer.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2darknhgj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2yzsrbdtc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2cqfmuerm.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qgsvrwtn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qzwxstub.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2mdsmqbyj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ajrsczdv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2uokazqzc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2xvwspyzc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2osttjcud.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2aggbcpor.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ddnkrrtf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2hhrndloa.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2duijrevu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ubuzivyr.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xmhgmarl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2kptrxstk.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jahmxmrl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2bjrrognk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2mugdswem.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ohrexksf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xdxlrxde.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2revktfge.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qzqmlvry.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ksmypydj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2cudkjgaq.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2aedizahg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2kpygrygd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bvbxapqt.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2juhcqbap.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ksowmlli.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2knmkrhoo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2nlqmegkb.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2wgowbyrd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2efvgahzp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2afmjszdo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2icbbhnev.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2gmvstvgo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2yosothkr.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2opbtedpe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zfwshczx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2nbmjxjmf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2xrkwfcqr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2sfqyntoq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2bjrnkevi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2pxacttmi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2huujeexr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ucnwgrlu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2rbhcdulb.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mryaixav.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2citxinxp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qfhpzdbm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cbyhclfj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2sgzpiumw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2drsbzedx.html


<!-- 参考信息 -->