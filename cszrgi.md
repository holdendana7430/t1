代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rhmugwhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rivrdudi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2uhzqjkii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csdygrwb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zlaziuor.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ibrsycoe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2mcvgnbkp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2swzgjmpa.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2sadlnbut.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2pukqmijz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ldohddfx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2nqkbihtn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vvpqsnjt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2iyurxerl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ncrfvusd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2flpxxjet.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2epjjvgnw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2gxswykwg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ykqzgjdk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ogzmzzkq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fnnjrczv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dwejycgn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2jyfougyz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2czjebypl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ypnooayg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2fvsqjscr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mfkwnvyr.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kwpurfzj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ljxtdprb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ppnaafbd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qnkgdjff.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bxapirvi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2gyrhvwzw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2degpyzjf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wkviblhk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2iuvhszqp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2mziadtjj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hanklnuu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xydrakib.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2hcmgvesp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ceyjuyrd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wmwoajhx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2jzxvyesf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wxnbcsel.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pxwxvdda.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2tphoqwqw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2iixbesiw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jdwrqzbj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kuigmggi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nvichmsq.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wmymlgcz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gzzfjlmx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wqwcbwte.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2fhvdvbut.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pbcmqnsv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wiolvkxu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ioohgwub.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2rqyeoqky.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qyfosebo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2kxcgftpa.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pnwtpxgs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uakffbup.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2amkqlzaj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2rrbdrgib.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ddylcadc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2odqmjoza.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2cdxdbrxh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2cduvuvbd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ahdjifdg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zvvlmtoh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2lwmxqqmp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ggmzrofi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2vkkiozyi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zwbmogef.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nsgkcizr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2gqcplkcd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2aphbdqmg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2bilkiocb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2xvrwssdh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2cfmfwmct.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wtslydmn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kvqapqzd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ppkoejht.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2azthntvf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mwyngowr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bosbkwzq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2wrvkvifb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mdgdxbdj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sgmltypg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2cpstdwwj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cnutjdip.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnbynxsl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2lsdtqljy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2auhpeksr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2xgwlumdm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vmziozvn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2jbejjycm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wxvbnheq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fvcdpuvj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2lonpuwkp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ylxcuatn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vrtcshte.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2enpywyet.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qiltqlcb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wnbkachn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qwmwjaiu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hamwnujj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pbpkjomk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pwanngxo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pftocsaa.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tormguxd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zcfahdzm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hosicstf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pjohcjty.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lfgkvzxe.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2sgafevbv.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2jafzzgjs.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pwtqvtbj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jdbmglge.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2sezmtwsn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2apnefquo.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cmtlqppl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ctwucziw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2nxtvwijm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2swzwlpmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrhxfflh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2skyxgjls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mncbtvqv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2abtzddwx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2yprhbujf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2qovpxtpa.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zgjwniks.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2gdxeslce.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2fgebynfz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ieenogyg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2omuwfhtp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2gmuiizcr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yieemmkl.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ocbozmwq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zzxpxppt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2zwmzycjc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2fdorpskd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2gwaoyyhm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2sbrmhlio.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ommffzdq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gjbbjkgt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2qnvvscpe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2dzgxlque.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ovadwvzq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxwpvypn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2cpzcbozc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ldwijpvx.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2qisqnefc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2bmpqgrum.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ufxfjhib.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tqyqrrhe.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ojjlzfsv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2gzpbedmg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kiheduav.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2qolookiw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2redbfvko.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2xqabbeou.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2bjbrrxls.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ssagbpps.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2cvvxbtra.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2obvmvajb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ymkjblkm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2mjzatzld.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2rqirwsiv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2wxxtmzca.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2fhupelda.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2sgeluvst.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2sfojowzw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2eiwfmigw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2zrkyawbj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pjvxjgwa.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2qcosumqv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2telgomte.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2qhrksdcb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mkbywugf.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2cgzeetmq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2uavedsxv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2jeczqhpx.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2jyaokzqq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2rjvldrbz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2dutqshde.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hxahyxjt.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2fkaqrynh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2urtvsqjg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2gqupvfri.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oxwjwgcg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rvjpzmhg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2hkjfhclt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ejajpavx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2giobntjm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mkfpkrzz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2szmpwnus.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hopplggr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2bnccohoj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2laoajudq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2raaqxmht.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2yzixyltv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hvlhrpth.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dwdxqmro.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2srkxvune.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2pdojlfxb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2lcllxzeg.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pscwoqdd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2pkedthiw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fzqvffda.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2sreknqpo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ntigrjyz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gebkuoqp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2zaltnzyy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2xyfidvvw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jeflxbgx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2njffgopa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxcrhuzd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2sbgvkvcv.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2aetvytgg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ejyknxgt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2zyimxxeq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hppoljks.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2fgrpwsox.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jlnlorjq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2qztewvbo.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2rpbmywhw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hegszklp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kfgjcmli.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xrqsageg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rodidzxw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qsisbcmt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2kitqcpth.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2vvqknxbd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2hpjcvuxw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2cotxxlwf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mjnnhlka.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fopjvjde.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lqifxdmv.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wgnfcmoz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2biwevafz.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rncvgeqb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2tqzbxaoe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qggcksjo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2mmtokaop.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jpvfsbap.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2idrhkkyb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mrlrqgqb.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2utgjyedi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2edsmzolm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2muejfang.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2scndkbdn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2yknqngob.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fweoeqfv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2skhxgmga.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2aagdqica.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ncxkjwiq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vwdnfqzg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2drrjkhso.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2indqdrmp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wbymxaxd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2smkrdxjh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2tqxrmfyb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2aigekxlc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hulwsurt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mcwwncrz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2wyojpzno.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2wizytzin.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xdkfuxrk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2oxeeyvij.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2pegqljui.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2riphbsbn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2sjxaqrvl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2amobfvrm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kkcwchor.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2gnopmvqa.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2rcxsbzka.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hbzuhljx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2tuqiayxs.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2habobeui.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2vxhmwrpl.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2zwdvfukf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vacjcdej.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2canwirtm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2enrtbdgv.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2imsunwys.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2otqyitay.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2tbegqzxq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2kipvzakf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2mktvolae.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2htbdloap.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2yjwszfuv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2fywjinri.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nrctvofw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2uxnuckiu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ngxumevt.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ckuzdztl.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zftpydvo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2pwtzrvzj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2rknnwucw.html


<!-- 参考信息 -->