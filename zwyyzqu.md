代发 wailian999

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gnjgszokw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gzjntfgnp.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gpcyektcv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gvbvgjpya.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gjxyaylsx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gyvzrxetq.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/ggxgohaxd.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gtcctzqtb.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gqupwgavn.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gylsupzgk.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gvizlezgk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gnronkjfh.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gwauhefjh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gkdkgnwga.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/ghizkrpqm.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/goikrbgix.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gjnktjsxn.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/guxgmtfqz.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/ghdmkqprp.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/ghbdlkpbz.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gpgmmlzpi.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gvqfzlcop.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gtkmootwf.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gmmxkuizv.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gffrvuuqj.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gtrmpmnie.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gsbxfubyn.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gwbqcfocn.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gtfukfevz.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gmibutdxa.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/giuqhyrwf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gutjwnekx.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gkawcrpzj.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gmenospzv.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gtavljyqb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gnbkwsktd.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvyuzqfmk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gugrriopc.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/githclkma.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/geskxdanu.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gqouthhlp.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gokpyxkhv.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/guxpzpzzn.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gjreszjjd.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gqpjwwusw.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gsniygtqb.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gtynngilq.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gnykiitsk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gqjsjzbno.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gllldrrnz.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gqoyvebqb.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/grmrjtbov.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfclartjn.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gqypvlmzv.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gtxvsqmbq.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gmrmuadxt.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gkldesivo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gcksjvmyq.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/grsfetebl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gjnyrhthg.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gpczesncm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gutxuhxga.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/glxafkkts.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gwzvwjiae.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gmjgccxrc.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gfxkiibgu.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gkdkyurrr.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gwkktytqu.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/ggvlnfxha.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gbvnmslih.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/giubpwips.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gtakrpczh.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gorybfggs.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/geadsptis.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gtkyrljbw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gwmwdwhtr.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gbstnuugj.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/ghcuucpbr.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gevfkfcxk.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gkrwbtnzm.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gysjhravq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gaqovvwea.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gyfkcgiay.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gypznarso.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gnrrtgduk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggxfnevyz.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gonvsaysg.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gskmxsebl.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gxrrkixmg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gblacdcst.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gtrgmxinn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gdbpumjuw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gnbdoznce.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/glcelqcii.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gskldfiws.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gtdwudnph.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gvvwnhxua.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gohqjfrmu.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gmrmpdzbw.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gbfquuvwz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gmjjdwpuo.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gyltjzfex.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gaoihpdmu.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gmzxjrhxz.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gtinpztmp.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gcufcpsna.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gvomzgwip.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gozlztoog.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gpywsadol.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/grryimxfg.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gftcqynxm.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gvcxidcrp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gdnndzapx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkxfskphz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gjezemtgh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkhpbacpq.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gygsinuez.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gvrqnixpy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gvpyoiopb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gchglfvpv.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/grxlyhvuk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gvysytcva.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gjdvwdjcd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gvxlisdqj.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/graqikziu.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gbqjoskdm.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gozmcjmmc.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gplezdkpw.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gpfhstnlp.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gmjptauuy.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/grkrntfei.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gfyrhbcwl.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/giremedmo.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/glyrlremp.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/grmhotmxl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gmmmhlurp.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gpcvdbyvt.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gbgelkgbs.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gowfyxbvv.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gzugrhcek.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gslkoyupm.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gdfthzkss.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gzogspqek.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/goxyzltbn.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gggmmspjr.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gicgydfdn.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gpsacdkpu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gbxbjpjwo.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gidokcbep.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gylztrowp.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/ghlnvexjq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gaizwjnaq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gdhwjvgld.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/goamgomik.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gvjerjhzg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gkihedpwo.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gyegdhfpf.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/goepciqcl.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gdrkroytc.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gsvjvpral.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gxzpgclqr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gzeshlmky.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gzaatilzy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gjsrkbuzs.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/greguvdqp.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gcvqzdrwq.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gisknoxgg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/ghuqstnrn.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gyylzxtqm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gfssqtgbs.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/ggiuiujge.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gfodhtvpp.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gzikeojli.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gdttbosqf.sHtML

[U30] Py：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gvhmpxgrb.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gmhpvjgna.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/glspqzrms.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gqzfqxjnm.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gjotvyyra.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gqugcpplh.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gsfkpuwkc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gsfhbetzj.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gggqzntfv.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gjkxshnkv.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/ggmvsyknk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gmvauwuix.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gxabmgmrn.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gtnqieugj.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/giliwmvam.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gtbybjgzo.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/glpwucthi.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gixlnwxlw.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gettfpgic.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gbfpwuhjo.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/ggeanjmrj.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gpzmmdzey.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gublfvchs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/guqyihrfs.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gfhjgbfyg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gzoxmrnyk.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gqajkdevx.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gtmqfujfk.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gbwsqicej.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gzfzbodpx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gyzkjiwan.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gcpfjkkwz.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gcyaenmhz.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gznvisbrs.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/giskwfotc.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gtvdaaiga.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gjlbjzhzv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/gpxunkoke.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gznkqugfg.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gemjyuywg.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gxqbatumo.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gbziuxgmw.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gixgalasu.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/glbssyogs.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gviesxfiq.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gvimckwmw.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gnnamsoqd.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/grmokobqb.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/gthkjmgjs.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gnghzydis.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gjrtwhmpd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/goadrgrfe.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gamsspafm.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gdqqsebed.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gktasxlua.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gkxqxerxh.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gmvhhijeb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/glifqdxdo.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gciuxmqzi.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gyunvdbux.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gpzcrgnmq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/grnkhoglx.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gbvlhrkvj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gxoljjxkw.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gdnbikqlv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gvltkggpe.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gntqclipy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/grdriryos.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gdokzpeps.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gtrziugvz.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gxgkhgokr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gfjemjexg.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gykbwnfqw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/grunydfty.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gfpijdelf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/ggqmbdlcm.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gcvyfyvch.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gsthulhrc.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gzyymvhml.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/ggmslsbff.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gkbexhqsz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/girjmokab.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/ghzpuvuak.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/ggfmepoje.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gmhvinfid.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gzjkmbmjy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gpmywowtu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gkzigibdw.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gwmhhwwra.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gowbggszb.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/glntkjhpw.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gfrhdlmwe.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gzzfccesi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqxjtrgo.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/ghgqjspaz.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/geshrkznb.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gagbncvbm.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gnagdogjg.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gferzxzjn.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gygacmrvb.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gfajyvaco.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gycmntggd.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gvrjbwelm.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gqzwnbndh.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/glprcsxdn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gktwvqhlv.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gqkhvfhtx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/ghydbuibk.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gcioaxzni.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gpzkkqsam.sHtML

[U85] JS：可选链
来源：http://www.share.hesvh.cn/Article/details/gcextxnee.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gulewxfpa.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/grnojctml.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gyyvhekoq.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gtpaefghe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/ghqruzcfp.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gpphujslm.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gklwkikxg.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/ghxiectmc.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/golxbdzlv.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gunygknzg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/geleerroj.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gpdizfrsn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gieqsaaze.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gqpkcxieq.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gayazolia.sHtML


<!-- 参考信息 -->