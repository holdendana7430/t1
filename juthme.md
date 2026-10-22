代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2piuzpqzm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2vczwioms.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nppmjmtw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2nqozggkj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dczejkmn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cxlgqesx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vuhgxkwp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ymayzkyv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cskbijnz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vfexkblc.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2kgdspwwc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2wxlfrjzm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2nhhvtwph.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2fnpcloub.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2rwxtbcpd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2dbtsueyx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2slnpksdr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mggediic.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ygzdtapv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kygmzcpc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sdatjmyq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jiouxoho.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2otazozvu.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ncaheqty.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wulbcnfe.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vnjngwrh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mzqxtspc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uwggddzq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2odjapbck.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dqdnsbon.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2claaexpp.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kjddujws.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xzqfjjjw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2rvbuuijq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2bfabszfk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rbcdbtdd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2pjzrpwmv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mrxorhfs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wujtwvgd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hevppjlt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sixzajwm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cbyxjtyx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ifffseqo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pzilguri.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2gfvjkatn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2lkkqxiaq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2cqgopwdr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ykyhkubm.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2sexofpvd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2pkvvriel.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2dlkiazoc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2yvrctlji.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rqjhgjcz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2messpcmz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2qqunozej.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lzvdwnru.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tvgfbgrq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hrswqxhk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sznqchyn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mogivhfy.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yidonjas.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ghwdsttl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2lnxmdpdy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2qbiqclaj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2idmixdwa.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nrejnjuk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2lowrxajc.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2gtezlijl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fwjnuhdy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2lgdwquqo.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2uphxwmui.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fqockmtl.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sjoinzns.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fwjzfpxt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2amzkuucv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ryamovqn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2doxjxxpf.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2bbvfllgo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xukhwiia.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ijnuanyz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rxikalyk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2tlvxamgl.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ijgokhhq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2nbhvtmns.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2atbjfamp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbenorsg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2odytgenb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwjabtue.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2eepgzash.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2krpsjbte.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wiudlhck.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2sjsdmafh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ixafmvtp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aaaokibw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wndayaan.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2muakxtmb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmxycuyp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sedjbywl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hwliguko.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2gwllpxrp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2deuyqmdu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kelkjgtw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wnwtskkg.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tvoilkay.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2smlldwkn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2siefzdmg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zleewmnm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2dtcvrskm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dioerxln.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pxveyqdd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qdovjtwk.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2loxkjkdv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2odtxpqki.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ufegdbwt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wrbaflmf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2udoofmjy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2gmvogynq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osrpsdze.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bqrjzmvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gczlfwte.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2pittftim.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lddngxzb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bktnecta.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qzqvhsgs.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2sgwtrztk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2eyylclty.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2dwwzwakw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2yitprqsc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2nspuxdme.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dwtphing.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2nooavfss.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2npjquozq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pfnchoav.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2cplgvmsz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2lqnsuenk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ftrkjpjn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2gevgnbix.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2fcitturc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2rclerpmw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2iksiqwfd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2qntojdup.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2nvszlatr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2dwdpmuvh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xeeuhxut.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ulrqmghk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2gcqkmggn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2egxojydk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lsssuqca.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2wjhtghjb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2yzwpyowi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2zweztzwb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2sdtkbwpl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2cnanoesg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2wbgaignp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2agpmjbfe.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wbatgprm.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ogtckkir.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fskhzwuk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hdtkitrq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gjjxftbr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2mtxutkds.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2gcvqmihb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ygldnnla.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2zvwvdufc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ydjmrxdu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qjipptoq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2bzievymi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vrufjjkj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2koxvfvnc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2oqoqlxtr.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2iexjerwc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2vxjkymjs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2gjamltsg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2agvyigyj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rkrzrssg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2mofcfimb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qnutjgep.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2kukbhqbk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vmxhfijh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2diejowfv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2vkosqjsp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2nnnyqchp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vdggidqh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nohbdrdz.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2zakfkqnu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2gggabjyr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2cgjiqfki.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mgxtbynm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2sssfhely.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2igmilpys.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2leqwihkw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2lscehwlx.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2kvbkxoxv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2bzwsqghh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2kkpkhnaa.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2wakttbvf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2tcycwctr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2kdxnunxp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qpiwknks.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kukyttud.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2igqjbtzz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2pvydlhcc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2efpadwbl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2edmmlgjz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2dxssmbtb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2leelehgw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2dpftlqoa.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2exrvigwj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2mrqpbtxe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2piiwlpzk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2klwpkolj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2nebgrxmp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2bvnhpckt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2iostowax.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2izcbxsts.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2grvjdkeu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pfescaud.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2ewvkgsiw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2jlvqwgco.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwtwpoci.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kinpdhwo.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2lnuitrza.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2knjwyvnd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2cerpnsgw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xovwnlfg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2zmrhinql.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mzmqmrde.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2efkyyoma.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2srfugzye.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ltwumckg.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2emeujkkz.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvjggvfe.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ugnqasqo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2obzotgpa.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2zdikzqfs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2tkeszcob.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2oevnynyi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cedcmunq.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2lbtqbqlh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2mwkhxvgv.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2spahnljo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2biismzgi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2gnnlxyut.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ljfxevxt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2otvnwbsq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ujjdidbm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xpvsmvcz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fgnsmytu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2woxfvaqk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wueopvwk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2lxynflmq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ytppenra.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2sxwwlyub.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2dvywakro.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2vcahzzub.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qclnvfnn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2qrfxsznw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2voeyvxng.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2aecrpkub.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2tnjjtaab.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hvnwrgzd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2bklgmjed.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2itwzfxcc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2rkvdimfw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hdjsmezs.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2pdczkmxd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2leqefqnj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2fhsudexk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2phgbbjwl.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gazfoikc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2gnvjcddg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pftynrvj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2znsovrls.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2remgpxkl.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jkljnlvh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zwfevypx.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qabkavmp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ykuqimhm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2xtvlkkzf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ddhrnzax.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2cwkpbski.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bbgnjwyc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ozhbjjht.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2maogklnq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2kykzofdp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2djoohirz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2bzoxnntl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2wdzwqhfx.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2kgewwtra.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2qnnsmvnx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2cwopyyyj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2wukoxwqg.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ibusdvhq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2decekxsj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2inmridbx.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rnvooivi.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2teszptkg.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2maowzacv.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2okpnwwxs.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ppwnxpix.html


<!-- 参考信息 -->