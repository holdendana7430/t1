代发 wailian999

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2khpktotf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hkcfatpc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ewoftpst.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2qmwxhiux.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pjwsyjuc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kqnltcdv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2alzamgqh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2npjzgusx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cluoibaj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jbvexbor.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mivixiwc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xtmzaqkv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dyvgxjca.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2wjgitcej.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fctircpr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2driosuln.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ognmmwqy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jwgwswbm.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2dtwwysrf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rgnqstsu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dwmnrrwg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2vcewwvox.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2dvgtlpyi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ueedxaiq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jthyoigx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjcxonhd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hbrwopvh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qqonlcjl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2heqqneco.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rqgbtarz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2phaxlwxq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2afunhsjk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2dzlykrmb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2nsgwymiv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fqeeifsv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2tftodrqj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2tgzlkmbs.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2pbfudufy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2yxzyqmdo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2cejzcfju.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2gcoghxiw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tbfcjmut.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2imiwjtpb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lrdyjpzy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nzfrqhlr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2pbgikcdy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xiwoyndv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ulxxpcnq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wbmksdxp.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2luoksyqj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vxnkogmj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ytareuxb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rxfdasgj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2tysqreev.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dpthkjkg.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2okktyfuk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zvgovqdx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xpdsunsw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2pbwhtteo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2dalzlfrx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bhiolrce.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wmplcdgm.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ywfqqovz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2khzrwknk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2huyokcci.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2omabqjop.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2htzkuptn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2myhviaix.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fkrwfzjx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2eyjecuib.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2yvhviesv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ggcjvdek.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jleeuivk.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2gjzlnpqn.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ajwwofgg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2wxipfjmg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2braxnkqe.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ktziirkh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ghvkmzkr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2dnevlcvs.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2boyxdkgt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gecgvqqt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2eojiworo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vbsfpqgp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cfmugkyg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qbkkpuds.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2oiqflyds.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhmgwxpc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qhkaycvx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgqmxgsf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zmuouxoa.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vjhrndqr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gbaenglb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpqpkolu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wgflcxfj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lzklggws.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xhysywia.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aozfyaya.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2immgxlrr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2taejougt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahgvufsx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2inpsqpbz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cuwntrik.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2muxzkqys.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2bgjdapcj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vdlfphhx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yjnkswiu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nbbnngdm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2byqnxsyu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zgrjnipm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdpchmgz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2alxfhpsm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zoqhtdmm.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rtjatrcs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nxzowjtp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ogdkdumv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2uhcwwmdf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rnykmedj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cyowpkds.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2mhzteidr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ucduiuse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfxgihfl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ytjewixx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yltieyow.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2pualzkxt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rqopbbsu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2yvpotmhs.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2fdtsavcw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wtnnydww.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2oswvpboe.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2emfydyll.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2uoljzukq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2cskfrkws.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gucuxcqu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2gindgwzt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2pvrqafse.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2djquhuvq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2riwexieg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pannbiaz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2vxuptggh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2pjuukxrp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2vdvyylmy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2yyqmmnkq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2iahdehvg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hydnbfzf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2qaxylorh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dmmhuuug.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xiyxwvld.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2plkiryxu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2clewftto.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2fexdfrtf.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2cgmtdvoo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2dctnjcjr.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mibzpqrf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2qojfyixm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2kiayjxnc.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2jxltgonf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2lgxpzbxs.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2cnklwwok.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2eyrpjemx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2qbkjrlnx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2lnolikgm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ppcnptrj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ljipzyaf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2znsntmwy.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2crrhnioz.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qaqgahvp.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2acilnfgw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2drruywda.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2nsdkvuwf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2bflewhcf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2twlazkva.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2rzmxfwoe.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ttkmglcm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xgwsytbn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2cjvhodxd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2uqmjnccg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2advujrrq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2wexyvybx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2emgipfjq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2jawcfhyz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ikdfdehk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2klgcxgbq.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dukvyrjs.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2kmkrzcvm.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2sdxdjzcd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wppvynmz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2tncmycmt.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2etihvekq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2bexynuje.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ujeolqee.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2dbjgphbb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2jnzrbisn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jadkrxkm.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2newliiww.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2bnvqztke.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2jywwiamn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gofogjux.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2chdylchh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2amqgpvqu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2rbjmzmyp.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2rfflvptv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2aquzmfoj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jvxjntjb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2zequfddx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2qzctopgq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ubeiffwl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2doboczhy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2svlxpklv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vzspuhhu.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2oylpofwp.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2zmvknxei.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2fstplukn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfnjzjxc.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ituhwhaa.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2iochhrfc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2yoseqcgx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2kxuemlyk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ittnjjnh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqnahgun.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2unhlaydv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2gjojtpit.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2xutlatba.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sueyrbwg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ycwljjuu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2qtecwyie.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gojnhuyl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kqtxrpij.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2gwqbjgjm.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2wyfexfxi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2iayouryy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2tunbffnm.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hllvcnya.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mjtwwgol.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jxgxkodj.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zqzhouvf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xzfmarcx.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2wcxgizlo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vhwayclb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dcdczaol.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2oeoyqslj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qyyylbla.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2yzzclasp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rpogkvie.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2yfcakoit.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jgefsqgm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2gayxidkg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hmpwdfhr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2nnoutwmy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2xtkjifcx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2stqrhyvw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2kmodavuy.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2yciftfsc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eqiewptz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2uelrecnl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fnnjnfdx.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2fzzahbwu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2meumrkjm.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2dcvlcuqt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2urdfbhba.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2weztblil.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2jdghesub.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vsxjrldn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2wifzbfff.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ntuexpue.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2glvyyttv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2krawesxl.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wxtdsrch.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kgwcjhyr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2qyyadqxp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2snnzmopo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2jawhqppd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2eisigvft.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tbtscfys.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2lreknjxr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2erblddlv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2mqgvpbfd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wtgnvkif.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xneifzlq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2bggmulwn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2kernlgqk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2whppvfhg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2gigyjxkz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2hhobkuan.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2swgyfpoj.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2glaogjpx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2xrsmbjxu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ucfesrhl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2lpctjgua.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2koakjgyx.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2xextncfq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2veeshpig.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2owzuelrp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2mmgxrkvi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2wjecbtpr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2uxrnbscn.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vjtybytj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ufggsqee.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2orecweyt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2atcywrti.html


<!-- 参考信息 -->