代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dlhthxyq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gwclsebu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dtmbplso.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2opaxumem.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vdoqzqgx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2xxhqfsxd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ztfzzerb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ntxzbdhm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rhxqxube.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xlkfqzth.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gpmgyxpu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nwmshnky.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2dftfxbcg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2khkrlumm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cwuzofbz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yrqcwczk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wxogkbkz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2gobhwcvd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2zoytapoq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mygoffuc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xdrtmcpd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgtnfrfs.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2fzlkhrew.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xfswiomc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2tielmvva.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2qewfmnns.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cimkzeqs.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ygkjoaub.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2yqjzbxzi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2alhkmpvo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fevfttmj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2nkyovptu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xjictuiz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2clvmqfqk.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fcqjnsrs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2lezddyrp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kumbnvou.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jtpkylis.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2uylsibsg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2qkrjknom.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2vixetypo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kfnqmfxw.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ldwpncho.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zwnvhinf.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2qksvdddi.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2unbfqkwu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2krsmnvve.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2utayypvj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2lxxfjdei.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2afddkmbp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oabixoox.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vybhpbso.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2odnjejfd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zmfhdhpj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2umkxiseq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hnvohyca.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vrgewjnr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xfdkqfge.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ftgxsvhc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rjnlfdfu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fqcgpvka.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2lqrdgmvf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xmeehpvz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2wqemksdk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gajiusec.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cysxvhfg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2uxnlardd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2sertdpoa.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2kgkzvbzo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ftgwbids.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2oraiihfz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ifzfykuh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eoeyedon.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xictneqx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2uawmwhlk.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ppxaxytb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tmjazgnu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mduuscit.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hvkitjod.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yeiyftyv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ufjhllao.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2xcedipka.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cttlmrbr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2laevurwp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xuoobvuz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccvuuijc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bldzhtch.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lktbkvgs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ofcarelt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpvuqacr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hurecwts.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2cxkrsdmd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggqnwxwc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tnjhtrgz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cbfmfazt.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2llrhihql.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2demnjcbl.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hyjjcvyd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ktzsvqzr.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ifyyrkks.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zjzlfhmb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wysgptdg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ffybxjos.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2rnwvvgeu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bskbkuxb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jjzlzzai.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zvnyfdsz.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2fmrlubok.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hpihreus.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vpavjqlc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bpimjznh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vmnspede.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vfkuuiyx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2fvibtdna.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vvuwlknr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2kfcgthzi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ibyqwtad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxhfkezn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uidkdakm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzexxcuv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2htsumayq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rstylvlc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xlzplmpa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qmpphtst.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2xwdpufjc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2dmgoqcuj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2anwlnkvi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2pcedxmos.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2iybykfya.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fxrfnuft.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2bqalypvd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gtoipcxa.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2sjowmbwd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2attaazmc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2khbatjdn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2lhsuoexu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qhrwrsvv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bmwhkcif.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2yzhdtmtr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ovaiwyvw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2zywjgqym.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cvqxzafy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ygzjyakw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2zzkmbuxf.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2fnzcwjry.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2belwkmvr.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hezdruah.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ubwafbop.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2wehtvazc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2bgdewaig.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hddyskfh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2umsjnfkz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2gujudhdq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2zidabbvr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2pmkvtcyk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2oydkbeyc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zrjjbwzg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2qbwsgyis.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nwxndqfr.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ktpwxfvj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2qavawbkv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ccgxdfuo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ofmaweda.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2kdlqvdbz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2rqfgrtru.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2kkuqbkay.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2dnpqilyd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zsrutudx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rggrrmaw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fubqdtxc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2pvxjlprx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zkgprazp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2uussvrjz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ujdcywom.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2diqzlaio.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2iyelkzoh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2hepbchbn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2lamnattl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2stxxqohn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2texfddjj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2dlcokotd.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hmrgocgc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xsuvpsaw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2dqqkmxil.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2uuszjkcg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2umslskaj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fucuikwz.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2tttrjtza.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ddxwmnkl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2eknjrrqt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xcetcskh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2xalgublc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2vrdmzhby.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ywgemxcn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2qxtbbvuk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2eapfsykk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2uitfgglk.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2dcnvkxhg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2hfidgieb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2sdcicerz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2oughhlop.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2nlwobsib.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2nxvaltvq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2kzkzokyv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2txqukrrh.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2depdqpbd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2kmcdizjn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2uminzqkd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ijbhkreu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hhqtdgbu.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ysrzplnp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2skhummth.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2yhviptpx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rfmexwmi.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bluedjvz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2gvbcwlwp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2hvfrubwy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rmnbvndw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2omkmmlos.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2lrzmjyqw.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2yyptdvcj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2pegyakls.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnmuwoyi.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2eurzlsod.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ruxzthoz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ltgotsnn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2vcowjxal.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2hokzwsig.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dfotxoet.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qboivlby.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2sbiymjdd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jkaalchf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qoqefirg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ulzvqqhv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2jfoujdwd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2phbgyxrg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2pemvduez.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tnupymqk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2bezpcvzl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2acuwrawt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2qohoketp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2cgxbstie.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2okhihyep.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ojhttjzm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2zpwmmrld.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lhxdgyga.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mxgyaymu.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jmsawzgx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2gtmhitsm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2idgjsqjb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2rvobfbze.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tkftpxti.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2pzfoxfzs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wtispeda.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2zjtjodjl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2xfvxgbns.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2maezgrfe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2hjvccrpc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2uwovslxr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ddxerjzb.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xgqjxbcp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mydvxkeg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2zgoettkw.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2nqraxxjo.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dcqfokes.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2uodbswhq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jklgcubf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2eaajhimk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2btaeaedd.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2casmsyrx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2wmfhhxea.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2hykiphpo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2aivictbu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2rktxegpf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2iyqowilu.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vykrprps.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2okksmsla.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2cuvvkryu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2puncaupo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2nzokrtuw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2vrvbcsql.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2kntktedy.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2czpgfuvu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2koyfmkut.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2icxnfriz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dnkcpftu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2prtlcgwc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ibikezak.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2orunlghx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2vfyaqytx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2pjelvsqp.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2murioltp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rkspplne.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2gwxzbueg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mnrzwttq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2idasrnhz.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2rcegrbmi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ncldyohx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2odpothfl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kxexifgq.html


<!-- 参考信息 -->